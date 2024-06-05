---
layout: post
title: Low-Cost and Open-Source Water Level Sensing
date: 2024-05-01 00:00:00 -0400
img: water_level.jpeg # Add image post (optional)
tags: [oceanography, sensor development] # add tag
categories: research
---

# Open Water Level Sensor

**Please visit [https://github.com/COAST-Lab/Open-Water-Level](https://github.com/COAST-Lab/Open-Water-Level) for the actively maintained Open Water Level sensor repository. The following information is copied from that repo.**

## 🔌 Introduction to the Sensor
This project aims to enable students, communities, businesses, and anyone else to monitor their local water level using a relatively low-cost and open-source sensor. To get started, read through this page and subsequent directions. 

![Water level sensor](../assets/img/for_posts/SMCKERR_WL_WL01.jpeg)

## ℹ️ About this Repository
The GitHub repository provides updated designs for a low-cost, open-source, cell-equipped water level sensor. The initial design, published in the journal Oceanography in the special section DIY (do-it-yourself) Oceanography, used a lower resolution sensor and had internal datalogging capabilities. The article, *A Low-Cost, DIY Ultrasonic Water Level Sensor for Education, Citizen Science, and Research*, can be found here: [https://doi.org/10.5670/oceanog.2023.101](https://doi.org/10.5670/oceanog.2023.101). The article corresponds to an older version of the code and hardware which can be found here: [https://github.com/SUPScientist/Seaport_Tide-SLR](https://github.com/SUPScientist/Seaport_Tide-SLR). That first version of the Open Water Level sensor used an Adalogger M0 microcontroller/datalogger and an ultrasonic sensor with 1" resolution. It had no real-time data communication feature.

If you are looking for a cellular data transmission-enabled device with higher resolution (1 cm) and solar power, this updated repository ([https://github.com/COAST-Lab/Open-Water-Level](https://github.com/COAST-Lab/Open-Water-Level)) has what you need. 

## 🌊 Deployment Considerations
Deployment is the last step but it's probably the most exciting, so we'll discuss this part next. The Open Water Level sensor has a ~ 6.5 m (21') range with a 1 cm (0.39") resolution. Deployment locations must be chosen with these values in mind. If you are deploying the monitor at a location reasonably close to an existing NOAA tide station, start by examining the known tidal range at your location: [NOAA tide predictions](https://tidesandcurrents.noaa.gov/tide_predictions.html). You will want to deploy the monitor at a location where it can aim straight down (normal) to the water's surface and at a height higher than the highest high tide or floodwater height that the location is expected to experience. You also want it to be low enough to capture the lowest low water. The package is water resistant, but not fully waterproof if submerged for extended periods.

## 📈 Live Data
The first two Open Water Level sensors were deployed on Smith Creek through a UNCW Cahill Grant with Drs. Monica Rother (EVS) and Andrea Hawkes (EOS) and with major installation and surveying support from Dave Wells. These stations (co-located with CTDs) are intended to monitor tidal excursions of saltwater into what had been freshwater ecosystems. We recently began a project with the City of Wilmington to deploy additional sensors on Burnt Mill Creek in an effort to improve resilience to flooding through more spatially dense flood alerts and community engagement. 

As we continue to build out our sensor network, we will be adding stations and their data here: 

<div class="resp-container">
    <iframe class="resp-iframe" src="https://wl.cormp.org/"></iframe>
</div>