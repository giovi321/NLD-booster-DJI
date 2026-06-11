# Installing the NLD booster board on a DJI RC2

This guide also applies to the DJI RC. Disassembly is not covered here. [This video](https://youtu.be/dhpUh3fc1Z8) was made for the RC but works for the RC2 as well.

## Tools needed

- Soldering iron with a thin tip, capable of reaching 370°C
- Thermally conductive, electrically insulating silicone adhesive (something like this):

<img src="https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9" width="300">

- Multimeter
- Hex and Phillips screwdrivers
- Optional but useful: plastic pry tools for opening electronics:

<img src="https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5" width="300">

## Before you start

- Protect all solder joints with thermally conductive, electrically insulating silicone adhesive.
- Use hot glue on antenna connections so they are easy to remove later.
- Fit heatsinks on both boards. The NLD-supplied ones work; better options are on Amazon.
- Signal cables must not run over or under the booster board.

## Installation

With the remote disassembled, carefully remove the fan assembly and aluminum heatsink without disturbing the thermal paste on the heatsink.

### Step 1: Connect power

The easiest access to power is the left battery (orient yourself with the antennas facing up). Right next to the battery connector are two small pads: one square, one circular. Solder positive and negative to these pads, connect to the step-up converter, and cover with silicone adhesive. The pads are not masked, so no scraping is needed.

<img src="https://github.com/user-attachments/assets/84bd62b7-80bc-459f-bac5-7fd410ec257c" width="600">

Connect the EN pin of the step-up converter to the top-most pin of the ribbon connector for the C1/C2 buttons on the back of the remote. Solder and cover with silicone adhesive.

<img src="https://github.com/user-attachments/assets/02a135ea-abfc-440f-873a-d80f987c154f" width="600">

### Step 2: Connect the antenna

From testing, the choice of antenna makes no measurable difference. I used one of the external antennas because I am planning to add SMA connectors later for interchangeable externals.

There is a cable length problem to solve first. The right antenna's cable is too short to reach the booster board, which mounts on the left side of the fan. The left antenna is labeled "G" and appears to be the GPS antenna, so it cannot be used for the booster.

The solution is to swap the two external antennas. Disconnect both (labeled "G" and "ANT0") from the PCB, remove them from the body with pliers, and reinstall them on opposite sides. The right antenna goes into the left slot and vice versa. When reinserting, pay attention to orientation. The antennas do not rotate 360 degrees and will only slide into the hole correctly when aligned properly.

<img src="https://github.com/user-attachments/assets/417ba36e-a6c6-4ae3-bb7c-2bb3994f88dd" width="600">

Connect the cable of the antenna now on the left side to the booster board and finish all the power connections.

### Step 3: Physical modifications

Cut the piece of plastic shown below from the back of the remote body to make room for the booster board.

<img src="https://github.com/user-attachments/assets/1b31d383-5dac-4663-8fc0-633d96ce6103" width="600">

Cut the piece shown below from the fan duct assembly. This improves airflow and also prevents the board from covering a screw once it is glued to the heatsink, which would make future disassembly impossible.

<img src="https://github.com/user-attachments/assets/ea0df4d9-483e-4115-a9bc-a2cf22d3167d" width="600">

### Step 4: Secure the board

Wrap the step-up converter in heat shrink tubing and place it near the buzzer at the top of the remote.

Glue the booster board to the aluminum heatsink in the section not covered by the fan assembly, using thermally conductive silicone adhesive. Signal cables must not run over the booster board.

<img src="https://github.com/user-attachments/assets/5e6bb913-2738-49b2-88ac-fa55c516e083" width="600">

## Optional: add a dedicated cooling fan

After several weeks of use, I fitted an additional fan and the thermal performance improved noticeably. The booster module runs better with active cooling.

The fan I used is a 1703 blower from SUNON (available on AliExpress), paired with a 15x15x4mm heatsink. It fits the space well and draws only 35mA.

<img src="https://github.com/user-attachments/assets/49606fb3-6f73-40b4-97c7-34e063005d63" width="600">

I designed a 3D-printable mount for the fan. It is not strictly necessary but makes the installation much easier. I printed mine in TPU, which is more forgiving on tolerances when closing the remote back up.

[Fan support STL file](https://github.com/giovi321/NLD-booster-DJI/blob/main/Fan%20support%20for%20DJI%20RC2_v2.stl)

**Installation:**

1. Remove the screw holding the original fan and heatsink in place, fit the printed mount, and screw everything back together.
2. Use cyanoacrylate to glue the fan to the mount.

<img src="https://github.com/user-attachments/assets/035c136f-be91-4494-b592-450a0823810c" width="600">

3. Apply two strips of silicone adhesive to the heatsink surface. These serve two purposes: they lift the booster board slightly to allow airflow underneath, and they hold the board in place under the pressure of the back cover when the remote is closed.

<img src="https://github.com/user-attachments/assets/f78de367-cee7-4902-9fcb-1bfe56799720" width="600">

4. Stick the heatsink to the back of the booster board at the top-left corner.

<img src="https://github.com/user-attachments/assets/51fc7ce0-e61c-4bdb-8cc4-44f23ebba711" width="600">

5. Connect the fan ground (black wire) to the ground output of the step-up converter.
6. Connect the fan 3.3V supply (red wire) to the EN pin of the step-up converter. The EN pin provides a 3.3V signal and 35mA is low enough that drawing from it causes no problems.
7. Place the booster board on the two silicone adhesive strips and close the remote.

<img src="https://github.com/user-attachments/assets/f9fc1608-46f9-4fcd-8e62-9ebfd2d92c7b" width="600">

The fan turns on as soon as the remote powers up. It is audible, but the cooling benefit is real.
