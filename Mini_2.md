# Intro
My approach to installing the NLD booster board on a DJI Mini 2.

NOTE: i am not going to explain how to disassemble the drone and the remote, you can easily find video on youtube such as this: https://www.youtube.com/watch?v=C_9mIduaoMY

# Tools needed (bare minimum)
- A decent soldering iron with a thin tip and capable of reaching 400 celsius
- Siliconic non electrically conductive but heat condictive siliconic glue such as this one:
![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter to check for polarity and connections
- Phillips screwdrivers
- a sharp blade to scrape the PCB mask off the contacts
- some sandpaper and a little tool to stick the sandpaper to like this one:
[pic unavailable for now]
- Optional but highly recommended: some cheap tools to open electronic devices such as these: 
![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

# Additional components needed not sold by NLD
- 15cm long female ipex4 to female ipex4 cable (available on AliExpress)
- 14x15x4mm heatsink (Available on Amazon)

# General recommendations for the installation
- Use siliconic non electircally conductive but heat conductive glue to protect all new solder joints
- Use hot glue to stabilize antenna connections, so its easier to remove if you ever need to
- Use some heatsinks: the ones provided by NLD are decent but not the best (even though I have succesfully used them, on amazon you can easily find better solutions). Both the boards need a heatsink: in my explanation I didnt say it but I did use the heatsinks on both devices. 
- the battery connectors on the drone need to be scraped with a blade in order to be able to solder onto them
- Make sure that signal cables do not run over or below the booster board (not like I did in the pictures) as the interference could heavily degrade the signal


# Installing the booster on the Mini 2
Once you have taken the drone apart, you need to follow these steps

## Physical modifications to the drone
Using a cutter, cut a square window on the top of the drone (already disassembled) with the same size of the heatsink. 
![immagine](https://github.com/user-attachments/assets/4a1d6f11-0854-4d29-b4c1-a749dd821f3f)

I used the tool in the picture below with some 120 grit sandpaper attached to the tip to finely sand the edges and get the right size
![immagine](https://github.com/user-attachments/assets/a5628589-9d4c-4091-a76e-7ce5e8a4b9c8)

Stick the heatsink to the booster board and stick the booster board to the drone plastic cover using siliconic glue
![immagine](https://github.com/user-attachments/assets/53906b2d-94e9-4407-aa70-8838d3d70f40)

This should be the result
![immagine](https://github.com/user-attachments/assets/9dfbc7b9-6510-49aa-923b-9ef517b7b28a)

Stick the step-down board to the plastic shell of the drone in the back: be careful, where I stuck it in the picture below is not ideal, so you can put it somewhere else, BUT: do not put it on top of the GPS antenna (the large piece highlited in red in the pic below)
![immagine](https://github.com/user-attachments/assets/0cecb7ab-bf3f-4b33-af66-e859a5f7d1c0)


## Connect the power
Connect the step-down power module to the ESC board (you'll need to first remove the Core board from the drone).
Connections shown on the picture:
- GREEN: connect the ground (black wire) of the step-down module
- RED: connect the positive (red wire) of the step-down module
- YELLOW: connect the EN pin of the step-down module

![immagine](https://github.com/user-attachments/assets/7f5fb054-110d-4afb-b4ef-71cfbe75bf7d)

This is what the board looks like when it's on the drone:

![image](https://github.com/user-attachments/assets/93be2b71-102c-41a2-9bc6-62b31e5b7165)

TIP: in order to solder the wires to the battery connector (green and red connections) you will need to scrape the contacts with a sharp blade to remove any mask and use a very high temperature on your soldering iron (400 celsius)

## Connect the antennas
I don't really have pictures but the procedure is the following
- Buy a 15cm long ipex4 female to ipex4 female cable (you'll find it on AliExpress)
- When you open the drone, you need to remove this long antenna cable and replace it with the new one 15cm long that you bought by routing it in the exact same path through the drone (see the green line in the picture below)
![immagine](https://github.com/user-attachments/assets/7f7865cb-b596-47e9-903d-9b92d9eed730)

NOTE: Make sure that signal cables do not run over or below the booster board as the interference could heavily degrade the signal
