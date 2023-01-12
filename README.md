# physics-solver
A simple Physics question solver. (wip)

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

### converter
- Power (P) to Energy (Q): Q = P / t -> `PtoQ(P: Power, t: Time)`
- Energy (Q) to Power (P): P = Q / t -> `QtoP(Q: Energy, t: Time)`
- Degrees Celsius (°C) to Kelvin (K): K = C + 273 -> `CtoK(degc: Celsius)`
- Kelvin (K) to Degrees Celsius (°C): C = K - 273 -> `KtoC(degk: Kelvin)`

