# VillageVR

## Introduction
VillageVR is an Interactive Virtual Reality Environment created using Unity. All the concpets used in this was learned from Virtual Reality Course offered by University of London on Coursera.

This project can be viewed by anyone having a simple Head Mounted Display like Google Cardboard.


## Tools Used

### Unity
* I built most of the project in Unity 3D.  Currently, the only way to create fully immersive interactive virtual reality experiences that you can step into and interact with is to use 3D computer graphics.

* A 3D game engine is essentially a IDE (Integrated Development Environment) which allows realtime integration of scripts with 3D graphics to produce various kinds of media such as Games, Movies, Animations or in my case VR Environment.

### Virtual Studio Code
* Virtual Studio Code which is a IDE developed by Microsoft was used for coding various scripts to add interactivity to the VR Environment.

### Blender
* I used Blender to create some of the 3D assets used in the environment. 

## 3D VR Environment
I wanted to create an environment that should sustain my hardware requirements but still also allow user to properly experience VR. So, I decided to create a open environment consisting of Green Terrains, Mountains, and buildings. I created some of these assets using Unity, Blender, and some were imported from the Unity Asset Store.

## Interaction in VillageVR
In order to create the VR illusions, I had to add ineractivity to VR Environment. I added multiple interaction scripts each serving different purpose such as Audio, Teleportation etc. 

Most of these scripts are already provided by Unity as they are often used to add any form of interaction, but I had to modify them according to the requirements of my project. 

Due to hardware restrictions I decided to only use Sight Based Interaction (Looking at a particular object for a few seconds to interact with it).

* **VR Interactive item** is the script that detects the light rays from the main camera which is actually the user’s viewpoint.

* **VR Action Harness** is basically to used to provide user some kind of feedback that their gaze has been registered and an interaction is happening.

* **VR Interactive Audio** essentially triggers the audio of the object on and off depending on the output of VR interactive Item Script.

* **VR Interactive Audio** is similar to VR interactive Audio. It triggers an animation whenever gaze is detected from the user.

* **VR Teleport Target** transports the camera base to where the user is looking at. So when a user looks at one pedestal from the main camera the camera base is transferred to that pedestal. Thus allowing user to navigate through the VR world.
 
### State Machine Interaction
I also used State Machine based Interaction which was added to the game object “Rake”. A state machine consists of a number of states, where each state is basically an animation. But the important thing is it also consists of transitions between states.

If a user would gaze at the rake, RakeStart animation would be turned on and the rake would start working and when the user would look again at the rake, it would stop working and the rake would return to its original position. To implement this interaction VR Interactive Animation script was added along with VR interactive item and action harness.


## User Interface in VR

I created a diegetic UI which essentially means that the User Interface will be present inside the VR Environment. I wanted to add it to just guide the users what to do in the scene and which of the objects can they interact with.

## Results
![alt text](./Result_1.png)

![alt text](./Result_2.png)
 

  
 
