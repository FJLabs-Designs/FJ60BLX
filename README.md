# FJ60BLX Bluetooth 60% Mechanical Keyboard PCB

The following repository will hold the design files of the FJ60BLX Bluetooth Mechanical Keyboard PCB. This is designed to be a living repository and design files in this repository will be continually updated as the board iterates and changes.

## About this Repository

This repository contains rolling updates to the FJ60BLX Bluetooth PCB. Included are the base Eagle files (Board File, Schematic, and CAM Processor Job), the associated Gerber files for that revision, and the associated Bills of Materials. Each of these files will be segregated into their respective versions that are date-coded with the day of export. 

## Eagle Files

The core of this repository are the bare Eagle files. These files are the basis for the Gerber exports. **When using the eagle files, please remove the FJLabs and FJ60BLX branding.**

## Gerber Files

Included are the Gerber Files for manufacturing. These should be available in 5.6 format for all copper layers, and 4.5 format for all drills. Your PCB manufacturer requires these files to create the PCB itself. Additionally, included in the Gerber files are the relevant Pick and Place Coordinate/Centroid files which are needed for PCBA. 

## BOM Files

The included BOM files are available as Excel spreadsheets with LCSC links whereever possible. Certain components are not available from LCSC and must be purchased either directly from the manufacturer or from an authorized components distributor. 

## Renders

This folder includes a master list of all renders that have been sent to subscribers of the FJ60BLX mailing list and are date-coded. 

## Manufacturing Information

### Bluetooth Module

The PCB uses the MDBT40-256v3 Bluetooth module designed and manufactured by Raytac. This module must be programmed with the Adafruit Bluefruit SPI Friend firmware for compatibility with QMK. The relevant firmware has not been included as it is property of Adafruit and its respective company. However, this firmware is available for free open-source on GitHub (link not provided). Additionally, a SoftDevice file is required for programming of the bare Bluetooth module, which is included in the Adafruit repository for the Nordic 51822 chipset. 

Instructions are not included for programming the Bluetooth module over SWD, as it is more productive to purchase such modules pre-programmed directly from the manufacturer. The difference in cost between a programmed and unprogrammed module is negligble and therefore, for production, it is *highly recommended* to purchase preflashed chips. 