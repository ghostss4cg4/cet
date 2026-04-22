# ⚖️ CHAPTER 5: SECOND LAW & ENTROPY

## Carnot
```
η_Carnot = 1 - T_C/T_H
ω_Carnot = T_C/(T_H - T_C)
```
T in KELVIN always.

## Entropy — Ideal Gas
```
Isothermal: ΔS = -nR·ln(P₂/P₁) = nR·ln(V₂/V₁)
Isobaric:   ΔS = nR∫(Cp/T)dT = nR[A·ln(T₂/T₁) + B(T₂-T₁) + (C/2)(T₂²-T₁²)]
General:    ΔS = above - nR·ln(P₂/P₁)
```

## Entropy Generation (Irreversible)
```
ΔS_gen = ΔS_system + ΔS_surroundings ≥ 0
ΔS_system = state function (same as reversible!)
ΔS_surr = Q_actual/T_surr (positive = heat received)
```

## EXAM: Nuclear Plant (2024 Q3)
```
T_H = 315+273.15 = 588.15 K
T_C = 20+273.15 = 293.15 K
η_max = 1 - 293.15/588.15 = 50.16%
Q_H = W/η = 750/0.5016 = 1494.6 MW
Q_C = Q_H - W = 744.6 MW
Actual η = 0.6×50.16% = 30.1%
```

## EXAM: Heat Exchanger ΔS (2025 Q2ii)
Ideal gas Cp=(7/2)R, same flows, 70→190°C, hot enters at 320°C.
```
Energy balance: T_hot_out = 593.15-(463.15-343.15) = 473.15 K
ΔS_cold = (7/2)R·ln(463.15/343.15) = +8.73 J/mol·K
ΔS_hot = (7/2)R·ln(473.15/593.15) = -6.58 J/mol·K
ΔS_total = +2.15 J/mol·K > 0 ✓
```
Note: ΔS_total same for parallel and countercurrent!

## EXAM: Irreversible Isothermal Compression (2024 Q3ii)
```
1 mol, 130°C, 2.5→5 bar, W_actual = 1.3×W_rev, T_reservoir = 25°C
W_rev = RT·ln(P₂/P₁) = 8.314×403.15×0.693 = 2325 J/mol
W_actual = 1.3×2325 = 3023 J/mol
Q = -W_actual = -3023 J (leaves gas)
ΔS_gas = -R·ln(P₂/P₁) = -5.76 J/mol·K
ΔS_surr = +3023/298.15 = +10.14 J/mol·K
ΔS_total = -5.76 + 10.14 = +4.38 J/mol·K > 0 ✓
```
