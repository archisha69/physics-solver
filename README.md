# physics-solver
A simple Physics question solver. (wip)

## instructions

<hr>

0. Leave parameter blank if it is an unknown. (note: Only **one** unknown per function)

<hr>

e.g. Finding the energy produced:<br>
`et(P = '200 W', t = '30 s')`<br>
> Value of Q equals to output: `0.006 MJ or 6 kJ or 6000 J`

e.g. Finding the power needed:<br>
`et(Q = '6 kJ', t = '30 s')`<br>
> Value of P equals to output: `0.0002 MW or 0.2 kW or 200 W`

<hr>

1. Parameters' unit can be ignored if the unit equals to its basic unit.

<hr>

e.g. Watt for power and seconds for time<br>
> `et(P = '200', t = '30')`

e.g. Joules for energy (note: In this case, you **must** convert `'6 kJ'` to `'6000 J'` first in order to operate correctly as Joule is the basic unit)<br>
> `et(Q = '6000', t = '30')`

<hr>

Avaliable units (**all** lowercase are accepted):
- `MW`, `kW`, `W` for *P (power)*
- `MJ`, `kJ`, `J` for Q and E(energy)
- `h`, `mins`, `s` for t (time)
- `MJ degC-1`, `kJ degC-1`, `J degC-1` for C (heat capacity)
- `degC`, `degK` for T (Temperature)
- `degC` for dT (delta temperature) (note: Kelvin or Degrees Celsius doesn't affect the changes of temperature)
- `kg`, `g` for m (mass)
- `MJ kg-1 degC-1`, `kJ kg-1 degC-1`, `J kg-1 degC-1` for c (specific heat capacity)
- `MJ kg-1`, `kJ kg-1`, `J kg-1` for l (latent heat)
- `MPa`, `kPa`, `Pa` for p (pressure)
- `N` for F (force)
- `m^2`, `cm^2` for A (area)
- `m^3`, `cm^3` for V (Volume)
- `mol` for n (mole number)


... etc.

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
<p align=center>=====CONVERTERS=====</p>
<hr>

- Power (P) to Energy (Q): Q = P / t -> `PtoQ(P: Power, t: Time)`
- Energy (Q) to Power (P): P = Q / t -> `QtoP(Q: Energy, t: Time)`
- Degrees Celsius (°C) to Kelvin (K): K = C + 273 -> `CtoK(degc: Celsius)`
- Kelvin (K) to Degrees Celsius (°C): C = K - 273 -> `KtoC(degk: Kelvin)`

