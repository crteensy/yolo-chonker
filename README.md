# yolo-chonker
betaflight developer FC for the H735

The layout has 6 layers, and the decoupling is designed for oshpark's 6-layer stackup (see oshpark_6L_stackup.png)

- Format: 30x30 hole distance
- Battery voltage range: 2-6S
- 5V DCDC: LMR33620CRNXT
- 3V3: TPS62824
- Separate DCDC for HD out; LMR33620CRNXT set for 10V or 5V, configured with a solder jumper
- MCU: STM32H735
- peripherals that can be connected to the MCU with solder jumpers:
  - IMU: ICM-20602 and BMI270; dual gyro is possible
  - Flash: S25FL064L
  - Baro: DPS310
  - LEDs:
    - voltage rails LEDs: HD DCDC (5/10 V), 5V, 3V3
    - two standard LEDs for the FC
    - WS2812B including an output pad to attach more
  - battery voltage sensing
- SWD pads
- no analog OSD!
- no HD connector!
