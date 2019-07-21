---
layout: post
title: Game Development using Phaser
date: 2019-07-19
description: A repost of my old work in USC Interaction Lab
excerpt: Simple Game Development using Phaser - html5 game engine framework
project: true
---

# Summary
The goal of my work was to continue to developer a simple game for kids specifically aim for
kids with Autism spectrum disorder (ASD). 

# Documentation(updated on 8/15/2016)
1.	Ubuntu version we use is 14.04 (Trusty Tahr)
2.	To set up and run all the html file, you need a local web server. Python is used to set up the server.
3.	Install Python 2.7.11 on Ubuntu.
4.	Click on terminal, change directory into clone repository in bash, and run –mSimpleHTTPServer
5.	Open any web browser, type in http://localhost:8000/index.html, you should be able to run the game in the web browser
6.	If you want to switch to the other game, type http://localhost:8000/app2.html or http://localhost:8000/app3.html

## Game description 
### Game 1 Activity 1 - Pack moonrocks 
#### index.html
•   Changes the way that the rocks are generated on panel
•	Create box and panel group
•	Set up coordinates in the box and panel
•	Rearrange object position after they are being drag
•	read index.html_about.txt under the clone repository
•	index.html combines activity 1 & 2 
### Game 1 Activity 2 - Charge Spaceship 
#### app5.html
•	Changes the way that the crystals are generated on panel
•	Create box and panel group
•	Set up coordinates in the box and panel
•	Rearrange object position after they are being drag
### Game 1 Activity 3 - Select Galaxy 
#### app4.html
### Game 1 Activity 4 - Select Planet 
#### app3.html
### Game 1 Activity 5 - Feed the stardust 
#### app2.html
•	Create Left and Right group
•	Set up coordinates in yuki and yana box
•	Star returns to its original position while they are not in yuki and yana box

### Game 2 Activity 1 - Board the space pet 
#### app6.html
•	Space pets return to its original position if they are not dragged into the right spot
### Game 2 Activity 2 - Organize by color
#### game2-1.html
•	sort colored rocks into the empty boxes without color
#### game2-3.html
•	sort colored rocks into the empty boxes that match its color
#### game3-1.html
•	sort colored crystals into the empty boxes without color
#### game3-2.html
•	sort colored crystals into the empty boxes that match its color
### Game2 Activity 3 - Organize by item 
#### game6-1.html
•	sort item into the empty box

### Game 2 Activity 4 - Copy the sequence
#### game4-1-2.html
•	copy the sequence into the 4 empty boxes
Game 2 Activity 5 - Complete the sequence
#### game5-1.html
•	generate a sequence with 1 type of object and 1 empty slot
#### game5-2.html
•	generate a sequence with 2 type of object and 2 empty slot
#### game5-3.html
•	generate a sequence with 3 type of object and 3 empty slot

## Note
- https://draeton.github.io/stitches/ is used to create spritesheet for images
- Phaser game engine/framework is used
    - Preload and Create functions are written under window.onload function
        - Preload function
- Load all images / scale the game
    - Create function
- Add sprite to image
- Enable input of sprite
- Add event like onDragStart, onDragStop, onDragUpdate, onButtonPress, onButtonRelease

## Extra Information on Index.html
Index.html combines the PACK_MOONROCKS activity 1 already in index.html with the CHARGE_SPACESHIP activity 2 from app5.html

## NOTE:
The variable name changes below: 
Goal is the rectangle that frames the target number.
Box is the either the rectangle (activity 1) where the moon rocks or battery where the crystals (activity 2) are moved to.

var activity, initially 0,  is used to keep track of the current activity.

Using a switch that checks against activity we are able to run the code pertaining to the current activity.

Things that may need changing:
•	the way the value of activity is changing. Currently in changeActivity, activity increments by 1 ( activity++). 
•	may want to move the code from the changeActivity function into the create function and delete the changeActivity function.
•	may want to use Phasere's physics properies to make use of a sprite overlapping function.


# Link
[Original Repo](https://github.com/interaction-lab/games-old/tree/Kin)
[Repost Website]