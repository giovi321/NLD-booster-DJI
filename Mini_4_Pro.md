# Intro
My approach to installing the NLD booster board on a DJI Mini 4 Pro.

NOTE: i am not going to explain how to disassemble the drone and the remote, you can easily find video on youtube such as this: https://youtu.be/rLTtYpftaGs?feature=shared

# Tools needed (bare minimum)
- A decent soldering iron with a thin tip and capable of reaching 400 celsius
- Siliconic non electrically conductive but heat condictive siliconic glue such as this one:
![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter to check for polarity and connections
- Torx and phillips screwdrivers
- a sharp blade to scrape the PCB mask off the contacts
- Optional but highly recommended: some cheap tools to open electronic devices such as these: 
![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

# General recommendations for the installation
- Use siliconic non electircally conductive but heat conductive glue to protect all new solder joints
- Use hot glue to stabilize antenna connections, so its easier to remove if you ever need to
- Use some heatsinks: the ones provided by NLD are decent but not the best (even though I have succesfully used them, on amazon you can easily find better solutions). Both the boards need a heatsink: in my explanation I didnt say it but I did use the heatsinks on both devices. 
- the battery connectors on the drone need to be scraped with a blade in order to be able to solder onto them
- Make sure that signal cables do not run over or below the booster board (not like I did in the pictures) as the interference could heavily degrade the signal


# Installing the booster on the Mini 4 Pro
Once you have taken the drone apart, you need to follow these steps

## Connect power
1) remove the main board and the obstacle avoidance cameras from the top
2) remove the three torx screws holding the battery connector in place and gently lift the battery connector from its place but do not remove it completely as it is not needed - I dont have pictures but you sinply have to remove the screws from the hole where the battery goes, then from the top of the drone (underneath the obstacle avoidance cameras) push a bit with tweezers the little PCB where the battery connector is installed. Now ok the back of the pcb lift gently the piece of adhesive plastic and you will expose the back side of the battwry connector. Here you need to identify correctly the contacts with the positive and negative and solder the wires that will go to the step-down voltage converter. 
3) using a sharp blade, scratch the back of the connector to remove the masking from the PCB so that you can solder the wires - it will take quite some time to make the solder stick to those pads, don't over heat it (350 celsius is fine) and if it does not work just keep scraping them with a blade
4) solder the wires according to the following pin out of a Mini 4 Pro battery and cover with siliconic heat-conductive
![338014364-85232647-8a49-44d1-b3a3-88f20bb655ff](https://github.com/user-attachments/assets/857ae314-c66a-4ed5-8d86-c96ad2aab921)

6) connect the step-down voltage converter to the battery and the booster board
7) connect the EN pin of the step-down voltage converter to the inductance labelled with 2R2 as shown in the picutre below and cover with the siliconic heat conductive glue
![338014131-4d84ec24-1892-418b-a313-3f99b1996834](https://github.com/user-attachments/assets/eb515ecb-e488-45f1-8e90-4fd73c0442b4)

8) glue with the siliconic glue the step-down converter board to the top of the obstacle avoidance sensors cluster
![338014160-6e45433c-1c5e-4add-b2a9-b0326a34729f](https://github.com/user-attachments/assets/0e1cde2b-e19f-41ef-a047-eeef397ace45)


## Connect the antenna
8) disconnect the antenna connector labelled with ANT0 and connect the booster board (ANT0 has the longest cable thus it is able to reach the booster board, any antenna connector will work in any case, as long as the cable can reach the booster board)
![338014176-7903fb15-44de-485e-b4e8-a11b95d597a6](https://github.com/user-attachments/assets/ab5e3f54-3dbd-407e-a990-9c0f7c805b95)

## Secure everything
9) glue with the siliconic glue the booster board to the piece of aluminum between the GPS antenna and the obstacle avoidance sustem sensors cluster
![338014191-0cf86dd7-0990-4a75-bb7f-b0593a43f2f9](https://github.com/user-attachments/assets/fe16bee5-c781-47db-b6e7-0b92493f2129)
![338014202-ce52ea50-1f77-40a8-8729-f0c561dd3514](https://github.com/user-attachments/assets/c3c859e9-9023-474b-a12a-b78a3b6776f4)
NOTE: you cannot see it from the picture, but I did install a thin heatsink (the one you get from NLD) below the booster board.
