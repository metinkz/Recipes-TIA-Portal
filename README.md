# Food Production Automation with Recipe Management

A food production automation project developed in **Siemens TIA Portal** as part of a PLC course to learn **recipe management** using WinCC.
The system demonstrates how predefined recipes can be used to control desired temperature values for multiple tanks via an HMI.

## System Overview
- Two-tank temperature control system
- Each tank has an individual heater and temperature feedback
- Desired temperatures are set automatically using selected recipes
- System operation is controlled and monitored via HMI

## Recipe Management
- Recipes are created using WinCC recipe functionality
- Each recipe contains:
  - Desired temperature for Tank 1
  - Desired temperature for Tank 2
- Recipes represent different products (e.g. Chocolate, Biscuit)
- Selected recipe values are written directly to PLC tags

## Control Logic
- Tank temperatures are read from simulated PT100 analog inputs
- Raw values are converted and scaled to engineering units
- Heaters are switched ON/OFF based on comparison between:
  - Current temperature
  - Recipe-defined desired temperature
- Tank control logic is identical for both tanks

## HMI Features
- Recipe selection via dropdown list
- Display of current tank temperatures
- Input and display of desired temperatures from recipes
- Start/Stop control for the heating process

## Tools
- Siemens TIA Portal
- Siemens WinCC Advanced

## What I Learned
- Creating and managing recipes in WinCC
- Linking recipe values to PLC control logic
- Using data records for product-based automation
