---
layout: default
---
{% include nav.html %}

# Retro Synth

**Course:** Hands-On PCB Engineering DeCal @ UC Berkeley

|Demo |Description|
|:---------------------------------------|:---------------------------------------|
|![synth_vid](./synth_vid.mp4) | As part of a student run project course, I am working with 2 partners to build a functional 12 note analog PCB synth. After we collaborated on the schematic and layout of the board, my partners focused on firmware development and software debugging while I executed the soldering, assembly, and hardware bring-up of the board. We then conducted rigorous testing to validate circuit functionality and successfully created the synth.|

**Design**

This PCB has 12 tactile switches, each simulating one of the 12 chromatic pitches. We are using an ESP32-S3-Wroom-1 microcontroller, programmed to generate a wave of the corresponding pitch depending on the switch pressed and the waveform selected. This wave goes through high and low pass filters that can be adjusted to change the sound quality. This wave goes through high and low pass filters controlled by potentiometers, then an amplifier and speaker. At the same time, the waveform will be displayed on an OLED display. 

Components:

- USBC for a power supply and data bus
- 5V to 3.3V voltage converter
- ESP32 Microcontroller
- Four potentiometers for filter, waveform, and volume control
- 12 buttons that play sound when pressed
- OLED display for waveform
- Class AB Amplifier
- Speaker

|Schematic |Layout|
|:---------------------------------------|:---------------------------------------|
|![block diagaram](/images/synth-schm.png) | ![synth schematic](/images/synth.png)|


**Bring Up**

One challenge I faced was soldering the board. The components we ordered were very small, and I pulled up the trace on a capacitor for the first board I tried to solder. Eventually (with solder paste, heat guns and plenty of flux) I was able to finish soldering and we could move on to testing.

![synth-pic](/images/synth-pic.png) 

