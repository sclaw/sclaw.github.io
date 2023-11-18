---
title: Atmosphere
publishDate: 2023-11-18 00:00:00
img: /assets/30day/atmosphere.jpg
img_alt: Washington DC Heat Islands
description: |
  
tags:
  - 30DayMapChallenge
  - Maps
  - Geostatistics
---

Day 18: Atmosphere | #30DayMapChallenge

For those of you who don't know DC, Northwest DC has historically been more affluent than Northeast DC.  You see that as you drive around, but I've always been struck by how you can even see it from space.  Those tree-lined suburban streets in the northwest quadrant stand out against the paved streets of the Northeast.  

A fellow graduate student turned me on to this dataset last year, and it turns out that change in land cover has implications beyond aesthetics.  By measuring temperature transects, this group from Portland State University showed the stark differences that land cover has on afternoon air temperature.  Heat exposure has significant impacts on public health, and these impacts will only be exacerbated by warming global temperatures.  As the climate crisis worsens, we have a lot of work to do assisting those facing the brunt of the impacts.

I was always a little skeptical of this dataset. They used a machine learning model to predict afternoon temperature based on satellite land use. It seemed to me that, DUH, temperature would be correlated to land use when you're using land use to predict it. So I took their raw data points and did a simple kriging analysis, which is shown in the bottom left. The land-use correlation stood out even when the model was blind to land-use (phew). I dug into their paper some more and saw that they actually didn't use any intermediate land-use classification for their temperature prediction, but instead built the predictors using focal buffers on raw sentinel-2 bands. I really like that approach, and have seen similar things popping up across the hydrologic literature as well. That Shandas team has put together some great data products, and I'm glad they stand up under my (modest) scrutiny.


Citation for data:
Shandas V, Voelkel J, Williams J, Hoffman J. Integrating Satellite and Ground Measurements for Predicting Locations of Extreme Urban Heat. Climate. 2019; 7(1):5. https://doi.org/10.3390/cli7010005

Data accessed at:  [https://osf.io/eb4tw/](https://osf.io/eb4tw/)


30DayMapChallenge:  [https://30daymapchallenge.com/](https://30daymapchallenge.com/)
