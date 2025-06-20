---
layout: post
title: Low-Cost and Open-Source Water Level Sensing
date: 2025-01-01 00:00:00 -0400
img: waterLevel_new.jpeg # Add image post (optional)
tags: [oceanography, sensor development] # add tag
categories: research
---

# Open Water Level Sensor

**Please visit [https://github.com/COAST-Lab/Open-Water-Level](https://github.com/COAST-Lab/Open-Water-Level) for the actively maintained Open Water Level sensor repository. The following information is copied from that repo.**

## ℹ️ About this Repository
This GitHub repository provides updated designs for a low-cost, open-source, cell-equipped water level sensor. The initial design, published in the journal Oceanography in the special section DIY (do-it-yourself) Oceanography, used a lower resolution sensor and had internal datalogging capabilities. In this repo, we describe how to use a higher-resolution sensor with a cellular modem for near-real-time water level information. 

The article, *A Low-Cost, DIY Ultrasonic Water Level Sensor for Education, Citizen Science, and Research*, can be found here: [https://doi.org/10.5670/oceanog.2023.101](https://doi.org/10.5670/oceanog.2023.101). The article corresponds to an older version of the code which can be found here: [https://github.com/SUPScientist/Seaport_Tide-SLR](https://github.com/SUPScientist/Seaport_Tide-SLR).  
[![DOI](https://zenodo.org/badge/688666593.svg)](https://doi.org/10.5281/zenodo.13991877) --> GitHub release.

Please read the following for a high-level overview of the project and the contents of this repository.

## 🔮 Table of Contents 
Scroll down or click the following links for more information: 
- [Introduction to the Sensor](#-introduction-to-the-sensor)
- [How to Build a Sensor](#-how-to-build-a-sensor)
- [Firmware and getting started guide](https://github.com/COAST-Lab/Open-Water-Level/tree/main/Firmware)
- [Deployment Considerations](#-deployment-considerations)
- [Live Data Portal](#-live-data)

![Water level sensor](../assets/img/for_posts/SMCKERR_WL_WL01.jpeg)

## 🔌 Introduction to the Sensor
There are several versions of the DIY water level sensor. They include different microcontrollers (e.g., an Arduino-based Feather Adalogger with internal logging capabilities and a Particle Boron with cellular communication capabilities) and sensor interfacing options (analog, serial, and pulse-width modulation). 

If you are looking for a cellular data transmission-enabled device with higher resolution, this repository has what you need. To get started on soldering and building your sensor package, click here [Firmware](Firmware). If you are looking for the original, less expensive Arduino version with internal datalogging capabilities, see [https://github.com/SUPScientist/Seaport_Tide-SLR](https://github.com/SUPScientist/Seaport_Tide-SLR).

The device designs in this repository comprise a low-cost open-sourced sensor package designed to measure distance and transmit and store measurements.  It utilizes a Particle Boron with cellular data transfer, an Adafruit Adalogger Featherwing for local data storage, a Maxbotix ultrasonic rangefinder, a rechargeable lithium-ion battery, and a water-resistant enclosure. 

This repository aims to enable students, communities, businesses, and anyone else to monitor their local water level. To get started, read through this page and subsequent directions. 

## 🔨 How to Build a Sensor
We currently have two effective enclosure designs for the DIY sensor, one using a PVC pipe and the other using a Polycase housing. Visit the GitHub repo to find links to BOMs, enclosure designs, and datasheets for each model: [https://github.com/COAST-Lab/Open-Water-Level](https://github.com/COAST-Lab/Open-Water-Level).

## 🌊 Deployment Considerations
Deployment is the last step but it's probably the most exciting, so we'll start our procedural notes here. The Open Water Level sensor has a ~ 6.5 m (21') range with a 1 cm (0.39") resolution. Deployment locations must be chosen with these values in mind. If you are deploying the monitor at a location reasonably close to an existing NOAA tide station, start by examining the known tidal range at your location: [NOAA tide predictions](https://tidesandcurrents.noaa.gov/tide_predictions.html). You will want to deploy the monitor at a location where it can aim straight down (normal) to the water's surface and at a height slightly higher than the highest high tide or floodwater height that the location is expected to experience. You also want it to be low enough to capture the lowest low water. The package is water resistant, but not fully waterproof if submerged for extended periods.

## 📈 Live Data
The first two Open Water Level sensors were deployed on Smith Creek through a UNCW Cahill Grant with Drs. Monica Rother (EVS) and Andrea Hawkes (EOS) and with major installation and surveying support from Dave Wells. These stations (co-located with CTDs) are intended to monitor tidal excursions of saltwater into what had been freshwater ecosystems. We recently began a project with the City of Wilmington to deploy additional sensors on Burnt Mill Creek in an effort to improve resilience to flooding through more spatially dense flood alerts and community engagement. 

As we continue to build out our sensor network, we will be adding stations and their data here: 

<div class="resp-container">
    <iframe class="resp-iframe" src="https://wl.cormp.org/"></iframe>
</div>