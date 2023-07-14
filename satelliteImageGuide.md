# Satellite Image Guide
## Description
The purpose of this guide is to teach how to receive images from weather satellites for example the NOAA15-20 satellites. The guide is meant for use in education for example geography class. It will teach you how to find a satellite, get the coressponding raw data from it and decode this data into an actual image. This guide will use for accessebility a WebSDR, but the same could also be achieved by using a physical SDR you own, like the HackRF One or the RTL-SDR.

## Requirements
PC with Windows / MacOS / Linux
Internet connection to get the raw audio data from the satellite using a WebSDR.

## Basic structure
1. We will use the website www.n2yo.com to get the position of the satellite.
2. The satellite encodes the pictures in audio and sends it over a specific frequency. This audio can later be decoded into an image. To recive the audio we will use a WebSDR in our case from Nürnberg, Germany.
3. To decode the raw audio data into an image, we will use a software called noaa-apt.


## Prework
To decode the audio data we will later receive, we will use a software called noaa-apt, you can find the install instructions on the website (https://noaa-apt.mbernardi.com.ar/download.html). As of now, there are only precompiled binaries available for windows, so you may be required to compile the software yourself. You will find detailed instructions on the download site, please refer to them. We won't provide exact install instructions, as they might change over time.

If you have installed the software, we can proceed with the next section.

## 1. Finding the satellite



