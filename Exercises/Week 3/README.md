# Blinky Function

## Board
STM32429I Discovery board (class board)

## Environment 
STM32CubeIDE

## Assignment

Make an LED on the board blink with a given delay and add button functionality to toggle the LED on or off. Bonus points for making the button via an interrup
and even more for debouncing the button.

## Implementation 

The implementation of this function can be seen in the included files. The main.c file contains the code to call the HAL functions in order to toggle the pin 
as well as add the delay between the pin toggles in the while loop. There main.h file contains the initialization of the pin using the existing HAL provided
for the board. These make it easy to change the pins linked to the LED as referenced by the manual. 

After speaking with a mentor during office hours, I was able to figure out a method to implement the push button interrupt using the generation from the .ioc file. After digging around in the stm32f4xx_it.c file I was able to find the interrupt handler and use the void HAL_GPIO_EXTI_Callback(uint16_t GPIO_Pin) function which is called by the interrupt handler. There I implemented code that would set the LED pin off and then toggle a variable used to keep track of the button state called B1State. Code can be found in the [Blinky/Core/Src](https://github.com/brhe4981/MakingEmbeddedSystemsClass/tree/main/Blinky/Core/Src) directory. 


- What are the hardware registers that cause the LED to turn on and off? (From the
processor manual, don’t worry about initialization.
  - The registers the change the LED pin status can be found in the manual under GPIO_PIN_13. If you follow this definition with a ctrl+Click in cubeIDEyou get the stm32f4xx_hal_gpio.h file which has the following as its definition. 
    - #define GPIO_PIN_13                ((uint16_t)0x2000)  /* Pin 13 selected   */  
- What are the registers that you read in order to find out the state of the button?
  - According to the manual under the pin PA0 and using the HAL we can see that the register for the button is GPIO_PIN_0. 
- Can you read the register directly and see the button change in a debugger or by printing out the value of the memory at the register’s address?

