# NLD-booster-DJI
My approach to installing the No Limit Dronez booster board for DJI drones and remotes

Available guides:
Remote controllers:
- [DJI RC2](https://github.com/giovi321/NLD-booster-DJI/blob/main/RC2_and_RC.md) (applicable also to RC)
- [DJI RC-N1](https://github.com/giovi321/NLD-booster-DJI/blob/main/RC-N1.md)

Drones:
- DJI Air 3 (work in progress)
- [DJI Mini 4 Pro](https://github.com/giovi321/NLD-booster-DJI/blob/main/Mini_4_Pro.md)
- DJI Mini 2
  - [Internal installation](https://github.com/giovi321/NLD-booster-DJI/blob/main/Mini_2.md)
  - External installation (work in progress)

# Some knowledge you should have
The NLD booster board kit comes with the following content, when ordered for the devices listed in this repository
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
