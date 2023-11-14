---
title: Points
publishDate: 2023-11-01 00:00:00
img: /assets/30day/points.jpg
img_alt: IP Addresses of the world
description: |
  What would you do with access to 420,000 computers?
tags:
  - 30DayMapChallenge
  - Maps
  - Carna Botnet
---

Day 1: Points | #30DayMapChallenge

What would you do with access to 420,000 computers?  In 2012, a security researcher found that many users of the remote terminal application Telnet had never changed the default root:root login credentials.  The researcher coded up a botnet program that would scan internet IP addresses and attempt to log in to any computer with Telnet installed.  Once installed, the virus would replicate itself and use that computer to scan more IP addresses.  Within 16.5 hours, the researcher was in control of 420,000 hosts.

What did they do with this newfound power?  Instead of acting maliciously, the researcher decided to catalog the entire internet.  They found they could scan every IPv4 address in about 1 hour.  For 6 weeks, they scanned the whole internet again and again collecting data on which addresses and ports were live.  After 6 weeks, the researcher had each bot quietly delete itself.  

This story may not have gotten much attention if it weren’t for what came next:  the Internet Census 2012.  Graphs and tables are valuable tools, but what really made this data beautiful was a gif of the world showing the utilization of IP spaces across 24 hours.  I find this gif incredibly beautiful.  

[![Internet Census 2012 GIF](/assets/30day/IC2012.gif)](/assets/30day/IC2012.gif)

Since I don’t have access to 420,000 computers, for my first day of the 30DayMapChallenge, I chose to simply plot the density of IP network addresses.  I downloaded GeoLite2 city-level data for IPv4 and IPv6 addresses.  IP network address locations seem to be binned at the lat-long of the city centroid within this database, which proved challenging to plot.  I first attempted to aggregate network counts by geographic centroid, but the tight packing of centroids in some areas and the sparseness in others yielded a map I wasn’t pleased with.  Instead, I created a .15x.15 degree grid across the globe and aggregated the count of IP network addresses within each grid cell.  The points for the final map were then placed at the centroid of each grid cell.
Drop me a line if you have any questions on my process or want to chat more!

Story source:  [https://darknetdiaries.com/episode/13/]( https://darknetdiaries.com/episode/13/)  
Huge thank you to Jack Rhysider for this story and putting so much into this great podcast!

Internet Census 2012:  [https://census2012.sourceforge.net/paper.html]( https://census2012.sourceforge.net/paper.html)

30DayMapChallenge:  [https://30daymapchallenge.com/](https://30daymapchallenge.com/)
