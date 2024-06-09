---
title: Raster
publishDate: 2023-11-21 00:00:00
visPriority: 28
img: /assets/30day/raster.mp4
img_alt: UVM Natural Areas
description: |
  
tags:
  - 30DayMapChallenge
  - Maps
  - Vermont
---

Day 21: Raster | #30DayMapChallenge

This is a recreation of the the Great Vermont Flood that devastated Montpelier, VT this past July.  I made this recreation using stage hydrograph data from the USGS, photos from the University of Vermont Spatial Analysis Lab (for calibration), and a detrended elevation raster that I created.  The raster detrending technique I used is a Height Above Nearest Drainage (HAND) raster, which converts the raw elevation at each point in the terrain into a height above the nearest river.  With that raster in hand, we can project the measured USGS river stages into inundation extents (with some calibration from the event photos).  

While this recreation did not use a model, there's a lot of cool work being done with low-complexity hydraulic models that are based on HAND.  Check out the probHAND paper (from Diehl et al. 2021) below as well as the dataset of floodplain maps for the Lake Champlain Basin of Vermont that we created using the model (hosted on VCGI).

30DayMapChallenge:  [https://30daymapchallenge.com/](https://30daymapchallenge.com/)

UVM Natural Areas:  [https://www.uvm.edu/environmentalprogram/uvm-natural-areas](https://www.uvm.edu/environmentalprogram/uvm-natural-areas)

VCGI LULC: [https://geodata.vermont.gov/pages/land-cover](https://geodata.vermont.gov/pages/land-cover)