---
title: "Uniqua"
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

Time Spent: 5 hours

## June 4, 2025
I've placed the first item in my 3d model! A humble Nema 42-40 stepper motor.
![image](https://github.com/user-attachments/assets/a1182d79-db0c-42f6-b9e0-9483e253193e)

Next, I want to place a pulley, but I realized I didn't know what size it needed to be. After looking at what other models used, I decided to go with a timing belt with a width of 6mm and a pitch(think wavelength) of 2mm, which means I need GT2 pulleys that also have a width of 6mm. I also need to figure out how high or low the pulley will be on stepper motor shaft. Looking through the Blot assembly guide, it seems top of the pulley should be flush with the top of the shaft.
![image](https://github.com/user-attachments/assets/13a907e5-6f11-43ed-810b-87b498fd5b91)

Now that I've got my first motor and pulley figures out, I s'pose its time to actually model some original parts. I want to create a sort of stand that will screw into the stepper motor, and also hold 2 of the y-axis linear rods. But, I shall procrastinate that until tommorrow.

Time Spent: 1 hour

## June 8, 2025
I spent so much time fiddling with CAD software today. For some context, I use laptop. This laptop runs Windows, and for some wack-ahh reason, Fusion360 has basically no touchpad support for it. The only think I can do reliably is zoom in and out.

So, I decided to try out FreeCad. While it does have pretty good touchpad support, it's very different from Fusion360 and I felt really uncomfortable using it.

I eventually went back to Fusion360, and it turns out it actually does have touchpad support, though it's a really weird method.

I started designing the part that will sit on the y-axis stepper motor and will hold some of the y-axis linear rods. They're very rough rn, but I hope to make 'em look better in the future.
![image](https://github.com/user-attachments/assets/d6e3703b-17e0-40b2-8b16-6a45a0198eea)


Time Spent: 1 hour

## June 13, 2025
Today, I built more of my first y-axis section. 
![image](https://github.com/user-attachments/assets/7a05886b-9e55-4d52-8c1d-71c294805d9b)
<i>Isn't it neat?</i>

Funny story! For a while, I looked for a 3d model of linear rods of the size I needed for this. Then, I realized that I could just draw  8mm circle, and extrude it to the desire length. Convenient! 

I also started desiging the first y-axis gantry. I had to spend some time figuring out how the linear ball bearings would fit.
(insert screenshots here)
![17498711022763998460259937815160](https://github.com/user-attachments/assets/e1dd005b-1644-4a91-a110-bcf6fa917067)
![20250613_205450](https://github.com/user-attachments/assets/fbfa9fcb-1ff4-47cf-bb94-63bb5d344800)
![1749871131004886167080428974541](https://github.com/user-attachments/assets/e0f054f8-4157-4746-bd41-1491eb0c1de6)


Ultimately, I came up with a two-part deisgn where the bottom half of the gantry holds the bottom half of the linear ball bearings and the y-axis belt clip, while the top half of the gantry holds the top half of the bearings, has screw holes for the x-axis stepper motor, and holds the x-axis linear rods .

While I was trying to deign the y-axis belt clip, I realized I didn't quite know how close it would be to the ball bearings. So, I went through the painstaking process of designing my own in the project. 
![image](https://github.com/user-attachments/assets/6bd86ef8-4f1b-4139-9eb8-7fd00de7f39d)
<i>Belt!</i>

I think I'm done for today. Next session, I'll work on actually designing the belt clip, and the top part of the gantry. 


Time Spent: 3 hours

## June 14, 2025
Today, I did a lot of work on the y-axis gantry.

The thing that probably took me the most time was figuring out how the belt would be positioned.

I was originally going for a thin wedge for it, until I realized it needed to have teeth to match the belt. I tought about using zip ties, but I don't want to add more expense to this project. Since I'm not that confident in my 3d modeling skills, I settled on this loop design, where teeth of the belt latch onto each other:
![image](https://github.com/user-attachments/assets/2b4605d3-2355-4d04-9d89-3f9dece6c1e8)

I still need to edit this a bit to ensure the bearing's stability, but I think it's pretty decent so far

I also started working on the top part of the gantry. It took embarrassingly long amount time to figure out how to position it.

This is what it looks like so far:
![image](https://github.com/user-attachments/assets/fa113fd0-ffdb-4207-9f1b-471227351088)

Since working on this is literally giving me a headache, Imma call it quits till next week. Next time, I wanna develop the top part of the y-axis gantry so that it can hold linear rods, a stepper motor pull, and the x-axis timing belt.

Time Spent: 4 hours

## June 16, 2025
So I decided to completely redesign my y-axis gantry.
![image](https://github.com/user-attachments/assets/5c410ad7-d22a-4a1c-acd1-0ed7c2df8fb5)
<i>Gantryless y-axis</i>

I increased the spacing between the y-axis linear rods, because I realized doing so would allow the x-axis motor to fit better on the y-axis gantry. The dimensions of the stepper motors I plan on using are 42mmx42mm, while the spacing between the rods was previously 36mmx36mm

I'm quite pleased with the general idea of my gantry, though I will have to go over an beautify it later on for taste.
![image](https://github.com/user-attachments/assets/3e3c780a-328a-4d6d-ae89-97d682343081)

This is what Uniqua looks like rn! Did I mention I named my pen plotter Uniqua?
![image](https://github.com/user-attachments/assets/57b7e048-5927-4df2-9e44-42f2a88efbca)

Time Spent: 2 hours

## June 28, 2025
Ok, so for some reason, I think one of my journal entries didn't save. What a shame. I don't quite remember what I wrote, but I will provide a rough summary based on the changes from the most previous picture.

I realized that the idler pulleys do not have to be at the tippy top of the motor shaft, so I moved them down exactly 4.5mm. This allows the belt clips to be level with the linear bearing slots. This also reduces the height of the y-axis gantry by by allowing the x-axis stepper motor be placed lower.

![image](https://github.com/user-attachments/assets/1dfe8027-a8b7-4d69-a5da-24e3de6b27db)

I also completed most of the top part of my y-axis gantry.

![image](https://github.com/user-attachments/assets/6269782f-0105-482c-8c39-c36cccb83335)

Today, I started designing my pen gantry. 

![image](https://github.com/user-attachments/assets/1afa1c71-d749-4170-be46-d5ffb8469eb9)
<i>Sure it's just 2 linear bearings, but it's got vision</i>

I also plotted and planned how I'd attach the two halves of the y-axis gantry. Or more specifically, where I'd put the screw holes. It was surprisingly difficult, as I have to make sure the screw dont effect the belts, stepper motors, linear rods, etc.

Time spent: 1 hours

## July 10, 2025
It's been 12 days since I've worked on this project.

I think I'm going to add limit switches to Uniqua. It would save me the trouble of having to manually home the switches each time I want to print something. The thing is, I'm not quite sure where to place them? I think I'll look at my 3d printer for inspiration.

----

After examinination, I can conclude that the switches just needs to be at the extreme of each axis. 

Then comes the issue of idler pulleys. The main problem of understanding I'm having is how to attach them with minimal friction. Examing my 3d printer, it seems that placing them directly against the plastic should be fine, but I could only see so much from my vantage point.

Time Spent: 1 hour

## July 16, 2025
I've finally decided on the positioning for the y axis idler pulley. It doesn't seem to matter if it's flush with the plastic. But, I might need too add a nut sore something directly above it for stability.

<img width="594" height="520" alt="image" src="https://github.com/user-attachments/assets/8dd9f552-35e3-4db8-8f72-dfa699ab2455" />

----
I've also completed the main part of the gantry, where the pen will be.
<img width="647" height="391" alt="image" src="https://github.com/user-attachments/assets/8ce7e537-64b6-4aed-b3f0-066a6363fe2f" />

Next, I need to add the mechanisms for the actual penholder.
This is the servo motor, which will be responsible for the lifting of the pen(to avoid stray lines)
<img width="629" height="294" alt="image" src="https://github.com/user-attachments/assets/e5f28235-44fa-4049-8f42-a37ef06c1e45" />

I found that in my attempts to make mounting holes for the 2 halves of the pen gantry, I had accidentally made them block the entry of the linear ball bearings
<img width="306" height="321" alt="image" src="https://github.com/user-attachments/assets/c8a28079-7bf6-434d-9a00-5da08a789a87" />

This is what they look like fixed

<img width="449" height="384" alt="image" src="https://github.com/user-attachments/assets/1424db51-da7f-4781-885b-8b9fb685b464" />

I'm most likely going to change them a little for greater stability. A note, I'm going to be using heatset inserts instead of screwing them into the plastic directly.

----

I've made a significant portion of my pen holder!

<img width="647" height="486" alt="image" src="https://github.com/user-attachments/assets/d340a0b5-d6f8-4572-8c94-9b80ab9d9b53" />

Time Spent: 4 hours


## July 17, 2025

So, I was originally goiing to mount the two halves of the y-axis gantry the same way I mounted the halves of the pen gantry(, as seen above. But I realized it would interfere with the linear ball bearings, so I settled on this mounting option:

<img width="563" height="552" alt="image" src="https://github.com/user-attachments/assets/b5e8c321-dd41-42c6-b8c5-b23ccc73bcb0" />
I also added some anti-slip protection for the ball bearings

<img width="197" height="460" alt="image" src="https://github.com/user-attachments/assets/63980641-16ce-4700-a147-63a63f8fa1a2" />

Time spent: 1 hour

## July 21, 2025
Time to add limit switches!!!

After some consideration, I think Im gonna place the x axis limit switch on the pen gantry, and the y axis limit switch on the y-axis gantry.

----
They have been placed!

<img width="680" height="393" alt="image" src="https://github.com/user-attachments/assets/19284ff0-9277-4938-b277-6b2c3bbcfe9b" />

----

So, I completely forgot that the holes i placed to connect the halves of the y-axis gantry will intersect with the linear rods, so I had to change the design.

<img width="655" height="515" alt="image" src="https://github.com/user-attachments/assets/9cdeb158-125e-4645-a3ff-2ca1e9548602" />

----
<img width="425" height="302" alt="image" src="https://github.com/user-attachments/assets/62513a58-b9ba-4176-8ea9-3282fff14abb" />

I've added the linear rods that will be used for the pen lift mechanism. In addition, I've made a significant portion of the actual holder part of the pen holder. I just need to add holes for the tightening screws. The little cylinder is for the servo motor to push up on, though I might have to replace it with a M2 screw for printability. Actually, I'm defintely going to do that.

<img width="351" height="430" alt="image" src="https://github.com/user-attachments/assets/ae9c8eee-08d4-4dff-ae80-436f9aaa0c1d" />

----
Hole created!

<img width="703" height="363" alt="image" src="https://github.com/user-attachments/assets/b67861cb-9415-4ffc-a9ef-3afdf3d9e3d2" />

----
Next, I need to add some flair to all the parts and a case for the electronics

Time Spent: 3 hours

## June 22, 2025
I've added the holes for the pen grip, which will allow for a firmer fit. I also increased the length of the penholder part so that a shorter spring can push it down.

<img width="396" height="519" alt="image" src="https://github.com/user-attachments/assets/22dc297c-b06a-444a-8e68-5ed1b8c5a7be" />

----
Upon concerns of stability, I redesigned the holder for the stepper motor so that it can be mounted upside down. This will allow me to use a threaded insert near the bottom.
<img width="384" height="469" alt="image" src="https://github.com/user-attachments/assets/e59b14a3-11d3-471f-be8d-65b783801bbb" />

Time Spent: 2 hours







