# 3D-printable cases for external booster module installation

These cases let you mount the booster module and step-down module on the outside of the drone, typically velcroed to the top. Use them when there is no room to fit the booster internally.

All cases should be printed in ABS. It handles heat better than PLA, which matters here since the booster module generates real heat under load.

## Requirements common to all cases

- Velcro strap to attach the case to the drone
- 2mm neoprene strips
- Female IPEX4 to female IPEX4 cable, 10-15cm (available on AliExpress)
- A small amount of silicone to seal the cable entry holes

Plastic cases also need:
- 4x M2x4x3.2 threaded inserts
- 4x M2x6 screws
- Raspberry Pi-style heatsinks (available on [AliExpress](https://www.aliexpress.com/item/1005007485448259.html) or [Amazon](https://www.amazon.com/dp/B07YR6M6F6/)):
  - 4x 14x14mm heatsinks
  - 1x 14x9mm heatsink

## Available cases

### Plastic case

The simplest option. Designed primarily for the DJI Mini 2 but compatible with any drone.

[Plastic case STL](https://github.com/giovi321/NLD-booster-DJI/blob/main/Cases%203D/NLD%20booster%20board%20plastic%20case_v3.stl)

<img src="https://github.com/user-attachments/assets/c3276901-b6b7-48af-9ffa-fde8e1c11226" width="600">

### Plastic case with built-in battery

If you do not want to solder anything to the drone, this is the option. The battery inside the case powers the booster independently.

[Plastic case with battery STL](https://github.com/giovi321/NLD-booster-DJI/blob/main/Cases%203D/NLD%20booster%20board%20plastic%20case%20battery_v1.stl)

Additional parts needed:
- USB Type-C female breakout board (available on [AliExpress](https://www.aliexpress.com/item/1005004861928502.html))
- 403040 LiPo 3.7V battery, at least 500mAh

<img src="https://github.com/user-attachments/assets/46fcf1c1-53d0-4343-a430-d2a142426b7d" width="600">

### Aluminum case

The most capable option. Fully waterproof, with the heatsink built into the case walls, so no separate heatsink is needed. It does need to be CNC machined or metal 3D printed, which costs more than plastic.

Apply thermal paste or thermal adhesive to bond the booster board to the inside of the case.

[Aluminum case STL](https://github.com/giovi321/NLD-booster-DJI/blob/main/Cases%203D/NLD%20booster%20board%20aluminum%20case_v2.stl)

<img src="https://github.com/user-attachments/assets/0c993181-0589-4907-988d-66ec8918444a" width="600">
