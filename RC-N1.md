# Intro
My approach to installing the NLD booster board on a DJI RC-N1.

NOTE: i am not going to explain how to disassemble the RC, you can easily find video on youtube such as this: https://www.youtube.com/watch?v=pexzuVWaB08

# Tools needed (bare minimum)
- A decent soldering iron with a thin tip and capable of reaching 400 celsius
- Siliconic non electrically conductive but heat condictive siliconic glue such as this one:
![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter to check for polarity and connections
- Phillips screwdrivers
- Optional but highly recommended: some cheap tools to open electronic devices such as these:

![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

# Additional components needed
- NLD heatsink

# General recommendations for the installation
- Use siliconic non electircally conductive but heat conductive glue to protect all new solder joints
- Use hot glue to stabilize antenna connections, so its easier to remove if you ever need to
- Use some heatsinks: the ones provided by NLD are decent but not the best (even though I have succesfully used them, on amazon you can easily find better solutions). Both the boards need a heatsink: in my explanation I didnt say it but I did use the heatsinks on both devices. 
- Make sure that signal cables do not run over or below the booster board (not like I did in the pictures) as the interference could heavily degrade the signal


# Installing the booster on the RC-N1
Once you have taken the RC apart, you need to:
- remove the aluminum heatsink from the remote
- remove the transparent plastic cover and put it aside: we won't be re-installing it

## Connect to power 
Following the picture below, connect the step-up board to the available pads on the board of the remote:
- GREEN: VCC+ 5v (red wire) of the step-up module
- BLUE: ground (black wire) of the step-up module
- YELLOW: EN pin of the step-up module

![immagine](https://github.com/user-attachments/assets/bb0227ca-9b16-4045-8b64-0c5e091a1634)

## Connect the antenna
- Connect the white antenna cable to the IPEX1 connector on the booster board marked with the label "ANT"
- Connect the remaining IPEX1 connector on the booster board to the antenna connector on the board of the RC

![IMG_6662](https://github.com/user-attachments/assets/734dca86-97c7-49db-bf9e-16988ad8cccf)

## Fix everything inside the remote
- Using some heatshrink tube, isolate the step-up board
- Stick a NLD heatsink to the booster board, leaving about 8mm of the board free of the heatsink so that we can stick the booster board to the aluminum frame of the RC using siliconic glue

![immagine](https://github.com/user-attachments/assets/7d939e7d-a16c-41b9-8943-e01d8a31578d)

