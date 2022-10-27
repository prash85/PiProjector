<h1 align="center"> Pi-Projector </h1> <br>

<p align="center">
  <img src = "/github_assets/images/00.PNG" width=700>
</p>

## Table of Contents
- [Introduction](#introduction)
- [BOM](#bom)
- [Notes](#notes)
- [Images](#images)

## Introduction

<p>
A few years back Texas Instruments release an experimental DLP Projector Module which became quite popular in the hobbyist community as some community members managed to get this working with Raspberry Pi Board. This project is an attempt to create my own version of PCB to interface this projector module with Raspberry Pi 3A. 
</p>

<p align="center">
  <img src = "/github_assets/images/github_assets/images/1_DLP2000EVM.jpg" width=500>
</p>

## BOM

* Raspberry Pi 3A - 1
* DC-DC Buck Converter 7-24V to 5V 4A - 1
* Beaglebone 46 Pin stacking headers - 2
* 20 Pin female header for Raspberry Pii - 1
* 12VDC Adapter - 1
* Dupont connectors for 5V  - 1
* And last but not the least - **Pi Projector PCB**

## Notes
- Assemble Raspberry Pi , DLP2000EVM Module and Pi Projector PCB as shown in the main image.

<p align="center">
  <img src = "/github_assets/images/github_assets/images/0_FullASM.jpg" width=500>
</p>

- Configure Raspberry Pi as <a href="https://www.youtube.com/watch?v=XFciR-U7yhc&t=1s">MickMake Pi Projector</a>. 
- Note that for me the I2C bus addresses were found to be as below:

<p> <code> i2cset -y 2 0x3b 0x0c 0x00 0x00 0x00 0x13 i </code> Set Resolution </p>
<p> <code> i2cset -y 2 0x3b 0x0b 0x00 0x00 0x00 0x00 i </code> Set parallel Interface </p>

- After updating the configuration, reboot the Pi to start seeing desktop on Projection wall. 

## Images

### Final PCBs

<p align="center">
  <img src = "/github_assets/images/github_assets/images/2_TOP.jpg" width=500>
</p>

<p align="center">
  <img src = "/github_assets/images/github_assets/images/3_Bottom.jpg" width=500>
</p>

### Random

<p align="center">
  <img src = "/github_assets/images/github_assets/images/4.jpg" width=500>
</p>

<p align="center">
  <img src = "/github_assets/images/github_assets/images/5.jpg" width=500>
</p>

<p align="center">
  <img src = "/github_assets/images/github_assets/images/6.jpg" width=500>
</p>

<p align="center">
  <img src = "/github_assets/images/github_assets/images/7.jpg" width=500>
</p>

<p align="center">
  <img src = "/github_assets/images/github_assets/images/8.jpg" width=500>
</p>