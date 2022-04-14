# Board Comparison
## Project Board - STM32F429ZI

- What kind of processor is it?
  - STM32F429ZI arm cortex M4
- How much Flash and RAM does it have? Any other memory types?
  - 2MB of flash, 256KB of SRAM
- Does it have any special peripherals? (List 3-5 that you find interesting.)
  - 3-axis sensors MEMS
  - 2.4" QVGA TFT LCD Display
  - Camera interface for CMOS sensors
- If it has an ADC, what are the features?
  - Three 12 bit ADC, share 16 external channels
  - single shot or scan mode
  - Scan mode has automatic conversion for selected group of analog inputs
- How much does the board cost vs what the processor costs? Is the processor in stock
anywhere? (Try Digikey, Mouser, Octopart, Google, and so on.)
  - Board
    - ST: $29.30 in stock as of 04/01/2022
    - Digi-Key: $29.90 in stock as of 04/01/2022
    - Amazon: $76.99 in stock as of 04/01/2022
  - Processor
    - Digi-Key: $20.60 out of stock as of 04/01/2022
    - Mouser: $20.60 out of stock as of 04/01/2022
    - Avnet: $14.30 for 100 units out of stock as of 04/01/2022
    - Newark: $26.17 out of stock as of 04/01/2022

![Discovery Board HW BD drawio](https://user-images.githubusercontent.com/45643404/161367241-94014e1b-1f04-4a28-b240-cec32e057e90.png)


## Assigned Board - Teensy 4.0

- What kind of processor is it?
  -MIMXRT1062DVL6A ARM Cortex-M7
- How much Flash and RAM does it have? Any other memory types?
  - 2MB Flash, 1024K Ram, and 1K EEPROM
- Does it have any special peripherals? (List 3-5 that you find interesting.)
  - USB device and host at 480 Mbit/sec
  - Temperature sensor built in
  - Cryptographic accelaration from onboard HW
  - 32 general purpose DMA channels (Pixel Pipeline)
- If it has an ADC, what are the features?
  - Two ADC, 16 channels each, 20 in total
  - 14 pins for analog input
  - Default 10 bits of resolution but max of 12 bits is possible
  - 0-3.3v range
- How much does the board cost vs what the processor costs? Is the processor in stock
anywhere? (Try Digikey, Mouser, Octopart, Google, and so on.)
  - Boards
    - PJRC: $19.95 + s&h in stock as of 04/01/2022
    - SparkFun: $19.95 + s&h in stock as of 04/01/2022
    - Amazon: $21.97 in stock as of 04/01/2022
  - Processor (Current processor DVL6A discontinued, Used DVL6B for pricing)
    - AVNET: $8.30 for min order of 240 units
    - Digi-Key: $16.32 for 1 unit out of stock as of 04/01/2022
    - Mouser: $16.48 for 1 unit out of stock as of 04/01/2022

![Teensy Processor HWBD](https://user-images.githubusercontent.com/45643404/161365343-740bcbde-0189-4a6d-b5a6-bd9d7d9d4a6f.PNG)

