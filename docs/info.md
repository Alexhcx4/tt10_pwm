<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This proyect generates a pwm output using a 4-bit input signal, at clk an external clock pulse is provided, it has a reset input pin.
The 4-bit assigned as sw, which is an abbreviation for switch, will be converted to a proportional duty cycle value (0-255).
Some of the possible combinations for the work cycle are 
sw=4´b0000; //sets the duty cycle to 0% (0/255)
sw=4´b0001; //sets the duty cycle to 6% (16/255)
sw=4´b0010; //sets the duty cycle to 13% (32/255)
sw=4´b0100; //sets the duty cycle to 25% (64/255)
sw=4´b1000; //sets the duty cycle to 50% (128/255)
sw=4´b1100; //sets the duty cycle to 75% (192/255)
sw=4´b1111; //sets the duty cycle to 94% (240/255)

AGREGA IMAGEN
MODULO/ENTIDAD

PWM EJEMPLO DIBUJO

## How to test

In this proyect we can get the PWM output signal by assigning values ​​to the 4-bit SW input, the RST input will reset the module.

IMAGEN TEST BENCH

## External hardware

A function generator will be useful for the CLK input, however, an integrated circuit can be connected to produce pulses at this input. 
An ocilloscope is needed to check and display the duty cycle that we will obtain in the PWM (pulse width modulation).

SEÑAL CUADRADA EN OSCILOSCOPIO
