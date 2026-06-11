# NLD booster board installation guides for DJI drones and remote controllers

Step-by-step guides for fitting a No Limit Dronez (NLD) signal booster board into various DJI drones and remote controllers. Each guide covers the wiring, placement, and physical modifications needed for that specific device.

---

## Disclaimer

- I am not affiliated with NoLimitDronez or any related entity. These guides are for informational purposes only.
- Everything you do based on this information is entirely at your own risk. I take no responsibility for damage, legal issues, or safety problems resulting from following these guides or modifying your devices in any way.
- Check your local laws before modifying or operating drones. In many jurisdictions, using a signal booster on a drone is regulated or prohibited.
- Read the safety rules below before you open anything.

---

## Safety rules

**Never power the booster without cooling.** In flight, the drone's airflow handles cooling automatically. On the bench there is no airflow, and the module will burn. Use a fan when bench testing.

**Never power the module without both signal connections in place.** The antenna output and the signal input must both be connected before powering on.

**Insulate every solder joint.** A bare joint shorting against the chassis at 120m altitude is not something you want to discover mid-flight.

**Use the right adhesive.** Several steps require thermally conductive, electrically insulating silicone adhesive. Using the wrong material can cause heat buildup or shorts.

**Handle IPEX connectors carefully, especially IPEX4.** They are very fragile and time-consuming to replace if damaged.

---

## Available guides

**Remote controllers**
- [DJI RC2](RC2_and_RC.md) (also applicable to the DJI RC)
- [DJI RC-N1](RC-N1.md)

**Drones**
- [DJI Air 3](Air_3.md)
- [DJI Mini 4 Pro](Mini_4_Pro.md)
- [DJI Mini 2](Mini_2.md)

**3D-printable cases for external mounting**
- [External installation cases](Cases%203D/readme.md) — use these if there is no room to fit the booster inside the drone

---

## What comes in the NLD kit

When ordered for the devices covered in this repo, the kit contains:

- 1x booster board for the remote (IPEX1 connectors)
- 1x booster board for the drone (IPEX4 connectors)
- 1x IPEX1 cable
- 1x IPEX4 cable
- 1x step-up module (converts any voltage above 1V to 5V)
- 1x step-down module (converts any voltage below 20V to 5V)

Other devices may need different connectors.

---

## How the installation works

The procedure is the same across all devices, though the order and specific details vary by device:

1. Solder the step-up or step-down board to the booster board (power connections only).
2. Connect the step-up or step-down board directly to the device's battery. Direct battery connection matters because a random PCB pad might show the correct voltage but not supply enough current.
3. Connect the EN pin of the step-up or step-down board to a 3.3-5V point that is only live when the device is powered on. This keeps the booster off when the device is off. On drones, this step is usually only needed if the battery connection point is always-on.
4. Connect the device's antenna to the "ANT" connector on the booster board. This is the signal output.
5. Connect the booster board's signal input to the drone or RC mainboard. This is the signal source the booster amplifies.

---

## License

The content of this repository is licensed under the [WTFPL](http://www.wtfpl.net/).

```
Copyright © 2024 giovi321
This work is free. You can redistribute it and/or modify it under the
terms of the Do What The Fuck You Want To Public License, Version 2,
as published by Sam Hocevar. See the LICENSE file for more details.
```
