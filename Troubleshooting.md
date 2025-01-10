# Troubleshooting

A list of issues I have ran into, with fixes, if applicable. Originally in CAN Bus repo, but moved over here to be more general for all software issues 


## CAN Troubleshooting

### Received message data not correct

I had an issue where the message data was not updating on the receiving end even though the changing end was sending new values. This turned out to be a result of Serial prints in the receiving program. The sender was sending data about every 1 ms, but the serial prints themselves in each loop were taking 2 or more ms. Increasing the baud rate and making messages more concise fixed this.

### CAN packets jumping to wrong case

This follows similarly to the issue above with serial prints. The long serial prints and low baud rate resulted in RTR messages that we sent out returning to us. 

### Received Message data bouncing between value and zero 

This stemmed from the switch...case statement not being included in the "if" statement that runs when a packet is received. Since the packet was never being parsed in the if statement, it would run forever even if there were no packets

### Subsystem that receives RTR transmits its response many times

This was due to the issue listed above. the switch..case was not in the if statement, so the RTR was never processed properly, and it kept sending. Another part of this issue is that it would still send four times after this. This was due to not checking the packetId, only checking if the packet was an Rtr. Thus, it was picking up all four different RTRs that were sent, even if they weren't CVT RTRs

### Message data on logic analyzer does not match what was sent

#### Data is consistent, but not accurate

We use CAN.print which has the same functionality as Serial.print. If you send it a "1", it will interpret that as an ASCII 1, and send the hex code for that instead.

### Data is inconsistent

If random data is coming through over the bus, it could be a baud rate issue where the clocks do not align with the samples. However, I noticed that the termination resistors have a big effect on noise and data issues. I tested with a physically short bus and three subsystems, and it would only function if there was one CAN pal with its termination resistor enabled. With a termination resistor on each physical end of the short bus, there were extreme issues 


## General Software Troubleshooting

###  Task watchdog got triggered. The following tasks did not reset the watchdog in time:

This could be happening for several reasons, but in my case itw as due to IDLE not resetting the watchdog on CPU 0 (secondary core). If the program is stuck in one piece of code too long, the watchdog will not be able to reset and the board will crash. I tried adding a delay at first, but it did not work. I determined that the issue stemmed from the CAN sender code. Since I was only using one subsystem at the time, the messages were not receiving an ACK over the bus and continued sending forever.
