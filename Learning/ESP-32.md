# Programming an ESP32 Microcontroller

## 1. Add ESP32 Board Link

* In the Arduino IDE, go to File -> Preferences

* In the box next to "Additional boards manager URLs," paste the following:

`https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json`

* Then, press OK.

## 2. Add ESP32 to Arduino IDE Board Manager

* On the left side of the IDE, click the second icon (Boards Manager)

* Search for "ESP32" in the filter bar

* Install "esp32" by Espressif Systems. This may take a few minutes

## 3. Install USB Drivers

* Click [this link](https://www.silabs.com/documents/public/software/CP210x_VCP_Windows.zip) to download the required drivers for ESP32 boards from Silicon Labs

* Right click the downloaded folder and extract the files from the ZIP

* Open the folder and run the *CP210xVCPInstaller_x64* application

## 4. Select Your Board

* At the top of the IDE, click the "Select Board" field

* If you currently have a board connected, you may see a COM port, and you can click this. If not, click "Select other board and port"

* Now, you are able to search for your specific board model. In most cases, we will be using "ESP32 Dev Module." This is a general driver that works with many commonly sold ESP32 boards
   * Also note, some boards that look like [this](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.instructables.com%2FESP32-Internal-Details-and-Pinout%2F&psig=AOvVaw0eAobmugqPfx9SuD1qVDpw&ust=1727239334852000&source=images&cd=vfe&opi=89978449&ved=0CBQQjRxqFwoTCKCJ04ni2ogDFQAAAAAdAAAAABAd) may be compatible with the "Node32s" board profile, which allows for uploading without needing to fiddle with the EN/BOOT buttons
 
