# Installing the NLD booster board on a DJI Mini 4 Pro

Disassembly is not covered here. [This video](https://youtu.be/rLTtYpftaGs?feature=shared) is a good reference.

---

## Tools needed

- Soldering iron with a thin tip, capable of reaching 400°C
- Thermally conductive, electrically insulating silicone adhesive (something like this):

![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter
- Torx and Phillips screwdrivers
- Sharp blade
- Optional but useful: plastic pry tools for opening electronics:

![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

---

## Before you start

- Protect all solder joints with thermally conductive, electrically insulating silicone adhesive.
- Use hot glue on antenna connections so they are easy to remove later.
- Fit heatsinks on both boards. The NLD-supplied ones work fine; better options are on Amazon.
- Battery connector pads need scraping before solder will stick.
- Signal cables must not run over or under the booster board.

---

## Installation

### Step 1: Access the battery connector

Remove the main board and obstacle avoidance cameras from the top of the drone.

Remove the three Torx screws holding the battery connector PCB in place. You do not need to remove the connector entirely. With the obstacle avoidance cameras out, push the small battery connector PCB up slightly from above using tweezers. On the back of that PCB, peel up the adhesive plastic layer to expose the connector pads.

### Step 2: Solder to the battery connector

Scrape the connector pads with a blade to remove the solder mask. At 350°C, with some patience, the solder will bond. Do not overheat. Solder wires to the correct pads following the Mini 4 Pro battery pinout:

![338014364-85232647-8a49-44d1-b3a3-88f20bb655ff](https://github.com/user-attachments/assets/857ae314-c66a-4ed5-8d86-c96ad2aab921)

Cover the finished joints with thermally conductive silicone adhesive.

### Step 3: Wire the step-down converter

Connect the step-down converter to the battery wires and to the booster board.

Connect the EN pin of the step-down converter to the inductance labeled "2R2" as shown below, then cover with silicone adhesive.

![338014131-4d84ec24-1892-418b-a313-3f99b1996834](https://github.com/user-attachments/assets/eb515ecb-e488-45f1-8e90-4fd73c0442b4)

Glue the step-down converter to the top of the obstacle avoidance sensor cluster using silicone adhesive.

![338014160-6e45433c-1c5e-4add-b2a9-b0326a34729f](https://github.com/user-attachments/assets/0e1cde2b-e19f-41ef-a047-eeef397ace45)

### Step 4: Connect the antenna

Disconnect the antenna connector labeled "ANT0". It has the longest cable of the group, which makes it the easiest to route to the booster board. Any antenna connector will work as long as the cable can reach.

![338014176-7903fb15-44de-485e-b4e8-a11b95d597a6](https://github.com/user-attachments/assets/ab5e3f54-3dbd-407e-a990-9c0f7c805b95)

Connect the ANT0 cable to the booster board's signal input. Connect the booster board's "ANT" output to the core board connector that ANT0 was removed from.

### Step 5: Mount the booster board

Glue the booster board to the aluminum section between the GPS antenna and the obstacle avoidance sensor cluster, using silicone adhesive. The NLD-supplied heatsink goes under the booster board, between it and the aluminum surface.

![338014191-0cf86dd7-0990-4a75-bb7f-b0593a43f2f9](https://github.com/user-attachments/assets/fe16bee5-c781-47db-b6e7-0b92493f2129)
![338014202-ce52ea50-1f77-40a8-8729-f0c561dd3514](https://github.com/user-attachments/assets/c3c859e9-9023-474b-a12a-b78a3b6776f4)
