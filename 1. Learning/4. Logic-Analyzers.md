# What is a Logic Analyzer?

A logic analyzer is an instrument for capturing, displaying, and measuring multiple electronic signals simultaneously in a digital circuit. Logic analyzers are capable of showing the relationship and timing among many different signals in a digital system and are often capable of analyzing digital communication protocols, such as I2C, SPI, and Serial. As a result, a logic analyzer is the best tool for debugging digital circuits and digital communication systems. [(Saleae)](https://articles.saleae.com/logic-analyzers/what-is-a-logic-analyzer)

# HiLetgo USB Logic Analyzers

I purchased one of [these](https://www.amazon.com/HiLetgo-Analyzer-Ferrite-Channel-Arduino/dp/B077LSG5P2) logic analyzers for Baja use debugging logic signals. All variations of this are pretty similar, and Sparkfun sells their own version too. These are fairly affordable but more than capable of what we need them for.

To get started with one of these:

## Download [Zadig](https://zadig.akeo.ie/) for Windows

This is the application you need to install the following driver.

## Run Zadig for WinUSB

Plug in the logic analyzer, select it as a device, and install the WinUSB driver. You may have to run the driver installation twice if any issues come up. This installation may take several minutes, so be patient.

# Saleae [Logic 2](https://www.saleae.com/pages/downloads?srsltid=AfmBOor6FygTGAU4ubF86uryjJIEr9ODfYEBilPChjsBzgmbG-cqx6jO) Software

Saleae Logic Analyzers are powerful, and more notably, expensive logic analyzers. They use Saleae's [Logic 2](https://www.saleae.com/pages/downloads?srsltid=AfmBOor6FygTGAU4ubF86uryjJIEr9ODfYEBilPChjsBzgmbG-cqx6jO) software which allows you to see the data that is read by the analyzer. It is simple to set up and use, and more importantly, it has built in decoding feeatures. For example, it can identify a string of CAN bits and decode the packet into its respective data fields. Fortunately, this software also works with non-Saleae devicse like the HiLetgo Logic Analyzer. 

Once you have installed the drivers above, the Saleae software should recognize the logic analyzer as a device.

## Getting Started with Logic 2 and CAN decoding

After starting Logic 2, you should be able to immediately start viewing logic data. Note that these more affordable analyzers are not likely to support the highest data sample rate in Logic 2 (24MS/s), so try setting it to 16 MS/s or lower.

To view decoded CAN data, click the **Analyzers** tab on the right side (1F icon), and click the + icon. Select CAN and whichever channel you prefer to use. The bitrate we generally use for Baja is 500,000 or 500kbit/s. Other CAN systems may be different. Leave the **Inverted (CAN High)** box unchecked. It is unlikely you will be able to view the CAN HIGH signal, which goes between 2.5V and 3.5V. Logic analyzers will generally mark any signal above 2V as high. Nonetheless, Logic 2 will still be able to decode the data solely from the LOW signal.
