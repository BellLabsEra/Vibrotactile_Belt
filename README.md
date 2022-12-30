# Vibrotactile Belt Repo
### Contents
Short-hand name | Descriptive Name | Short Description
--------- | ---------------------- | -----------------
electrical | Electrical Subsystem | Contains the Schematic, PCB, BOM, Workflow
src | Soucre | Contains the Python Firmware for the Raspberry 4 Model B, ChangeLog Document
notes | | Contains Hardware and Software Resources for knowledge building, PDFs of Handwritten notes, etc
images | blah | blah 
## System Architecture 
![System_Arch](https://user-images.githubusercontent.com/94195261/210112692-007c81c0-45f4-432b-94a8-f94da3d623b4.PNG)

System Architecture diagram showcasing how the Vibrotactle Belt’s electronics communicate with the VIVE HTC + Motion Capture systems and Unity VR game, via an SSH web socket. During VR game experiments, the mini-game will produce static or dynamic obstacles/threats. The host computer will relay obstacle locations in the form of a binary map and compute the Action Potential filed, then send the potential field height and safety heading vector (gradient decent vector) to the vibrotactile belt, which in turn will calculate and activate the vibration intensities of the motors within the dispersion range

---
### System Definition:
The vibrotactile belt is a wearable, haptic device, that primarily enhances a user’s ability to perceive and detect obstacles in their (immediate) surroundings; additionally, it has features that prompt them in a direction to evade the threat.

### Form: 
An adjustable belt containing 8 motors equally spaced along a person’s torso.
### Function:
The system will receive information about an obstacle/threat location in a 2D Space, then will send a wave of vibration to the user’s body (tactile stimulus), in the direction of the obstacle(s), with a magnitude depending on the distance the user is from the obstacle.

## UML Class Diagram of Firmware
