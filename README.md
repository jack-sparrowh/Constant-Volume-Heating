# Constant-Volume-Heating
Constant Volume Heating of closed tank filled with liquid and nitrogen blanket.

It provides T-P values for isochoric heating. This can be useful when liquid level in blanketed tank is required for pressure relief device (PRD) sizing.

By providing initial parameters like temperature, pressure and liquid level as well as function of vapor pressure of liquid and function for density, python will output T-P data given specified final pressure in tank (set pressure of PRD).

It is assumed that isothermal compressibility of liquid is 0. The reason being that usually density functions for liquids do not provide pressure dependence (I have never seen one that does).

Code is somewhat rough as I whipped it in short time.
