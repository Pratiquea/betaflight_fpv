#Initial setup
## Flashing firmware
### Betaflight
### PX4 or ardupilot
both Px4 and ardupilot have an error message "no cpu load information" which fails the pre-arm flight check and thus makes it impossible to fly.

## Betaflight Setup
### Configure Ports
Note: All the connections referred here are for Holybro KakuteF7 flight controller. Betaflight version is 4.4.1.

![Port config image](/D/FPV/ports.png)

Hardware connections:

  * AKK infintite DVR is connected to **UART1**.
  * Radio receiver (RC) is connected to **UART6**.

In the ports tab of Betaflight configurator:

  * For the UART1 row, select under the peripherals dropdown -> "VTX(TBS SmartAudio)"
  * For the UART6, enable the Serial Rx to allow RC connection.


### Configure Video Transmitter settings
Notes for VTX and AKK DVR: The DVR supports **TBS SmartAudio V2.0** protocol
Follow the setup in [this youtube video.](https://www.youtube.com/watch?v=eaSmoOPk9KY&t=1s)

[Betaflight VTX-Tables github link](https://betaflight.com/docs/wiki/archive/VTX-Tables)