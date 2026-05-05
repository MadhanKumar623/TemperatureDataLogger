# Temperature Data Logger - Wokwi Project

A Wokwi-based embedded temperature data logger project that reads temperature through ADC, gets real-time date/time from an RTC module, displays data on an LCD, prints logs through UART/Serial Monitor, and stores timestamped temperature data into an SD card.

## Project Link

https://wokwi.com/projects/390701463449896961

## Features

- Reads analog temperature input using ADC
- Converts ADC value into Celsius
- Gets current date and time from RTC
- Displays time and temperature on LCD
- Prints timestamped data through UART/Serial Monitor
- Stores temperature logs into SD card
- Uses modular files for ADC, I2C, RTC, LCD, UART, and SD card handling

## Main Modules

- `sketch.ino` - Main application flow
- `adc.h / adc.ino` - ADC initialization and analog reading
- `i2c.h / i2c.ino` - I2C communication layer
- `rtc.h / rtc.ino` - RTC date and time handling
- `lcd.h / lcd.ino` - LCD initialization and display functions
- `uart.h / uart.ino` - UART/Serial Monitor output
- `sdcard.h / sdcard.ino` - SD card write/read functions
- `diagram.json` - Wokwi circuit connections

## Working Flow

1. Initialize I2C, LCD, ADC, RTC, UART, and SD card.
2. Read the current date and time from RTC.
3. Display time on the LCD.
4. Print time through Serial Monitor.
5. Read analog temperature input.
6. Convert the ADC value into Celsius.
7. Display temperature on the LCD.
8. Store timestamped temperature data into the SD card periodically.

## How to Run

1. Open the Wokwi project link.
2. Start the simulation.
3. Observe date, time, and temperature on the LCD.
4. Check Serial Monitor for UART output.
5. Use the SD card file output to verify logged data.

## Purpose

This project demonstrates a complete embedded data-logging workflow using ADC, RTC, LCD, UART, I2C, and SD card interfacing in a simulated environment using Register Level Bare Metal Programming.
