---
marp: true
math: mathjax
class: invert
---

<!-- headingDivider: 1 -->

# Passpredict

## How to see a satellite in your backyard


# What is passpredict?

- A Python library to compute satellite overpass predictions for a point on Earth.
- Includes a command line interface for quick predictions from your terminal.
- Open source, MIT licensed.
- Developed by me, with inspiration from other open source astrodynamic toolkits, such as Skyfield, Poliastro, Orbit-Predictor, and Gpredict.

Available now on PyPI with `pip install passpredict`


# Who am I?

Hello! I'm Sam Friedman.

- Final year PhD student at Texas A\&M researching uncertainty quantification in coupled, multidisciplinary systems.
- Primary coding background in scientific computing, but have branched out to general software development.
- Just started as software engineer at HawkEye 360 working on their space software team.


# Why would someone want to compute when a satellite overpass will occur?

- For **fun**: go outside and see a satellite with your naked eye. You can even see the International Space Station in bright cities.
- For **hobbyists**: download raw image data from NOAA weather satellites (DIY Google Maps!); bounce HAM radio signals off of satellites to communicate with people around the world; take a picture of the ISS!
- For **engineers**: know when your satellites are in line-of-sight of your groundstation antennas for downloading/uploading data.
- For **astronomers**: plan your astronomical observing times to minimize the impact of satellite trails on your data collection (more on this later)


# This is a challenging problem

- The equations and methods are well known, but it requires enough domain knowledge that developing the software is difficult.
- There are existing Python libraries and projects, but they aren't easily extensible to create a general purpose prediction interface.

But with enough textbooks we can figure it out.

So passpredict was born in 2019 to fill the need for a generalized approach to the satellite prediction problem.


# Satellite Pass Predictions: An Overview

## Inputs

- satellite orbit data: position and velocity of satellite at a specific time (the *epoch*)
- location coordinates: latitude, longitude, elevation of the observer
- time span: time interval to search for passes, $t_0$ to $t_f$

## Outputs

-



