<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

This is a 2-bit synchronous up counter made from two JK flip-flops wired as T flip-flops (each built in Wokwi as a D flip-flop plus an XOR gate). Both flip-flops share the same clock. Bit A (uo[0], LSB) toggles on every rising clock edge. Bit B (uo[1], MSB) toggles only when A is 1. The output counts 00, 01, 10, 11 and then wraps back to 00.

## How to test

Apply a clock signal to the clk pin, or press the Step button in the Wokwi simulation. Watch outputs uo[1] (B) and uo[0] (A). On each rising clock edge the count should go up by one (00, 01, 10, 11, 00). The outputs should not change on the falling edge. No inputs (ui) are used.

## External hardware

Two LEDs, one on uo[0] (A) and one on uo[1] (B), to display the count. No other external hardware is needed.
