<div id="top"></div>

<h1 align="center">Music Production via Color Recognition </h1>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://jacobsschool.ucsd.edu/">
    <img src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/d8df4aa599e8800ce6632881d2a99c795d335105/img/UCSDLogo_JSOE_BlueGold_Print.jpg" alt="Logo" width="1000">
  </a>
<h2>Team 6 - Odysseus </h2>
<h3>MAE148 Final Project</h3>

  ![](img/Car.webp)

</div>

## Table of Contents
1. Table of Contents
2. Team Members
3. The Project
4. Robot Design
6. References
7. Acknowledgemnets
8. Contact Information


## Team Members
![](img/Team.jpg)
<p align="center"> From Left to Right
* Kenneth Ho - Mechanical Engineering, BS, Class of 2026
* Kim Garbez - Mechanical Engineering, BS, Class of 2025
* Daniel Weng - Mechanical Engineering, BS, Class of 2024
* William Harris - Mechanical Engineering, BS, Class of 2025
  
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
* Play associated notes through a speaker integrated with the Jetson
* Multi-color detection and line following working simultaneously via modifying the Lane_Detection node 

### Challenges and Issues
* Concurrent line following around curves while playing notes
* Notes occasionally play twice
* RoboFlow color recognition with GPS navigation
* Speaker integration to the Jetson (resolved)

### Potential Improvements
* Multithread the lane detection code to:
  * Fix lane detection pausing:
    - Split locate_centroid into image_processing & lane_detection
    - Run these two methods concurrently
    - Implemented but untested, unsure if logic for each method works when split
  * Fix double detection:
    - One thread per color
* Adjust tempto through car speed rather than color placement
* Set up our own "musical road" to play multiple songs

## Demonstrations
One of our first times successfully playing notes upon seeing colors

https://github.com/user-attachments/assets/d42f7c1c-3745-4665-9393-c30176c342c2


An early run on the track

https://github.com/user-attachments/assets/10d149b9-d804-42b4-803d-4374953c319b


Successfully playing a song, "Au Clair de la Lune"

https://github.com/user-attachments/assets/710a8d51-5a31-4fa2-b96d-086e3f6e10a3


## Robot Design
### Mechanical Designs
| Part | CAD Model |
|------|--------------|
| Electronics Mounting Plate, by Kim Garbez | <img width="634" alt="Electronics Plate" src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/3689840ba557e5019b51dbe9dce521f3714cee7c/img/Plate.png"> |
| Camera Mount, by William Harris | <img width="634" alt="Camera Mount" src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/792c0eef7e7c57e736fde877688d5b3292c942d8/img/Camera.webp"> |
| Lidar Mount, by Kim Garbez | <img width="634" alt="Lidar Mount" src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/792c0eef7e7c57e736fde877688d5b3292c942d8/img/LIDAR.png"> |
| GPS Mount, by Kim Garbez | <img width="634" alt="GPS Mount" src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/792c0eef7e7c57e736fde877688d5b3292c942d8/img/GPS.png"> |
| Jetson Case, Retrieved from: https://www.thingiverse.com/thing:3532828/files | <img width="634" alt="Jetson Case" src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/792c0eef7e7c57e736fde877688d5b3292c942d8/img/Jetson_Case.jpg"> |


### Electrical System Diagram
<img width="634" alt="Wiring Diagram" src="https://github.com/dwengxz/SU24-TEAM6-MAE148/blob/792c0eef7e7c57e736fde877688d5b3292c942d8/img/Team_6_Wiring_Diagram.webp">

### References


### Acknowledgements
<p align="center"> Special Thanks To: Eric Foss, Alexander Haken, Dr. Jack Silberman

## Contact Information
* Kim Garbez - kgarbez@ucsd.edu
* William Harris Mechanical Engineering, BS - wharris@ucsd.edu / williamlh3rd@gmail.com
* Kenneth Ho Mechanical Engineering, BS - keh009@ucsd.edu / kenneth85451@gmail.com
* Daniel Weng Electrical Engineering, BS - dweng@ucsd.edu / dwengxz@gmail.com
