# What is a Logic Analyzer?

A logic analyzer is an instrument for capturing, displaying, and measuring multiple electronic signals simultaneously in a digital circuit. Logic analyzers are capable of showing the relationship and timing among many different signals in a digital system and are often capable of analyzing digital communication protocols, such as I2C, SPI, and Serial. As a result, a logic analyzer is the best tool for debugging digital circuits and digital communication systems. [(Saleae)](https://articles.saleae.com/logic-analyzers/what-is-a-logic-analyzer)

# HiLetgo USB Logic Analyzers

I purchased one of [these](https://www.amazon.com/HiLetgo-Analyzer-Ferrite-Channel-Arduino/dp/B077LSG5P2) logic analyzers for Baja use debugging logic signals. All variations of this are pretty similar, and Sparkfun sells their own version too. These are fairly affordable but more than capable of what we need them for.

To get started with one of these:

## Download [Zadig](https://zadig.akeo.ie/) for Windows

This is the application you need to install the following driver

## Run Zadig for WinUSB

Plug in the logic analyzer, select it as a device, and install the WinUSB driver. You may have to run the driver installation twice if any issues come up.

# Saleae Logic Software

Saleae Logic Analyzers are powerful, and more notably, expensive logic analyzers. They use Saleae's Logic 2 software which allows you to see the data that is read by the analyzer. It is simple to set up and use, and more importantly, it has built in decoding feeatures. For example, it can identify a string of CAN bits and decode the packet into its respective data fields. Fortunately, this software also works with non-Saleae devicse like the HiLetgo Logic Analyzer. 

Once you have installed the drivers above, Saleae should recognize the logic analyzer as a device.

## Getting Started with CAN decoding

In Logic 2,
