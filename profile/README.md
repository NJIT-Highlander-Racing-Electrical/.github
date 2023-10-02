# NJIT-Highlander-Racing-Electrical 

A GitHub Organization for NJIT's Highlander Racing Electrical Subteam

This organization contains individual repositories for each subsystem on the car, including:
* Dashboard
* Semi-Active Suspension
* CVT Tachometer/Temperature Sensor
* Driver's Seat Pressure Sensors
* Gas/Brake/Steering Angle Sensors
* Fuel Level Sensor
* Dedicated Data Acquisition Logger
* GPS Data
* 2WD/4WD Engagement Switch
* Power Research

## Important Links

2024 Baja SAE Rules (Rev A, 8/31/23)
https://www.bajasae.net/cdsweb/gen/DownloadDocument.aspx?DocumentID=024d6763-9fb8-45c5-b87c-08351214cede

Eletrical Inventory Spreadsheet
https://docs.google.com/spreadsheets/d/1Qi0S1_aLF-bAy1xNMarseqDGTy3XCX9PLI8lnr3L_F0/edit?usp=sharing

## 2023 Design Goals 
* Custom PCBs for subsystems where applicable
* Custom durable and compact 3D printed enclosures for subsystems
* All data outputs from subsystems are shared with each other via CAN-Bus
* Any data on the CAN-Bus is saved to a dedicated DAQ logger
* Single battery that powers all subsystems
* Universal power and data connections/cables throughout the vehicle
* Strong design process documentation (photos, schematics, research, etc)

## CAN-Bus Message ID Hierarchy

With CAN-Bus, data is constantly being sent to and from all devices in the loop. While not every device is set to receive every message, it is important that there is a hierarchy to the messages. This way, more crucial data is sent first. Our Message ID hierarchy can be found in this repository.
