---
title: "The Nest"
author: "bcon"
description: "Versatile Filament Spool Storage with Active Temperature Control"
created_at: "6-2-2025"
---

Total Time Spent: 28 Hours

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

Time Spent: 1.5 Hour

## 6/5/2025 Log 3: Starting CAD

![image](https://github.com/user-attachments/assets/5d9c8a02-4d4a-4d9a-a09f-b0b874dd597f)

I started the CAD for this system. I first made the 2020 frame that used these special corner blocks to create a strong joint between the corners. This is different from the corners on Hydra, but since this system is smaller, it doesn't need to be as strong and thus these would work. 

![image](https://github.com/user-attachments/assets/50be3d11-c880-43ab-93e1-5491bc759a64)

Next, I created the panels that would enclose the system. Since this system needs to be sealed, these panels go edge to edge to ensure that the system is fully sealed and thus moisture cannot enter. 

![image](https://github.com/user-attachments/assets/8e8139d0-9012-4ce7-adf4-b0901c0fbbaf)

Finally, I created the corner blocks. These not only better secure the corners, but they add a unique function of this system: stackability. 

![image](https://github.com/user-attachments/assets/16fe3c5f-1bc6-4fbc-8407-a8b2986127fb)

Through a mirrored, layered design, it is possible to stack multiple of these systems on each other. I will be keeping this part of the design in mind as I create the other parts of the system to ensure it stays stackable. 

Time Spent: 6.5 Hours

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

Time Spent: 5.5 Hours

## 6/11/2025 Log 5: Wiring

I decided to do the next step: electronics. After extensive, extensive research I got this: 

![image](https://github.com/user-attachments/assets/18dc0bc9-86a7-4eaf-bf35-da9f3407c855)

I am using an AC ceramic PTC heater to heat the heated chamber. I am also using a 35W 5V power supply that will allow me to power my controller, most likely a Pi 0 2W. Additionally, I have an SSR to control the power going to the ceramic heater. I will also use the controller to control when the chamber gets heated, along with giving me crucial information - such as the humidity of the system. 

Time Spent: 3 Hours

## 6/12/2025 Log 6: Almost Done

![image](https://github.com/user-attachments/assets/696d8efb-b3a0-452f-9f65-ad3f276f1c93)

I spent a small amount of time today adding in the fused inlet. Final thing to do is the silica gel holders and the doors and I am done. 

Time Spent: 30 Minutes

## 6/13/2025 Log 7: Sensor and Screen

I spent some time figuring out what screen and sensor I wanted to use, after which I put them into the CAD. The sensor will allow me to know what the temperature and humidity of the system will be, while the screen will allow me to control the system.

![image](https://github.com/user-attachments/assets/ccffced9-4128-484d-97f0-6274867c03d0)

I just have to figure out how I am doing the front doors, after which I believe I am done. 

Time Spent: 2 Hours

## 6/15/2025 Log 7: Doors! Finally!

![image](https://github.com/user-attachments/assets/2ef9055d-c8e7-46e5-a2e4-f98a03ef55d7)

I decided to use a gasket sealing tape like [this](https://www.amazon.com/Frost-King-R734H-Sponge-Rubber/dp/B000BQWWF4?crid=1D80KEYQZYFL0&dib=eyJ2IjoiMSJ9.7Rkj69G2fHceRJ7jjl61apGrT-A6o6k0OrctL8sxLlTQOcWf3_lJsEPm9X1-suWQniuu0oC5ps_Q9cI413ym1mWteZnjWixh07DJOnLhR-w0ClCAGNCQJps0yZ1uk2SVjAdt9Xio7yu8fGbQed3_b9-OcdWfGO_GLKZJDUzu4qvVHQjKrEvDKht1DVHDWdJxFRqKKPfzOd_in4G6XvqsBVE-7R6tYX3RdyY8sXTLV3fTUEb-qT9S2zSp6YGlBd6Zv6nPap-WLCOoVV2E86yNI-Z_A9-5HfxqLH7w8gnIx3g.29bXTPl1r7yZlH6CzJnNph30QZI5mxy9kII5ceC3Dws&dib_tag=se&keywords=edpm%2Bfoam%2Btape&qid=1750051417&sprefix=edpm%2Bfoam%2Btap%2Caps%2C129&sr=8-6&th=1) along with some nifty clips in order to create an airtight seal. By compressing the foam, it creates a seal, leaving moisture unable to enter. These clips are reminicent of the AMS system. 

![image](https://github.com/user-attachments/assets/d6681774-339f-4793-81fe-53e80935ff40)

With this, I am officially done! 

Time Spent: 2 Hours
