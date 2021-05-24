# Pen-Testing-Drone-Prototype

The following files and or folders to check out are:
      
  * Custom Drone Software Sub folder under this repository. 

     I reverse engineered how the tello drone API communicates with the drone in order to fabricate my own user interface. The final build will integrate the arduino library in        order to directly communicate and control the server motors for the drone, as well as allowing me to properly integrate the pentesting app with it. This has a lot to do with      python which is what you're looking for. Hope this helps.
       
  * Drone Schematics.cpp

     I know this file says CPP, but it's actually just all text and documents the full schematics of the project, and will help you better understand how I critically think,            analyze, and organize my projects. A must read
       
  * RB_Flight_Controller_Module.ino
              
     This is the main face of the program. I'm creating my own flight controller, that will control a series of servo motors, via ESC modules, that will allow me send various data      signals to the drone in order to manipulate the speed of the motors in order to manipulate the altitude and movement of the motors. 

Inspired by Marcus's drone from Watch Dogs 2 and as a tribute to the series, I'm developing a penetration testing drone, it's sole purpose,
to fly around capturing packet data, as well as cracking Wireless encryptions, integrating the use of a raspberry pi zero to host my UDP BackDoor 
Server program in order to communicate with the drone and see what's on the pi as it's flying. Think of it as a flying wifi-pineapple. When the 
drone boots up, the pi zero will auto login, where a set of scripts will run, starting up the UDP Server. 

The flight controller for the drone is built up from scratch, rather than using a pre-built one. The drone will take a series of commands from 
the transmitter, the controller, also built from scratch (keyboard input option available as well), and depending on the value read from the analog of the 
joystick module, will move the drone either: forward, backward, left, right, up down, and shifts the values of the signal values sent to the ESC's of the 
drone in order to move the drone accordingly, all calibrated properly. The drone is still in prototype phase, and is near completion. 

In the future I will be diving into how to facial recognition software, which I will build from scratch in order to build a true replica of Wrench from Watch
Dogs 2, his face mask that acts as a build board, where his facial expressions are scanned by the mask in order to display a a set of emojis that show his emotions.
