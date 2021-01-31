# Overview

Lightweight homebridge plugin that allows you to control your DreamScreen Ambient TV device with homekit.
Features full control over color, video, ambient and sleep mode.                
It uses my python script featured here: https://github.com/ToracX/DreamScreenCommander


## Installation:


install homebridge: ```npm install -g homebridge```                        
install this plugin: ```npm install -g homebridge-dreamscreen```                   
update your ```~/.homebridge/config.json``` file with correct ip adress, see below.

## Example config:
#### Dont forget to set the correct ip.
```
"accessories": [
  {
   	  "accessory": "Dreamscreen",
   	  "name": "TV Backlight",
      "ipadress": "192.168.178.187"
  }
]
```
#### The ip adress of you're dreamscreen can be found in the app under "Update and Reset".

## Using the plugin
You get two accesoires packed in one tile, seperating them is completely possible 

First accesoiry is the switch, this is used for setting the mode. 
* Flipping it on enables video mode / amiblight. 
* Flipping it off puts the dreamscreen to sleep.

Second accesoiry is the led slider, this has two main functions.
* Changing brightness, simply by sliding to an exact percentage.
* Changing color, when you change the color the dreamscreen gets set to ambient mode and will display the set color.


## Ideas for usage
* Automatically adjust Dreamscreen brightness based on room ambient brightness
* Control your Dreamscreen inputs with scenes.
* Set time based events to turn on and off the leds.

If you have any questions, ideas or improvements please fill in an issue form and I will look at it as soon as possible.
