# NJIT-Highlander-Racing-Electrical 

## A GitHub Organization for NJIT's Highlander Racing Electrical Subteam

This organization contains individual repositories for each subsystem on the car, including:
* Dashboard
* CVT Tachometer
* Driver's Seat Pressure Sensors
* Gas/Brake/Steering Angle Sensors
* Fuel Level Sensor
* Dedicated Data Acquisition Logger with GPS
* 2WD/4WD Engagement Switch
* PC Base Station
* Power Systems
* CAN-Bus

## Important Links

2025 Baja SAE Rules (STILL WAITING FOR THIS TO BE POSTED -- should come out end of August or beginning of September)

[Electrical Folder in Google Drive](https://drive.google.com/drive/folders/1Pz5bq8r8b9oh7MFo3oWOcobUKbDVZDIy?usp=drive_link)

[Electrical Inventory](https://docs.google.com/spreadsheets/d/19zXsWbHnRgKuqglurabbrF1yi5oSlVw6kvXuMUWI1O0/edit?usp=drive_link)

[Electrical Purchase List](https://docs.google.com/spreadsheets/d/1hTMg6dxTZtMp4cDH3FeMRMjF6Ft8n0DMCeNlGOwD0Es/edit?usp=drive_link)

## 2024-2025 Design Goals 
* Custom PCBs for subsystems where applicable
* All data outputs from subsystems are shared with each other via CAN-Bus
* Any data on the CAN-Bus is saved to a dedicated DAQ logger
* Strong design process documentation (photos, schematics, research, etc)

### Wireless Communication of Vehicle Data
* Transmit vehicle data wirelessly in real time to a dashboard/control station on a PC
* Use some kind of long-range radio transmission

### Common CAN-Bus Library
* Provides all variables and functions to read/write data to CAN-Bus
* Simplifies each individual subsystem's CAN-Bus implementation
* Far easier to update CAN-Bus functions system-wide (just download most up-to-date library)  
* Enables every subsystem to have access to all data variables

### Improved Enclosures
* Durable and compact enclosures with reasonable mounting points
* Water-resistant connectors (aviation plug connectors may be sufficient)
* Cable glands for any wires that are not part of an aviation plug connector
* O-rings or other seals for clamshell enclosures

## Electrical Design Timeline

### September
* Assign existing projects and research based on interest and experience
* Decide on potential new projects
* Look into what parts and sensors are best for the job

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

### April-May
* Competition! 🎉🎉
* Season Wrap-up
* Make sure all documentation is posted to the GitHub
* Mentioned what worked well, what didn't, and what we can improve on for next year


## Andrew's List of Things to Do
* Fabricate more kill switch mounting plates
    * This includes both the rear square tab with two 1/8" rivet holes and the front tab that wraps around the switch body
* Design a new mounting bracket for the newer version of brake light
* Fix 2WD/4WD switch 9V/12V toggle that got bonked at comp
* Mail back X2 transponders for newer TR2 version
* Take inventory again
* Work on designing a better trailer layout
   * Install Toolgrid Organization System sponsor hardware
   * wall mounting things, laying out workbenches better, and organizing drawers/cabinets better
* Keep Electrical Bible updated based on 2024-2025 rulebook
* Reach out to RuggedRadios on or after 9/1/24 for 2025 sponsorship
