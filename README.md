# Air Quality Wing Hardware

![Render](images/render.png)

## What is it?

The Air Quality Wing (Previously Particle Squared), designed by [Jared Wolff](https://www.jaredwolff.com), is an all-in-one air quality sensor for Particle and Feather based development boards. It brings together a trio of sensors to give you as many data points as possible. That way, there won’t be anything missing when you go to measure the air inside your home or workplace.

Here’s what’s on board:

### Particulate Sensing

The Air Quality Wing also has support for the **[Honeywell HPMA115S0 dust sensor](https://sensing.honeywell.com/honeywell-sensing-hpm-series-particle-sensors-datasheet-32322550-e-en.pdf)**. This sensor counts the concentration of potentially harmful particulates in the air. Plus, it does it all using ***lasers.***

It can detect both large particles 10µm in diameter and smaller ones less than 2.5µm in diameter. These are the same readings that are commonly known as PM10 and PM2.5.

### Sensing Volatile Compounds

Second to that, is the **[AMS CCS811](https://ams.com/ccs811)**. This senses volatile organic compounds and eC02. These types of readings are useful in places where there may be combustion. (Think stoves, furnaces, etc) It can act as an early warning mechanism. That way you stay safe, happy and healthy!

### Temperature and Humidity

Finally, the **[Silicon Labs Si7021](https://www.silabs.com/documents/public/data-sheets/Si7021-A20.pdf)** temperature and humidity sensor. These readings can be used on their own. Additionally they’re used by the CCS811 to compute an accurate TVOC and C02.

### Flexible Power Sources

No outlet nearby where you want to measure? No problem!

You can easily plug in almost any lithium polymer battery to your Particle or Feather based board and use it immediately. The Air Quality Wing has extra circuitry that allow you to use either USB or battery power. How great is that?

[To get yours go here.](https://www.jaredwolff.com/store/particle-squared/)

## Library/Code

Here are the links for the [example code](http://github.com/jaredwolff/air-quality-wing-code) and Particle [Library](http://github.com/jaredwolff/air-quality-wing-library).

## Changelog

### Revision 3

- Fixed bug related supply voltage not being stable to the HPMTA115S0
- Relocated D7 to D5 for CCS811 reset signal

### Revision 2

- Added ferrite for noise immunity
- Swapped out MCP1624 with MCP1640

## License

The license for these files is: [Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/). See included `LICENSE` file for all the legal stuff.
