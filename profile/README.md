# NJIT-Highlander-Racing-Electrical 

## A GitHub Organization for NJIT's Highlander Racing Electrical Subteam

This organization contains individual repositories for each subsystem on the car, including:
* Dashboard
* CVT Tachometer
* Gas/Brake Pedal Sensors
* Fuel Level Sensor
* Data Acquisition System
* PC Base Station
* Wheel Speed/Suspension Travel
* Power Systems
* Enclosures
* CAN-Bus



## Important Links

[2026 Baja SAE Rules](https://www.bajasae.net/cdsweb/gen/DownloadDocument.aspx?DocumentID=cd82c643-bb41-4c95-8cca-cbb19d8f2d95)

[Electrical Folder in Google Drive](https://drive.google.com/drive/folders/1Pz5bq8r8b9oh7MFo3oWOcobUKbDVZDIy?usp=drive_link)

[Electrical Inventory](https://docs.google.com/spreadsheets/d/19zXsWbHnRgKuqglurabbrF1yi5oSlVw6kvXuMUWI1O0/edit?usp=drive_link)

[Electrical Photos/Videos](https://drive.google.com/drive/folders/1SR_HuOiAXgWjmbBMsi99OzsaskyCo2m3)

[NJIT Baja KiCad Library](https://github.com/NJIT-Highlander-Racing-Electrical/.github/tree/main/2.%20NJIT-Baja-KiCad-Library)

[Learning Resources](https://github.com/NJIT-Highlander-Racing-Electrical/.github/tree/main/1.%20Learning)

## 2025-2026 Design Goals
* Complete KiCad library for commonly used hardware - CAN transceievers, USB-C ESP32 boards, pads for aviation plugs, etc
    * Includes symbols, footprints, and 3D models
* Move towards SMD boards
     * Custom CAN transceiver footprints for use on boards
     * Integrate 2024-2025 voltage regulator board on each subsystem's PCB
         * Components can be larger for easier soldering
* Full PlatformIO/GitHub workflow integration
* All data outputs from subsystems are shared with each other via CAN-Bus
* Any data on the CAN-Bus is saved to a dedicated DAQ logger
* Strong design process documentation (photos, schematics, research, etc)

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
* Use female headers on PCB to test designs
   * If they work, solder the components directly to another PCB
   * If they don't, troubleshoot the PCBs to see what needs to change for v2

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


## 2025-2026 Design Goals 
* Complete KiCad library for commonly used hardware - CAN transceievers, USB-C ESP32 boards, pads for aviation plugs, etc
    * Includes symbols, footprints, and 3D models
* Move towards SMD boards
     * Custom CAN transceiver footprints for use on boards
     * Integrate 2024-2025 voltage regulator board on each subsystem's PCB
         * Components can be larger for easier soldering
* Smaller shock sensors that just mount between chassis and upper control arm
* Live video feed
* Go Pro continuous USB-C power source
