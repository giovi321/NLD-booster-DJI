# Installing the NLD booster board on a DJI RC-N1

Disassembly is not covered here. [This video](https://www.youtube.com/watch?v=pexzuVWaB08) is a good starting point.

---

## Tools needed

- Soldering iron with a thin tip, capable of reaching 400°C
- Thermally conductive, electrically insulating silicone adhesive (something like this):

![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter
- Phillips screwdrivers
- Optional but useful: plastic pry tools for opening electronics:

![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

---

## Additional parts needed

- NLD heatsink

---

## Before you start

- Protect all solder joints with thermally conductive, electrically insulating silicone adhesive.
- Use hot glue on antenna connections so they are easy to remove later.
- Fit a heatsink on the booster board. The NLD-supplied one works fine.
- Signal cables must not run over or under the booster board.

---

## Installation

With the RC disassembled:
- Remove the aluminum heatsink from the remote.
- Remove the transparent plastic cover and set it aside. It does not go back in.

### Step 1: Connect power

Solder the step-up module to the RC board using the three pads shown below:
- GREEN: positive 5V output (red wire of the step-up module)
- BLUE: ground (black wire of the step-up module)
- YELLOW: EN pin

![immagine](https://github.com/user-attachments/assets/bb0227ca-9b16-4045-8b64-0c5e091a1634)

### Step 2: Connect the antenna

- Connect the white antenna cable to the "ANT" connector on the booster board.
- Connect the remaining IPEX1 connector on the booster board to the antenna connector on the RC board.

![IMG_6662](https://github.com/user-attachments/assets/734dca86-97c7-49db-bf9e-16988ad8cccf)

### Step 3: Secure everything

- Wrap the step-up board in heat shrink tubing to insulate it.
- Fit the NLD heatsink to the booster board, leaving about 8mm of board exposed at one end. That exposed section is what gets glued directly to the aluminum frame of the RC.

![immagine](https://github.com/user-attachments/assets/7d939e7d-a16c-41b9-8943-e01d8a31578d)
