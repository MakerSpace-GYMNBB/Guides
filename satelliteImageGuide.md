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
To find a satellite, which is near us, we will use the www.n2yo.com site. It allows, you to see the exact location of many satellites and predict their orbit. We will only focus on the Noaa 15, 18, 19 satellites. To find a satellite, for example noaa 15, tap onto the search bar in the top right corner of the screen. You may then type the name of the satellite into the search bar, for example "noaa 15", you should be then redirected to the site of the satellite. Please note, that you need to enter the noaa names with the space, so in the following format, "noaa NUMBER".

If you got redirected to the site, you should be able to see something like this.

<img width="880" alt="satInfoScreen" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/a8ecdd22-46cc-4093-b254-c43b325d4808">

1. Orbit of the satellite
2. Satellite
3. Next time the satellite will be passing over your location

You can navigate on the map like on google maps, use your scroll wheel to zoom out or the minus and plus buttons.
Your location should be marked by a red dot on the map.

Now that you know how to use the website, just search for one of the satellites and listen to them when they are near you. To be later able to listen to the satellite, note down the frequency it is sending on, which you can get from this list:

Noaa 15: 137.620MHz

Noaa 18: 137.9125 MHz

Noaa 19: 137.10 MHz


## 2. Listening to the satellites
You will be using a WebSDR, in this case the one from Nürnberg. A WebSDR is like a real radio but you can access the radio through the internet. For the Nürnberg WebSDR go to: http://nbgsdr.ddns.net
You should be presented with the followning after maybe scrolling a bit down.


<img width="880" alt="Bildschirmfoto 2023-07-14 um 10 51 25" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/85402302-cca9-4b06-b8a1-e29e1561584b">

1. Here you can enter your frequency, you want to listen on.
   
2. Here you can select the Band

Enter the frequency of the satellite you want to listen to or click on SAT!

---

<img width="1025" alt="Bildschirmfoto 2023-07-14 um 11 01 02" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/366a5092-e1c8-413e-956a-aab44559dd7f">

1. Bookmark of satellites, which you can click on and the frequency gets changed to the bookmarked one.

---
   
<img width="1080" alt="Bildschirmfoto 2023-07-14 um 09 53 07" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/12275eb2-6617-4907-bff7-92c001912e04">
1. Typical signal for picture transmission of noaa satellites

If you got a signal like in 1, scroll down and proceed.

---

<img width="823" alt="Bildschirmfoto 2023-07-14 um 14 40 27" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/c6f0dff2-f053-4ee4-9b88-dc6d3b72a3e3">

1. Start audio recording
   
If you are not already here, scroll down on the site. We will record the audio from the satellite, by pressing the "start" button.

---


<img width="801" alt="Bildschirmfoto 2023-07-14 um 09 53 25" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/e6483447-fe2c-40c5-8a17-ea2cfd768c49">

1. Stop button

If there's no data transmitted from the satellite anymore, press the stop button.

---

<img width="856" alt="Bildschirmfoto 2023-07-14 um 15 01 16" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/e098f7fd-c699-46ba-a625-b0e834bd5b85">

1. Download button

Download the audio recording by pressing the download button.


## Decode the satellite data
Open the noaa-apt software, for reference about installing and starting, see #Prework. We will now take the data we received from the satellite and decode it into an image.

<img width="999" alt="Bildschirmfoto 2023-07-14 um 15 12 17" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/56de2d6e-6c3a-4dc2-b756-7600bbae4dc3">

1. Processing tab
2. File select bar
3. Decode button

First, load the file by pressing the File select bar, select your already downloaded audiofile. Secondly, press the decode button. And last but not least, move to the processing tab, by selecting it in the top bar.

---

<img width="999" alt="Bildschirmfoto 2023-07-14 um 15 25 17" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/30b3d7bf-e9b1-4b5f-8a36-1a883e7f03c2">
1. Process button

Press the process button, the picture should appear on the right side of the screen.

---

<img width="999" alt="Bildschirmfoto 2023-07-14 um 15 27 50" src="https://github.com/MakerSpace-GYMNBB/Guides/assets/89091446/20553f24-cbc6-454f-ba02-f147d3454719">

We were able to get quite a good picture.





