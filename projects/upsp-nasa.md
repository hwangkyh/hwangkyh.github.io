---
layout: project
type: project
image: images/upsp-model.jpg
title: Data Analysis for Unsteady Pressure Sensitive Paint (uPSP)
permalink: projects/upsp-nasa
# All dates must be YYYY-MM-DD format!
date: 2021-08-13
labels:
  - Python
  - Linux
summary: Analyzed and processed data for unsteady pressure sensitive paint (uPSP) project at Ames Research Center, NASA.
---

<div class="ui medium rounded images">
  <img class="ui image" src="../images/usps-kulite.jpg">
  <img class="ui image" src="..images/upsp-model.jpg">
</div>

The current 5-year unsteady pressure sensitive paint (uPSP) development project is looking at developing this wind tunnel pressure measurement technology to reach production capacity. The applications of uPSP is in the launching of vehicles to mitigate vehicles shaking themselves apart due to the sound produced. Another method of measuring pressure is through the kulite microphones and so the cross correlation between uPSP and kulites covering the vehicle model in the wind tunnel will inform the project about the validity of the uPSP data. There is so much data that has been produced already from both uPSP and kulites, up to 200GB of raw data produced from 10 second data points. The research is in two parts: the first is looking at the kulite to uPSP comparison from the SLS test using .slow files from run 3014, and the second is looking at the harmonics results from .fast files from run 3091. Scripts using Python were produced to conduct this research and create PSDs by Fourier transform. 

Through this summer internship at ARC, NASA, I have successfully created a Python script that takes in .info and .slow or .fast kulite data and produces PSDs for set kulite sequences of runs 3014 (.slow) and 3091 (.fast) depending on mach number. Did cross correlation between kulites, showing time lag and decay the further downstream the kulite is.
