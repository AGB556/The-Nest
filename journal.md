---
title: "The Nest"
author: "bcon"
description: "Versatile Filament Spool Storage with Active Temperature Control"
created_at: "6-2-2025"
---

## 6/2/205 Log 1: Idea Generation

I started this project by defining my goals and generating some ideas to start the CAD off of.

Goals:
 - Store 5 Spools of filament
 - sealed environment
 - active heating w/custom PCB to sense temperature/humidity
 - purpose built for HYDRA (hence the 5 spools)

Bonus: Add in an AMS type system as well, or at least an option to add it on later. 

Drawings:

![image](https://github.com/user-attachments/assets/790134bf-b20f-4c33-8c54-a1e3bf8aee37)

One option is to have one sealed system with active temperature control and heating for filament drying. This has many pros and cons, pros being the simplicity behind the idea and the fact that it is relatively simple to build. However, some cons are the fact that the system has to cool 5 spools at once, which not only requires more energy, but could waste energy if some of the spools are already dry and ready to go. One could also turn this into a MMU type system.

![image](https://github.com/user-attachments/assets/b89acd39-42e0-43d6-9c37-ca89f397a26e)

Another option is to seperate the filament drybox system into its own seperate but connected chamber, which would cut down on the energy and effort needed to dry the filament, while still having the capability to hold 5 spools. I could also add a MMU type system to the non drybox part as well. 

After deliberating, I will be going to explore the second option as it seems more viable as an option. I have not decided whether or not I will try to add an MMU system yet, but I am currently leaning towards not going for it as Hydra already has the capability to use 5 different filaments. It is still on the table for now though. 

Time Spent: 1 Hour

## 6/3/2025 Log 2: Starting Some Sketching and Defining My Goals

I first went into this with the idea of having support for both 3kg and 1kg spools. I also knew I wanted the capability to hold 5 1kg spools to support Hydra. I started with a sketch that satisfied these requirements. 

![image](https://github.com/user-attachments/assets/8658ea86-acf1-4d56-8184-2e6cd7a57612)

After looking at the immense size this would take up, along with realizing that I have personally never used a 3kg spool, I decided to abandon support for the 3kg spool in the interest of space. 

![image](https://github.com/user-attachments/assets/6fad9689-39d5-4ea0-80ec-39b3e0158cab)

![image](https://github.com/user-attachments/assets/6cbac757-c785-420b-ab20-8a94689cd2ba)

This cut down on the space by a few inches in all dimensions, greatly decreasing the footprint. 

My next steps are to start modeling the frame and find some good rollers for the spools to ride on. 

Time Spent: 1 Hour

## 6/5/2025 Log 3: Starting CAD

![image](https://github.com/user-attachments/assets/5d9c8a02-4d4a-4d9a-a09f-b0b874dd597f)

I started the CAD for this system. I first made the 2020 frame that used these special corner blocks to create a strong joint between the corners. This is different from the corners on Hydra, but since this system is smaller, it doesn't need to be as strong and thus these would work. 

![image](https://github.com/user-attachments/assets/50be3d11-c880-43ab-93e1-5491bc759a64)

Next, I created the panels that would enclose the system. Since this system needs to be sealed, these panels go edge to edge to ensure that the system is fully sealed and thus moisture cannot enter. 

![image](https://github.com/user-attachments/assets/8e8139d0-9012-4ce7-adf4-b0901c0fbbaf)

Finally, I created the corner blocks. These not only better secure the corners, but they add a unique function of this system: stackability. 

![image](https://github.com/user-attachments/assets/16fe3c5f-1bc6-4fbc-8407-a8b2986127fb)

Through a mirrored, layered design, it is possible to stack multiple of these systems on each other. I will be keeping this part of the design in mind as I create the other parts of the system to ensure it stays stackable. 

Time Spent: 6 Hours

## 6/9/2025 Log 4: Roller System and Adding Color

![image](https://github.com/user-attachments/assets/ec11b834-8c18-4474-b8a7-d362b68ef0fb)

Obviously, from this screenshot, a lot has changed. First, I added the same color scheme as Hydra for it to match. Then, I worked on the roller system. 

Utilizing an 8mm diameter shaft along with some bearings, this made up the base of my roller system. 

![image](https://github.com/user-attachments/assets/3461575e-d592-462f-9147-7316a84e2c2d)

![image](https://github.com/user-attachments/assets/b1c7b740-bd20-4584-bf19-672012e5d484)

Using a custom 3D Printed roller over a set of roller bearings, I can create a roller that allows the spools to spin freely without binding while also keeping the spool constrained where it is so it doesn't walk off. Unlike systems like the Bambu Lab AMS, there is no physical divider between the spools, just this custom roller keeping them in place. 

![image](https://github.com/user-attachments/assets/369b418b-9a62-486b-9de4-991a9fdc9185)

Through some nifty 3d printed parts, the shaft runs all the way across and supports all 5 spools. Additionally, through another set of printed parts I successfully sealed off the active heating from the passive heating. 

![image](https://github.com/user-attachments/assets/0b94925c-7436-4ade-8a16-d45bf9874862)

This panel, combined with some liquid silicone will seal the active heating off. Additionally, I will use said silicone to seal off any other gaps in order to keep the entire system sealed. 

Next Steps: Electronics, Venting, and a place to store the silica packets. 

Time Spent: 5 Hours
