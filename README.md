# STM32-USB-Microphone-Interface
USB Audio Class Device with STM32G431CB and TLV320ADC6120


<img src="Assembled PCB Picture.jpg" alt="Assembled PCB" width="400"/>

The PCB is working, but not fully verified since the I2C + I2S driver for TLV320ADC6120 haven't been written yet.

Some changes needed to be made to the STM32 board, for revision B:
 - Move all components to the top of the board, so it could be reflowed at once
 - Change the USB-C connector to a more popular and cheaper one
 - RST button have the wrong footprint, missing the positioning hole
 
Software development:
| Task                                                        | Status      | Finished?                                                                       |
|-------------------------------------------------------------|-------------|---------------------------------------------------------------------------------|
| Setup STM32G431 as a USB Audio Class Device in STM32CubeIDE | in progress | <ul><li>[x] USB could connect to PC </li><li>[ ] USB microphone mode </li></ul> |
| TLV320ADC6120 I2C Control                                   |             |                                                                                 |
| TLV320ADC6120 I2S transfer with DMA                         |             |                                                                                 |
