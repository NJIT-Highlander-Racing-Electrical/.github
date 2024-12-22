# Getting Started with Arduino IDE

## 1. Download the Editor 

Downloading the Arduino IDE 2 is done through the [Arduino Software page](https://www.arduino.cc/en/software).
If using a Windows Computer, choose the Download Option for "Win 10 and newer, 64 bits".

## 2. Run the Installer
All of the default settings are sufficient, and this should only take a few miuntes.

## 3. Device Software Prompts
You may be prompted to install some device software and drivers from Adafruit Industries or Arduino after opening the Arduino IDE. These drivers are essential to communicating with connnected microcontrollers, so make sure you install them. 

## 4. (Optional) Dark Mode
You can set the IDE to dark mode via File -> Preferenecs -> Theme

## 5. Arduino IDE Features

### Board Select

Before uploading your code, you must select what type of board you are using. For most of our projects, we will be using ESP32 microcontrollers, but this requires some additional setup as described in [2. Programming an ESP32 Microcontroller.](https://github.com/NJIT-Highlander-Racing-Electrical/Learning/blob/main/ESP-32.md)

### Serial Monitor

The Serial Monitor in Arduino IDE is a tool that allows you to send and receive data between your computer and the Arduino board over a USB connection. It displays text output from the board, such as sensor readings or debugging information, and enables you to send input, like commands or parameters, back to the board. This is useful for monitoring real-time data and troubleshooting your code.

### Serial Plotter

The Serial Plotter in Arduino IDE visualizes real-time data from your Arduino board by graphing it. It plots values sent via the Serial.println() function on a graph, making it easier to observe trends, patterns, and changes in sensor readings or other data over time. It's a useful tool for understanding how data behaves dynamically in your projects.

### Debugger

The debugger in Arduino IDE allows you to step through your code line-by-line and check the value of variables throughout the program. It helps identify logical errors or bugs by letting you pause execution at specific points, set breakpoints, and observe the behavior of your code as it runs. This tool is  useful for understanding why a program isn’t working as expected, for instance if a variable is not being set to the right value. This is an alternative to using print messages to the Serial Monitor.

### Library Manager

The Library Manager allows you to install, update, and manage libraries that add new capabilities to your projects. Libraries are sets of pre-written code that make complicated tasks, like working with displays or complex sensors, easier. With the Library Manager, you can search for your sensor or component and find the library that it uses. For something like a display, this will give you all kinds of premade functions to easily display data and text in a variety of fonts and colors. 


## Additional Resources

### Arduino Tutorials

If you are looking to learn more about programming, hardware, and the Arduino IDE, Paul McWhorter has dozens of introductory videos that take you step by step through the Arduino process. His Arduino Tutorials playlist can be found [here](https://www.youtube.com/watch?v=fJWR7dBuc18&list=PLGs0VKk2DiYw-L-RibttcvK-WBZm8WLEP&ab_channel=PaulMcWhorter).

### Arduino Language Reference

There is also the [Arduino Language Reference](https://www.arduino.cc/reference/en/). This has every built-in/standard function, variable, and program structure explained with examples.

### Electronics Distributors

[Adafruit](https://www.adafruit.com/) and [Sparkfun](https://www.sparkfun.com/) are also excellent resources for hobbyists. They sell electronics components that nearly always come with detailed descriptions, datasheets, and programming examples to help get you started.  
