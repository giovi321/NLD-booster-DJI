# Intro
My approach to installing the NLD booster board on a DJI Air 3.

NOTE: i am not going to explain how to disassemble the drone, you can easily find video on youtube such as this: [https://youtu.be/rLTtYpftaGs?feature=shared](https://www.youtube.com/watch?v=8k8JhMTr9xc)

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
- Heatsink not needed on the Air 3 as the fan of the drone will be sitting right above the booster module (soon I will publish temperature measurements with the drone in flight)
- the battery connectors on the drone need to be scraped with a blade in order to be able to solder onto them
- Make sure that signal cables do not run over or below the booster board as the interference could heavily degrade the signal


# Installing the booster on the Mini 4 Pro
Once you have taken the drone apart, you need to follow these steps

## Connect power
1) Disassemble the bottom part of the drone and expose the core board. There is no need to disassemble the gimbal
2) Solder the step-down module to the booster board
![](https://github.com/user-attachments/assets/409bc8cc-ae49-412a-9cb9-6c166be928df)
3) Remove the glue holding the 6 antennas connector in place. I recommend to use some pliers and squeeze the hard glue to gently separate it from the connectors and board. Do not pull as this will damage the connectors
![foto_no_exif(1)](https://github.com/user-attachments/assets/b98966f8-7d5b-4038-8a80-1fef0f7638d7)
4) Very carefully unplug the connectors using pliers, applying a leverage from underneath the connector
![foto_no_exif(2)](https://github.com/user-attachments/assets/c71a6043-26e2-4c75-b22e-184b212492f2)
5) Remove all the screws on the core board and remove it
![foto_no_exif(3)](https://github.com/user-attachments/assets/130bbc12-a3ea-4a15-a42b-aaf43bf2156e)
6) Identify the battery connectors to which you will be soldering the black and red wire of the step-down module
- You will need the first and last connector (see picture for polarity: black = negative, red = positive)
- Using a sharp blade, scratch the connectors to remove the masking from the PCB so that you can solder the wires - it will take quite some time to make the solder stick to those pads, don't over heat it (350 celsius should fine) and if it does not work just keep scraping them with a blade
- Cover the soldered joints with siliconic glue. In the picture, I did solder the cables and covered them with siliconic glue already before taking the picture.
![foto_no_exif(4)](https://github.com/user-attachments/assets/bf16d1da-f116-4c71-8c1c-f1fe4130b839)
7) Solder the cables connected to the battery connector to the step-down module
![foto_no_exif(5)](https://github.com/user-attachments/assets/0c63f580-1de2-484b-a148-c053f0dd5176)

## Secure the booster and step-down modules
8) Optional: in order to protect the drone and improve heat dissipation, you can cut a square piece of metal from one of the disassebly tools mentioned in the "Tools needed" chapter of this text. Stick it with glue to the plastic part of the drone and cover the metal with Kapton tape.
9) Spread some siliconic glue on the part of the drone below the cooling fan like in the picture
![foto_no_exif(6)](https://github.com/user-attachments/assets/35575cac-f687-4f05-840f-9f5d7b55a5f5)
10) Stick the step down module and the booster module on the glue making sure that:
- The booster module is as close as possible to the gimbal
- The step-down module is distanced enough from the booster module to allow the foam/sponge parte of the fan to separate the two modules
![foto_no_exif(7)](https://github.com/user-attachments/assets/4944c193-3039-488d-8ac9-6fa60ef5a142)

## Connect the antenna
11) Now it's time to connect the signal and antenna cables to the board
- There is no antenna that works better than the others according to my empirical testing
- For convenience, I have used the black antenna cable that on the core board of the drone is marked as "1" (see picture below)
![core](https://github.com/user-attachments/assets/6374ee86-3844-42e6-9782-c8d55e173c71)
- Connect the black cable to the booster board to the connector marked with "ANT" on the booster board
![foto_no_exif(8)](https://github.com/user-attachments/assets/95d6454d-f04f-4846-a622-0f5dcd262b3a)
- Connect the black ipex cable that came with the booster board to the other connector of the booster board, route it around the board without overlapping it and leave the cable hanging on the side of the drone where the other antenna cables are hanging (basically follow the red line shown in the picture below)
![FG001 02_26 137](https://github.com/user-attachments/assets/d8769aa9-58b3-496c-aba3-84160836bcee)
12) Now you are ready to put the core board back in place:
- make sure that the signal and antenna cables do not overlap the booster board
- reconnect all the ribbon cables
- reconnect all the antenna cables except for the black cable that we plugged in the booster board
- connect the black ipex cable that came with the booster board to the empty connector on the core board (the one marked as "1" mentioned in the step 11)
![foto_no_exif(10)](https://github.com/user-attachments/assets/069fc85e-91e2-48e2-8ec1-605d234bc22a)
