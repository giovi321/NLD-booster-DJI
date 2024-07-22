# Intro
My approach to installing the NLD booster board on a DJI RC2. Should work almost the same on the DJI RC.

NOTE: i am not going to explain how to disassemble the remote, you can easily find video on youtube such as those:
- Instructions for the DJI RC, that works also for RC2: https://youtu.be/dhpUh3fc1Z8?feature=shared

# Tools needed (bare minimum)
- A decent soldering iron with a thin tip and capable of reaching 370 celsius
- Siliconic non electrically conductive but heat condictive siliconic glue such as this one:
![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter to check for polarity and connections
- Hexagonal and phillips screwdrivers
- Optional but highly recommended: some cheap tools to open electronic devices such as these: 
![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

# General recommendations for the installation
- Use siliconic non electircally conductive but heat conductive glue to protect all new solder joints
- Use hot glue to stabilize antenna connections, so its easier to remove if you ever need to
- Use some heatsinks: the ones provided by NLD are decent but not the best (even though I have succesfully used them, on amazon you can easily find better solutions). Both the boards need a heatsink: in my explanation I didnt say it but I did use the heatsibks on both devices. 

# Installing the booster on the RC2
Once you have disassembled rhe remote, carefully remove the fan assembly and the aluminum heatsink without touching the thermal conductive paste

## Connect to power
1) I found that the easiest access to power is through the left side battery (keep the antennas facing up to orient yourself), using the two little pads (one is squared and the other is a cirle) just right next to the battery connector.
Solder the positive and negative and connect to the step-up voltage coverter and cover the connection with siliconic glue. There is no need to scrape the pads as they are not covered by PCB mask. 
![338014222-1144d95c-4b53-4d06-9aa7-2db23c76e58d](https://github.com/user-attachments/assets/84bd62b7-80bc-459f-bac5-7fd410ec257c)

2) connect the EN pin of the step-up voltage converter to the first top-most pin of the ribbon connector of the C1 and C2 buttons on the back of the remote that you have now separated already. Solder and cover with siliconic glue
![338014233-d6538b95-d831-4211-81aa-60e8f58ce8e2](https://github.com/user-attachments/assets/02a135ea-abfc-440f-873a-d80f987c154f)


## Connect the antenna
After several trials and tests I understood that using one or another antenna makes absolutely no difference. I have chosen to use the external antennas as I am planning to upgrade the remote installing SMA connector to attach any external antenna I want.
However, if you want to use the external antenna, you'll need to do the following:
1) disconnect the two external antennas from the PCB (the ones identified with the labels "G" and "ANT0")
2) using pliers you can remove the two external antennas from the body of the remote and swap them (the right antenna will go on the left and vice versa) - be careful: the antennas do not rotate 360 degrees so when you insert them back in place you need to orient them correctly in order to be able to slide them into the hole

_We are doing this because the cable of the right antenna is too short to reach the booster board (which we will place on the left of the fan), and we cannot use the left antenna as it is identified by the label G so I suspect it is the GPS antenna which we dont need to boost (and it uses a different frequency so it would be useless to connect the booster board). I tried using the internal antenna identified by the label "ANT0" and I got still decent but poorer results compared to the right external antenna._

![338014242-f2bc9e08-3cb4-4564-bdf7-241a2d84e6b5](https://github.com/user-attachments/assets/417ba36e-a6c6-4ae3-bb7c-2bb3994f88dd)

3) Connect the cable of the antenna that is now on the left to the booster board and complete all the connections also for power

## Physical modifications to the body of the remote
1) cut off this piece of plastic from the back of the body of the remote to fit the board
![338014256-f35226de-ad03-4066-93e3-cf653aedede5](https://github.com/user-attachments/assets/1b31d383-5dac-4663-8fc0-633d96ce6103)

2) cut off this piece of plastic from the fan duct assembly (for two reasons: i) to improve airflow; ii) if you don't do it, once you glue the board to the heat sink, you will cover some screws and it won't be possible to disassemble the fan and heatsink)
![338014265-33c829ed-c83b-4500-8a85-00e149a86f4c](https://github.com/user-attachments/assets/ea0df4d9-483e-4115-a9bc-a2cf22d3167d)

## Secure the board
1) Using some heat shrink tube, protect the step-up voltage converter and place it somewhere on the top of the remote close to the buzzer
2) Using siliconic heat conductive glue, glue the booster board to the piece of aluminum heatsink that is not covered by the fan assembly
TIP: make sure that the signal cables do not run over the booster board as it could cause interferences and degrade the signal.

![338014279-9688204c-b10f-492b-966f-5c18c4167203](https://github.com/user-attachments/assets/5e6bb913-2738-49b2-88ac-fa55c516e083)

# Optional, but highly recommended: add a fan
After some weeks of testing, I have tried to install an additional fan to improve cooling. Infact, the booster module's performance increase notably with additional active cooling.
The fan I have chosen is a 1703 blower fan produced by SUNON (you can find it on AliExpress) together with a simple 15x15x4mm heatsink. It's not cheap but it's perfect for the job:
1) The size fits perfectly
2) The power consumption is only 35mA

![immagine](https://github.com/user-attachments/assets/49606fb3-6f73-40b4-97c7-34e063005d63)

I have designed a very simple 3D printable support for the fan which is not strictly necessary but it simplifies the installation process. I have printed it in TPU as it is more flexible and does not requires strict tolerances when closing the remote.
Here is the file: https://github.com/giovi321/NLD-booster-DJI/blob/main/Fan%20support%20for%20DJI%20RC2_v2.stl

Installation process.
1) Install the support by removing the screw that holds the original fan and heatsink in place and screwing everything back together
2) Use some cyanoacrylate (superglue) to stick the fan to the 3D printed support

![immagine](https://github.com/user-attachments/assets/035c136f-be91-4494-b592-450a0823810c)

4) Apply two strips of siliconic glue to the heatsink to support the booster board. We do this for two reasons: keep the booster board a lifted from the plastic and the heatsink to ease airflow and to secure it in place by simply using the pressure of the back cover of the RC (when the remote is closed up again).
![immagine](https://github.com/user-attachments/assets/f78de367-cee7-4902-9fcb-1bfe56799720)

5) Stick the heatsink to the back of the booster board, more specifically stick it to the top-left most corner
![immagine](https://github.com/user-attachments/assets/51fc7ce0-e61c-4bdb-8cc4-44f23ebba711)

6) Connect the ground (black wire) of the fan to the ground output of the step-up converter
7) Connect the 3.3vcc (red wire) of the fan to the EN pin of the step-up converter (yes, I know that we are getting the power of the fan from a signal line, but this is ininfluential as the power consumption is only 35mA)
8) Place the booster board on top of the two siliconic glue strips and close up the remote

![immagine](https://github.com/user-attachments/assets/f9fc1608-46f9-4fcd-8e62-9ebfd2d92c7b)

The fan now should turn on as soon as you turn on the remote. It's not very quiet, but the thermal benefits are incredibly good.
