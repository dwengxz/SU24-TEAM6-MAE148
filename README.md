# <p align="center">Music Production via Color Recognition 

![](img/UCSDLogo_JSOE_BlueGold_Print.jpg)

### <p align="center">Team 6 - Odysseus 
### <p align="center">MAE 148 Final Project - SU II 24

*insert image of car*

## Table of Contents
1. Table of Contents
2. Team Members
3. The Project
4. Robot Design
5. Contact Information

## Team Members
* Kim Garbez - Mechanical Engineering, BS
* William Harris -
* Kenneth Ho - Mechanical Engineering, BS
* Daniel Weng - Electrical Engineering, BS

## The Project
The goal of this project was to implement a method of color recognition that, upon recognizing a color, would be able to play that color's associated note from a major scale. By implementing this color recognition with a line-following algorithm, we hoped to create a car that would be able to play music based on the colors it saw along a lined track. 

### What We Promised
* Line Following via a yellow line
* 3 Colors (RGB) associated with the first 3 notes of a C major scale (C4, D4, E4)
* Play associated notes through a speaker integrated with the Jetson Nano
  
### Nice-to-Haves
* Recognize eight colors for the notes of a major scale
* Navigate via GPS
* Play songs with different tempos (adjusting the speed of the car)

### What we Delivered
* Navigate via line following
* Recognize and assign 3 colors (RGB) to the first three notes of a major scale
* Play associated noptes through a speaker integrated with the Jetson
* Multi-color detection and line following working simultaneously via modifying the Lane_Detection node 

### Challenges and Issues
* Concurrent line following around curves while playing notes
* Notes occasionally play twice
* RoboFlow color recognition with GPS navigation
* Speaker integration to the Jetson (resolved)

### If we had Another Week...
* Fix lane detection pausing:
  - Split locate_centroid into image_processing & lane_detection
  - Run these two methods concurrently
  - Implemented but untested, unsure if logic for each method works when split
* Fix double detection:
  - One thread per color
* Adjust tempto through car speed rather than color placement
* Set up our own "musical road" to play multiple songs

## Demonstrations

## Robot Design
### Mechanical Designs

### Electrical System Diagram

## Contact Information
* Kim Garbez - kgarbez@ucsd.edu
* William Harris -
* Kenneth Ho - keh009@ucsd.edu / kenneth85451@gmail.com
* Daniel Weng - dweng@ucsd.edu / dwengxz@gmail.com
