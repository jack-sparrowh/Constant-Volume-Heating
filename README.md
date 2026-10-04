# Constant-Volume-Heating
Constant Volume Heating of closed tank filled with liquid and nitrogen blanket.

It provides T-P values for isochoric heating. This can be useful when liquid level in blanketed tank is required for pressure relief device (PRD) sizing.

By providing initial parameters like temperature, pressure and liquid level as well as function of vapor pressure of liquid and function for density, python will output T-P data given specified final pressure in tank (set pressure of PRD).

It is assumed that isothermal compressibility of liquid is 0. The reason being that usually density functions for liquids do not provide pressure dependence (I have never seen one that does).

Main assumptions:
1. The isothermal compressibility is 0.
2. Rault's Law is applicable in all ranges of pressure and temperature.
3. Nitrogen is insoluble in liquid.
4. Ideal gas Law is aplicable to both nitrogen and liquid vapor.

Code is somewhat rough as I whipped it in short time as it is mostly a draft of an idea for future blog post.

Instead of providing number of steps for the iteration or step size I decided to go with dynamic step size given the logarithmic nature of T-P relation. You provide maximum step in temperature, and python finds related step size of pressure.
