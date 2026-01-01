# Arduino-based Hand Gloves Piano

![Arduino](https://img.shields.io/badge/Arduino-Uno-00979D?style=for-the-badge&logo=Arduino&logoColor=white)
![Language](https://img.shields.io/badge/Language-C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)


An Arduino-based digital piano that can be operated by wearing hand gloves. This project creates a small digital harmonium(piano) where touching each finger to the thumb produces a corresponding musical tone.

## Overview

The aim of this project is to create an Arduino-based piano that can be operated by wearing hand gloves. In a typical harmonium, we create different types of tones or music. In this project, we use sound frequencies to produce musical notes (Sa, Re, Ga, Ma, Pa, Dha, Ni, Sa in Indian classical music, or C, D, E, F, G, A, B, C in Western notation). It's like a small digital harmonium! When one finger touches the thumb, a corresponding tone will be sounded.

## Features

- 8-note piano using Arduino
- Operated via hand gloves with touch sensors
- Piezo buzzer for sound output
- Simple button-based interface

## Components Required

- Arduino Uno (or compatible board)
- 8x Push buttons or touch sensors
- 1x Piezo buzzer/speaker
- 8x Resistors (10kΩ recommended for pull-down)
- Jumper wires
- Breadboard
- Hand gloves with conductive material (for touch sensors)

## Circuit Diagram

<p align="center">
  <img src="https://github.com/Uchswas/Hand-Gloves-Piano/raw/master/circuit_diagram.png" alt="Circuit Diagram"/>
</p>

## Setup with Hand Gloves

<p align="center">
  <img src="https://github.com/Uchswas/Hand-Gloves-Piano/raw/master/hands_gloves_piano_setup.jpg" alt="Hand Gloves Setup"/>
</p>

## Wiring Instructions

### Button Connections
- Button C → Digital Pin 2
- Button D → Digital Pin 3
- Button E → Digital Pin 4
- Button F → Digital Pin 5
- Button G → Digital Pin 6
- Button A → Digital Pin 7
- Button B → Digital Pin 8
- Button C (octave) → Digital Pin 9

### Speaker Connection
- Piezo buzzer/speaker → Digital Pin 13
- Connect one terminal to pin 13 and the other to GND

### Button Wiring
- One terminal of each button → Respective digital pin
- Other terminal → GND
- Use 10kΩ pull-down resistors between digital pins and GND (optional but recommended)

## Prerequisites

- Arduino IDE (version 1.8.x or later)
- Arduino Uno board
- USB cable for programming

## Installation & Setup

1. Clone or download this repository
2. Open the Arduino IDE
3. Connect your Arduino Uno to your computer via USB
4. Open the `SourceCode.txt` file and copy the code
5. Paste it into a new Arduino sketch
6. Select the correct board: **Tools → Board → Arduino Uno**
7. Select the correct port: **Tools → Port → [Your Arduino Port]**
8. Click **Upload** to program the Arduino

## Usage

1. After uploading the code, the Arduino will be ready to use
2. Wear the hand gloves with conductive touch sensors
3. Touch each finger to your thumb to trigger the corresponding musical note
4. The piezo buzzer will play the corresponding tone when a button is pressed



## Project Structure

The source code can be found in the `SourceCode.txt` file. Simply copy the code into the Arduino IDE and upload it to your board.


```
Hand-Gloves-Piano/
├── SourceCode.txt               # Arduino source code
├── circuit_diagram.png          # Circuit diagram
└── hands_gloves_piano_setup.jpg  # Hand gloves setup image
```



---

**Note**: This project uses Western musical notation (C, D, E, F, G, A, B, C) in the code, which corresponds to Indian classical notes (Sa, Re, Ga, Ma, Pa, Dha, Ni, Sa) respectively.
