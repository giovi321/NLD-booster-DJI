# Installing the NLD booster board on a DJI Air 3

Disassembly is not covered here. [This video](https://www.youtube.com/watch?v=8k8JhMTr9xc) is a good starting point.

---

## Tools needed

- Soldering iron with a thin tip, capable of reaching 400°C
- Thermally conductive, electrically insulating silicone adhesive (something like this):

![immagine](https://github.com/user-attachments/assets/2a0a0e62-e4f0-48af-b45c-07f20505b6b9)

- Multimeter
- Torx and Phillips screwdrivers
- Sharp blade to scrape solder mask off PCB pads
- Optional but useful: plastic pry tools for opening electronics:

![338014083-f758fa75-01d6-4dda-90e6-f5000c77d285](https://github.com/user-attachments/assets/3a104caa-c078-41a8-82ae-4bfe9642fcd5)

---

## Before you start

- Protect all solder joints with thermally conductive, electrically insulating silicone adhesive.
- Use hot glue on antenna connections so they are easy to remove later if needed.
- No heatsink is needed on the Air 3. The drone's cooling fan sits directly above where the booster module mounts, so airflow handles it in flight.
- The battery connector pads on the core board are covered with solder mask. Scrape them with a blade before attempting to solder.
- Route signal cables so they do not pass over or under the booster board. Interference from the board can heavily degrade signal.

---

## Installation

### Step 1: Remove the core board

Disassemble the bottom of the drone to expose the core board. The gimbal does not need to come out.

Remove the glue holding the antenna connectors in place. Squeeze the hardened glue gently with pliers to separate it from the connectors without putting stress on the connectors themselves. Do not pull directly on the connectors.

![foto_no_exif(1)](https://github.com/user-attachments/assets/b98966f8-7d5b-4038-8a80-1fef0f7638d7)

Use pliers to unplug each connector by applying upward leverage from underneath.

![foto_no_exif(2)](https://github.com/user-attachments/assets/c71a6043-26e2-4c75-b22e-184b212492f2)

Remove all core board screws and lift the board out.

![foto_no_exif(3)](https://github.com/user-attachments/assets/130bbc12-a3ea-4a15-a42b-aaf43bf2156e)

### Step 2: Connect power

Solder the step-down module to the booster board.

![](https://github.com/user-attachments/assets/409bc8cc-ae49-412a-9cb9-6c166be928df)

Identify the battery connector pads. You need the first and the last connector (polarity shown in the picture: black = negative, red = positive).

![foto_no_exif(4)](https://github.com/user-attachments/assets/bf16d1da-f116-4c71-8c1c-f1fe4130b839)

Scrape the pads with a blade to expose clean metal. At 350°C, with some patience, the solder will bond. Do not overheat. Cover the finished joints with silicone adhesive.

Solder the battery wires to the step-down module.

![foto_no_exif(5)](https://github.com/user-attachments/assets/0c63f580-1de2-484b-a148-c053f0dd5176)

### Step 3: Mount the booster and step-down modules

Optional but worth doing: cut a square of metal from a plastic pry tool and glue it to the drone's plastic body beneath the cooling fan, then cover it with Kapton tape. This gives a better thermal surface.

Apply silicone adhesive to the area of the drone body directly below the cooling fan.

![foto_no_exif(6)](https://github.com/user-attachments/assets/35575cca-f687-4f05-840f-9f5d7b55a5f5)

Press the step-down module and booster module into the adhesive. Two things to keep in mind:
- The booster module should sit as close to the gimbal as possible.
- Leave enough space between the step-down module and the booster module so the fan's foam seal can fit between them.

![foto_no_exif(7)](https://github.com/user-attachments/assets/4944c193-3039-488d-8ac9-6fa60ef5a142)

### Step 4: Connect the antenna

From testing, no antenna consistently outperforms the others. I used the black antenna cable marked "1" on the core board.

![core](https://github.com/user-attachments/assets/6374ee86-3844-42e6-9782-c8d55e173c71)

Connect that cable to the "ANT" connector on the booster board.

![foto_no_exif(8)](https://github.com/user-attachments/assets/95d6454d-f04f-4846-a622-0f5dcd262b3a)

Connect the IPEX cable included with the booster board to the other connector on the booster board. Route it around the board without crossing it and let the free end hang on the same side of the drone as the other antenna cables (follow the red line in the picture).

![FG001 02_26 137](https://github.com/user-attachments/assets/d8769aa9-58b3-496c-aba3-84160836bcee)

### Step 5: Reassemble

Put the core board back in place. Before closing up:
- Make sure signal and antenna cables do not cross the booster board.
- Reconnect all ribbon cables.
- Reconnect all antenna cables except the one plugged into the booster board.
- Connect the free end of the IPEX cable from the booster board to the empty connector on the core board, the one marked "1".

![foto_no_exif(10)](https://github.com/user-attachments/assets/069fc85e-91e2-48e2-8ec1-605d234bc22a)

---

## Results

A quick RF meter test confirms the booster works well:
- Left reading: boosted antenna output, **-27.8 dBm**
- Right reading: unboosted antenna output, **-41.2 dBm**

![Untitled](https://github.com/user-attachments/assets/cc67ea3c-6716-4f4d-85e5-c14075558d40)
