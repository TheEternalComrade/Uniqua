---
title: "The Scheme Machine"
author: "@Ayo"
description: "A pen plotter for plotting schemes!"
created_at: "2025-05-30"
---

## May 30, 2025
Today, I started brainstorming. Imma be honest, I feel completely out of my depth with this one.
With a keyboard, there are plenty of resources, and I had completed Hackpad before to boot.

I'm not sure where to start. 

So, I've taken to gobbling up every resource I can find about pen plotters.

Here are some I've found so far:
![image](https://github.com/user-attachments/assets/383130a0-7df6-41c1-a4dc-08732876c0aa)
From Aliexpress

![image](https://github.com/user-attachments/assets/de689cf7-326a-4623-85bf-82fbf7f8f83e)
By [SuperbTech](https://www.instructables.com/member/Superb+Tech/)

![image](https://github.com/user-attachments/assets/fa97ddfb-8e67-406a-9af6-95dd355e1adf)

By [Dejan](https://howtomechatronics.com/author/howtom12_wp/)

Learning about and examining these designs, I'm starting to see a rough bill of materials:
- 2 stepper motors for the x and y axis
- A servo motor to lift and place the pen
- 6 linears rods, 4 for the y axis, 2 for the x axis
- 4 to 8 linear ball bearing(these are kinda expensive)
- 2 stepper motor drivers
- A CNC shield
- A elegoo uno(cheaper than arduino)
- A 12v power supply

One resource I found particularly helpful was [this plotter](https://www.youtube.com/watch?v=z4_OFkAW_JY&ab_channel=CreativityBuzz) 
designed with wood instead of plastic parts. I found that the design was a lot simpler without any of the frills plastic parts had. 
This was extremely useful in helping me get an idea of how to design the toolhead.

After a lot of YouTube videos, I sketched out a more detailed plan for The Scheme Machine. I wish I could say I had an intuitive goal for this, like I had convenience
for The Prince Keeb, but I just want this to work TT.

![20250530_212247](https://github.com/user-attachments/assets/ebd369d8-b7fe-4f3d-b6f4-0b1d41c5a149)

## June 4, 2025
I've placed the first item in my 3d model! A humble Nema 42-40 stepper motor.
![image](https://github.com/user-attachments/assets/a1182d79-db0c-42f6-b9e0-9483e253193e)

Next, I want to place a pulley, but I realized I didn't know what size it needed to be. After looking at what other models used, I decided to go with a timing belt with a width of 6mm and a pitch(think wavelength) of 2mm, which means I need GT2 pulleys that also have a width of 6mm. I also need to figure out how high or low the pulley will be on stepper motor shaft. Looking through the Blot assembly guide, it seems top of the pulley should be flush with the top of the shaft.
![image](https://github.com/user-attachments/assets/13a907e5-6f11-43ed-810b-87b498fd5b91)

Now that I've got my first motor and pulley figures out, I s'pose its time to actually model some original parts. I want to create a sort of stand that will screw into the stepper motor, and also hold 2 of the y-axis linear rods. But, I shall procrastinate that until tommorrow.

Time Spent: 1 hour


Time Spent: 5 hours


