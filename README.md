# physics-solver
A simple Physics question solver. (wip)

## instructions

<hr>

0. Do not input the parameter of the unknown that you are finding. (note: Leave only ***one*** unknown per function)

<hr>

e.g. Finding the energy (*Q*) produced:<br>
`et(P = '200 W', t = '30 s')`<br>
> Value of *Q* equals to output: `0.006 MJ or 6 kJ or 6000 J`

e.g. Finding the power (*P*) needed:<br>
`et(Q = '6 kJ', t = '30 s')`<br>
> Value of *P* equals to output: `0.0002 MW or 0.2 kW or 200 W`

<hr>

1. Parameters' unit can be ignored if the unit used equals to its basic unit.

<hr>

e.g. *Watt* for *power* and *seconds* for *time*<br>
> `et(P = '200', t = '30')`

e.g. *Joules* for *energy* (note: In this case, you ***must*** convert `'6 kJ'` to `'6000 J'` first in order to operate correctly as *Joule* is the basic unit)<br>
> `et(Q = '6000', t = '30')`

<hr>

## units
For avaliable units (original cases and ***all*** lowercase are accepted) are being saved inside `standard_units.py`

## constants
Constants are being saved inside `constants.py`.

## functions

<hr>
<p align=center>=====HEAT=====</p>
<hr>

- Energy transfer:  P = Q / T -> `et(P: Power, Q: Energy, T: Temperature)`
- Heat capacity: Q = CΔT -> `hc(Q: Energy, C: Heat capacity, dT: Temperature changes)`
- Specific heat capacity: Q = mcΔT -> `shc(Q: Energy, m: Mass, c: Specific heat capacity, dT: Temperature changes)`
- Specific latent heat: Q = ml -> `slc(Q: Energy, t: Time)`
- Total energy: E = ml + mcΔT -> `te(E: Total energy, m: Mass, l: Latent heat, c: Specific heat capacity, dT: Temperature changes)`
- Total energy2 : E = ml + CΔT -> `te2(E: Total energy, m: Mass, l: Latent heat, C: Heat capacity, dT: Temperature changes)`

<hr>
<p align=center>=====PRESSURE=====</p>
<hr>

- Pressure force: p = F / A -> `pf(p: Pressure, F: Force, A: Area)`
- Boyle's law: p<sub>1</sub>V<sub>1</sub> = p<sub>2</sub>V<sub>2</sub> -> `bl(p1: Pressure before, V1: Volume before, p2: Pressure after, V2: Volume after)`
- Pressure law: p<sub>1</sub> / T<sub>1</sub> = p<sub>2</sub> / T<sub>2</sub> -> `pl(p1: Pressure before, T1: Temperature before, p2: Pressure after, T2: Temperature after)`
- Charles' law: V<sub>1</sub> / T<sub>1</sub> = V<sub>2</sub> / T<sub>2</sub> -> `cl(V1: Volume before, T1: Temperature before, V2: Volume after, T2: Temperature after)`

<hr>
<p align=center>=====GAS=====</p>
<hr>

- General gas law: pV = nRT -> `ggl(p: Pressure, V: Volume, n: Mole number, T: Temperature)`
- Transformed ratio formula: p<sub>1</sub>V<sub>1</sub> / n<sub>1</sub>T<sub>1</sub> = p<sub>2</sub>V<sub>2</sub> / n<sub>2</sub>T<sub>2</sub> -> `ggl2(p1: Pressure before, V1: Volume before, n1: Mole before, T1: Temperature before, p2: Pressure after, V2: Volume after, n2: Mole after, T2: Temperature after)`

<hr>
<p align=center>=====MOTION=====</p>
<hr>

- Equations of motion1: v = u + at - ``
- Equations of motion2: s = 1/2(u + v)t^2
- Equations of motion3:
- Equations of motion4: v^2 = u^2 + 2as
- Transformed ratio formula:

<hr>
<p align=center>=====CONVERTERS=====</p>
<hr>

*(Sorry there's no Celsius to Celsius, Fahrenheit to Fahrenheit, and Kelvin to Kelvin)*
- *Power (P)* to *Energy (Q)*: Q = P / t -> `PtoQ(P: Power, t: Time)`
- *Energy (Q)* to *Power (P)*: P = Q / t -> `QtoP(Q: Energy, t: Time)`
- *Degrees Celsius (°C)* to *Fahrenheit (°F)*: F = C * 1.8 + 32 -> `CtoF(degc: Celsius)`
- *Degrees Celsius (°C)* to *Kelvin (K)*: K = C + 273 -> `CtoK(degc: Celsius)`
- *Degrees Fahrenheit (°F)* to *Celsius (°C)*: C = F / 1.8 - 32 -> `FtoC(degf: Fahrenheit)`
- *Degrees Fahrenheit (°F)* to *Kelvin (K)*: K = (F / 1.8 - 32) - 273 -> `FtoK(degf: Fahrenheit)`
- *Kelvin (K)* to *Degrees Celsius (°C)*: C = K - 273 -> `KtoC(degk: Kelvin)`
- *Kelvin (K)* to *Degrees Fahrenheit (°F)*: F = (K - 273) * 1.8 + 32 -> `KtoF(degk: Kelvin)`

