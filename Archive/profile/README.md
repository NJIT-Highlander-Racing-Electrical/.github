# NJIT-Highlander-Racing-Electrical 

## A GitHub Organization for NJIT's Highlander Racing Electrical Subteam

This organization contains individual repositories for each subsystem on the car, including:
* Dashboard
* CVT Tachometer/Temperature Sensor
* Driver's Seat Pressure Sensors
* Gas/Brake Angle Sensors
* Fuel Level Sensor
* Dedicated Data Acquisition Logger with GPS
* 2WD/4WD Engagement Switch
* Power

## Important Links

2024 Baja SAE Rules (Rev A, 8/31/23):
https://www.bajasae.net/cdsweb/gen/DownloadDocument.aspx?DocumentID=024d6763-9fb8-45c5-b87c-08351214cede

Eletrical Inventory:
https://docs.google.com/spreadsheets/d/19zXsWbHnRgKuqglurabbrF1yi5oSlVw6kvXuMUWI1O0/edit?usp=sharing

Electrical Purchase List: 
https://docs.google.com/spreadsheets/d/18E18Z8eGh2aedHmGQmZOifpqckm16rXo4czgnBeM4RM/edit#gid=0

## CAN-Bus Information
* +12V on Pin 1
* GND on Pin 2
* CAN-H on Pin 3 using WHITE wire
* CAN-L on Pin 4 using BLACK wire

* Note: Newer microcontrollers do not play nicely with CAN/TWAI, so any ESP32's with four mounting holes needs the CAN frequency doubled
  * From this: https://www.eevblog.com/forum/microcontrollers/psa-esp32-can-frequency-assignment-broken-in-chip-revision/
 
* We use the sandeepmistry arduino-CAN library: https://github.com/sandeepmistry/arduino-CAN

* Our ESP32's can run CAN-Bus reading on Core 0 if necessary (utilizing tasks for dual-core functionality)
  * https://randomnerdtutorials.com/esp32-dual-core-arduino-ide/
 
* With CAN-Bus, data is constantly being sent to and from all devices in the loop. While not every device is set to receive every message, it is important that there is a hierarchy to the messages. This way, more crucial data is sent first. Our Message ID hierarchy can be found in this repository.


## 2023-2024 Design Goals 
* Custom PCBs for subsystems where applicable
* Custom durable and compact 3D printed enclosures for subsystems
* All data outputs from subsystems are shared with each other via CAN-Bus
* Any data on the CAN-Bus is saved to a dedicated DAQ logger
* Single battery that powers all subsystems
* Universal power and data connections/cables throughout the vehicle
* Strong design process documentation (photos, schematics, research, etc)

## Electrical Design Timeline

### October
* Finish research
* Create a Bill of Materials (BOM)
* Meet with me about your proposed design
* Order Parts!

### November
* Work on breadboard prototyping and programming

### December
* Finalize breadboard design and have a close-to-finished program
* Create schematics for custom PCBs (if necessary)
* Make sure you account for CAN-Bus and 12V-5V power conversion!
* Order PCBs (if necessary)

### January
* Solder all components for permanent design (on PCB if necessary)
* Test circuit and program to ensure everything works
* Begin designing enclosures for your specific components
* Accessible enclosures with cable holes and assembled with screws
* Compact and durable

### February
* Final design and program improvements
* Begin testing subsystems together (dashboard, DAQ logger, CAN-Bus, power systems, etc) 
* Post summary of information to GitHub (if not done already)
* Schematics, code files, photos of device, data, research, etc
* Assemble systems on car (if the car is done)

### March
* Assemble systems on car and drive the car to test!

### April
* Competition! 🎉🎉
* April 25-28, 2024
* May 16-19, 2024

### April-May
* Season Wrap-up
* Make sure all documentation is posted to the GitHub
* Mentioned what worked well, what didn't, and what we can improve on for next year
* Take inventory of all Electrical parts in SAE room again

  
# 2024-2025 Plans

## Future Goals

### Wireless Communication of Vehicle Data
* Transmit vehicle data wirelessly in real time to a dashboard/control station on a PC
* Use some kind of long-range radio transmission

### Common CAN-Bus Library
* Provides all variables and functions to read/write data to CAN-Bus
* Simplifies each individual subsystem's CAN-Bus implementation
* Far easier to update CAN-Bus functions system-wide (just download most up-to-date library)  
* Enables every subsystem to have access to all data variables

### Improved Waterproofing
* Waterproof connectors
* Grommets for all wiring to sensors
* O-rings or other seals for enclosoures
  
### Miscellaneous
* Fabricate more kill switch mounting plates
    * This includes both the rear square tab with two 1/8" rivet holes and the front tab that wraps around the switch body
* Fix 2WD/4WD switch 9V/12V toggle
* Mail back X2 transponders for newer TR2 version
* Take inventory again
