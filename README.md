# NLD-booster-DJI
My approach to installing the No Limit Dronez booster board for DJI drones and remotes
Before attempting anything you **MUST** read the last chapter of this page.

## Available guides

Remote controllers:
- [DJI RC2](https://github.com/giovi321/NLD-booster-DJI/blob/main/RC2_and_RC.md) (applicable also to RC)
- [DJI RC-N1](https://github.com/giovi321/NLD-booster-DJI/blob/main/RC-N1.md)

Drones:
- [DJI Air 3](https://github.com/giovi321/NLD-booster-DJI/blob/main/Air_3.md)
- [DJI Mini 4 Pro](https://github.com/giovi321/NLD-booster-DJI/blob/main/Mini_4_Pro.md)
- [DJI Mini 2](https://github.com/giovi321/NLD-booster-DJI/blob/main/Mini_2.md)
  - Alternative: external installation (work in progress)

## Cases for external installation
If you don't have space to mount the booster board internally to your drone, you can opt to use one of the cases deigned specifically for this purpose.

[3D printable cases for NLD booster board](https://github.com/giovi321/NLD-booster-DJI/tree/main/Cases%203D)

# ❗❗ Some knowledge you should have before attempting the installation

**DOs and DON'Ts before the installation:**
- **DO NOT** power on the booster module without proper cooling (active or passive)
  - When the drone is in flight, the airflow cools it down. When you are testing it. When you are testing it, there is absolutely zero cooling (unless you use a fan) and this will burn the module.
- **DO NOT** power on the module without input or output signal
  - This means that when you test the booster module you MUST connect the antenna (output) and the signal from the drone or remote (input)
- **DO** insulate all connections and solder joints
  - You don't want to see your drone falling from 120m because you did not insulate properly a solder joint
- **DO** make sure that you have all the right tools and consumables
  - In the guides it is reported multiple times to use a good quality thermal conductive and electrically insulating glue
- **DO** be very careful when handling ipex connectors (especially ipex4)
  - These are extremely fragile and very paiful to replace (if not impossible) 

The NLD booster board kit comes with the following content, when ordered for the devices listed in this repository (other drones and remotes might require different connectors)
- 1x booster board for the remote (with IPEX1 connectors)
- 1x booster board for the drone (with IPEX4 connectors)
- 1x IPEX1 cable
- 1x IPEX4 cable
- 1x step-up module (a tiny board that converts voltage from anything above 1 volt to 5 volts)
- 1x step-down module (a tiny board that converts voltage from anything below 20v to 5 volts)

The procedure is always the same, maybe I show it in different order but the steps are the following:
1) Connect the step-up or step-down board to the booster board (just the positive and negative cables)
2) Connect the step-up or step-down board to the battery of the device (aways connect directly to the battery or at least make sure that the pad you're connecting it to is dicrectly connected to the battery. That's because the PCB of the device, in the point you have randomly chosen, might give you the correct voltage but not enough power)
3) Connect the EN pin of the step-up (or step-down) board to a 3.3-5.0 volt source that is turned ON only when the device is powered ON. We do this because we want the booster board to have power only when the device is turned on, and if we connect directly to the batteries we have constantly power. So the EN pin tells to the board "now it's time to enable your 5.0v output". Thi is typically needed on the RC only, but some drone batteries have different connection points (that could be always enabled) so we need the EN pin also on the drone.
4) Connect the antenna of the device to the booster board on the connector marked with "ANT" (this is basically the signal "output")
5) Connect the booster board signal input to the board of the drone or RC, this is the source of signal for the booster board which will boost the signal and transmit it to the output

# License
The content of this repository is licensed under the [WTFPL](http://www.wtfpl.net/).

```
Copyright © 2024 giovi321
This work is free. You can redistribute it and/or modify it under the
terms of the Do What The Fuck You Want To Public License, Version 2,
as published by Sam Hocevar. See the LICENSE file for more details.
```
