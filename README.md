# Hackathon PCB trophy
A cool trophy for the winners of your Hackathon

![trophies](https://i.imgur.com/uwmYAlM.jpg)

## What?
This repository includes the necessary software and hardware schematics and layout files to create some trophy-shaped boards that can be given as awards to the winners of a competition/hackathon/task/you-name-it.

The trophies have are programmable, using the ATTiny85 microcontroller and have the ability to play a tune once a button is pressed.

## Why?
As someone who often gets involved in organizing hackathons I had to come up with cool looking trophies for our competitions' winners. 3D printed trophies take too long to be produced and assembled so I resorted to a different option: PCBs. Compared to the 3D printed trophies, a PCB is more durable, can be assembled faster, requires less equipment from your side (i.e. no printer needed) and looks - if not more - then equally as cool. More importantly, the trophy is programmable and has the potential to spark interest in electronics and hardware.

## How?
The circuit as well as the code are relatively straight forward. A microcontroller (ATTiny85) is connected to a buzzer and a tactile button is connected to the microcontroller's reset pin, causing the firmware to reboot every time it is pressed. Everything is powered up by a CR2032 coin cell battery.

![fritzing circuit](https://i.imgur.com/UihgeHe.png)

On the software-side, the microcontroller plays an [RTTTL](https://en.wikipedia.org/wiki/Ring_Tone_Transfer_Language) tune (the [theme song from Rocky](https://www.youtube.com/watch?v=DhlPAj38rHc)) and then goes to deep sleep to preserve power. The RTTTL tune is played using code written by Brett Hagman from [Rogue Robotics](http://www.roguerobotics.com/).

### Components
* Hackathon trophy PCB ([Order it from PCBway.com](https://www.pcbway.com/project/shareproject/Hackathon_trophy.html))
* ATTiny85-20PU
* 12mm buzzer
* 4.7KΩ pull-up resistor
* 22Ω current limiting resistor
* 2032 coin cell battery holder
* 2032 coin cell battery

## Media
* [PCB trophies for your Hackathon](https://platis.solutions/blog/2018/05/16/pcb-trophies-for-your-hackathon/)
* [PCB trophies demo video](https://www.youtube.com/watch?v=lDynO2vfTys)
