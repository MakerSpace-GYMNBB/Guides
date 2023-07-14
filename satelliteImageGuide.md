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
To find a satellite, which is near us, we will use the www.n2yo.com site. It allows, you to see the exact location of many satellites and predict their orbit. We will only focus on the Noaa 15, 18, 19 satellites. To find a satellite, for example noaa 15, tap onto the search bar in the top right corner of the screen. You may then type the name of the satellite into the search bar, for example "noaa 15", you should be then redirected to the site of the satellite. Please note, that you need to enter the noaa names with the space, so in the following format, "noaa <number>".

If you got redirexted to the site, you should be able to see something like this.

<img width="880" alt="satInfoScreen" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/a8ecdd22-46cc-4093-b254-c43b325d4808">

1. Orbit of the satellite
2. Satellite
3. Next time the satellite will be passing over your location

You can navigate on the map like on google maps, use your scroll wheel to zoom out or the minus and plus buttons.
Your location should be marked by a red dot on the map.

Now that you know how to use the website, just search for one of the satellites and listen to them when they are near you. To be later able to listen to the satellite, note down the frequency it is sending on, you can get it from this list:

Noaa 15: 137.620MHz
Noaa 18: 137.9125 MHz
Noaa 19: 137.10 MHz


## 2. Listening to the satellites
You will be using a WebSDR, in this case the one from Nürnberg. A WebSDR is like a real radio but you can access the radio through the internet. For the Nürnberg WebSDR go to: http://nbgsdr.ddns.net
You should be presented with the followning after maybe scrolling a bit down.


<img width="880" alt="Bildschirmfoto 2023-07-14 um 10 51 25" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/85402302-cca9-4b06-b8a1-e29e1561584b">


1. Here you can enter your frequency, you want to receive on.
2. Here you can select the Band

Enter the frequency of the satellite you want to listen to or click on sat!

<img width="1025" alt="Bildschirmfoto 2023-07-14 um 11 01 02" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/366a5092-e1c8-413e-956a-aab44559dd7f">

1. Bookmark of satellites, which you can click on and the frequency gets changed to corresponding bookmark.












