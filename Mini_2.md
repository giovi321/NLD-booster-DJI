# Installing the NLD booster board on a DJI Mini 2

Disassembly is not covered here. [This video](https://www.youtube.com/watch?v=C_9mIduaoMY) covers both the drone and remote.

## Tools needed

- Soldering iron with a thin tip, capable of reaching 400°C
- Thermally conductive, electrically insulating silicone adhesive (something like this):

<img src="https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9" width="300">

- Multimeter
- Phillips screwdrivers
- Sharp blade
- 120-grit sandpaper
- Metal pry tool to use as a sanding block:

<img src="https://github.com/user-attachments/assets/a5628589-9d4c-4091-a76e-7ce5e8a4b9c8" width="300">

- Optional but useful: plastic pry tools for opening electronics:

<img src="https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5" width="300">

## Additional parts needed

- 15cm female IPEX4 to female IPEX4 extension cable (available on AliExpress)
- 14x15x4mm heatsink (available on Amazon)

## Before you start

- Protect all solder joints with thermally conductive, electrically insulating silicone adhesive.
- Use hot glue on antenna connections so they are easy to remove later.
- Fit heatsinks on both boards. The ones included in the NLD kit work, but better options are available on Amazon.
- Battery connector pads need scraping with a blade before solder will stick.
- Signal cables must not run over or under the booster board. The interference can heavily degrade signal. The pictures do not always show this correctly. Do it right regardless.

## Installation

### Step 1: Cut the heatsink window

With the drone disassembled, use a cutter to cut a square opening in the top cover, sized to match the heatsink exactly.

<img src="https://github.com/user-attachments/assets/4a1d6f11-0854-4d29-b4c1-a749dd821f3f" width="600">

Use the metal pry tool with sandpaper attached to clean up the edges and get the fit right.

<img src="https://github.com/user-attachments/assets/a5628589-9d4c-4091-a76e-7ce5e8a4b9c8" width="300">

Stick the heatsink to the booster board, then glue the booster board to the inside of the top cover using silicone adhesive, so the heatsink sits flush in the opening.

<img src="https://github.com/user-attachments/assets/53906b2d-94e9-4407-aa70-8838d3d70f40" width="600">

The result should look like this:

<img src="https://github.com/user-attachments/assets/9dfbc7b9-6510-49aa-923b-9ef517b7b28a" width="600">

### Step 2: Mount the step-down module

Stick the step-down board to the plastic shell at the rear of the drone. Do not place it on top of the GPS antenna, which is the large component highlighted in red in the picture below.

<img src="https://github.com/user-attachments/assets/0cecb7ab-bf3f-4b33-af66-e859a5f7d1c0" width="600">

### Step 3: Connect power

Remove the core board to access the ESC board. Connect the step-down module to the three pads shown below:
- GREEN: ground (black wire)
- RED: positive (red wire)
- YELLOW: EN pin

<img src="https://github.com/user-attachments/assets/7f5fb054-110d-4afb-b4ef-71cfbe75bf7d" width="600">

What the board looks like installed on the drone:

<img src="https://github.com/user-attachments/assets/93be2b71-102c-41a2-9bc6-62b31e5b7165" width="600">

For the battery connector pads (green and red), scrape them with a blade first and use 400°C. The solder mask is stubborn.

### Step 4: Connect the antennas

The internal antenna cable running through the drone is too long once the booster is installed. Replace it with the new 15cm IPEX4 female-to-female cable, routed through the exact same path as the original (shown as the green line below).

<img src="https://github.com/user-attachments/assets/7f7865cb-b596-47e9-903d-9b92d9eed730" width="600">

Then:
- Connect the "ANT" connector on the booster board to the grey cable coming out of the drone arm. That cable is the external antenna.
- Connect the remaining IPEX1 connector on the booster board to the core board using the new 15cm cable.

Signal cables must not run over or under the booster board.
