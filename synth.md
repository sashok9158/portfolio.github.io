---
layout: default
---
{% include nav.html %}

# Retro Synth - In Progress!

**Course:** Hands-On PCB Engineering DeCal @ UC Berkeley

As part of a student run project course, I am working with 2 partners to build a functional 12 note analog PCB synth. We are currently in the design phase for this project and I am working on cleaning up our schematic and adding footprints for the board on KiCAD.

**Design**

This PCB will have 12 tactile switches, each simulating one of the 12 chromatic pitches. We are using an ESP32-S3-Wroom-1 microcontroller to generate waves corresponding to a pitch depending on the switch pressed. This wave will then go through high and low pass filters controlled by potentiometers, then an amplifier and speaker. At the same time, the waveform will be displayed on an OLED display. 

I am currently working with my team to order parts to put together the board and desiging a 3D-printed enclosure to hold the synth. Next steps include soldering parts on to the board and coding the ESP32-S3-Wroom-1 microcontroller to generate waves corresponding to different pitches.

|Schematic |Layout|
|:---------------------------------------|:---------------------------------------|
|![block diagaram](/images/synth-schm.png) | ![synth schematic](/images/synth.png)|
