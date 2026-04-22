# ❄️ CHAPTER 9: REFRIGERATION

## Carnot Refrigerator
```
ω_Carnot = T_C/(T_H - T_C)    [T in Kelvin!]
ω_HP = ω_Carnot + 1
```

## Vapor-Compression Cycle (4 States)
```
1→2: Compression (adiabatic) — compressor
2→3: Condensation — condenser (Q_H out)
3→4: Throttling — expansion valve (H₃=H₄!)
4→1: Evaporation — evaporator (Q_C in)

COP: ω = Q_C/W = (H₁-H₄)/(H₂-H₁)
Mass flow: ṁ = Q_C/(H₁-H₄)
```

## Efficiency in Real Cycle
```
η_comp = W_ideal/W_actual
W_actual = W_ideal/η
H₂_actual = H₁ + W_actual
```

## EXAM: HFC-134a Problem (2024 Q7ii)
```
T_space = -23°C, T_cooling = 27°C, 5°C approach:
T_evap(refrig) = -23-5 = -28°C = 245.15 K
T_cond(refrig) = 27+5 = 32°C = 305.15 K

ω_Carnot = 245.15/(305.15-245.15) = 245.15/60 = 4.09

Mass flow (with property tables):
ṁ = Q_C/(H₁-H₄) = 200 kW / Δh  [kg/s]
```

## Liquefaction Theory (5-mark answer)

1. Linde/JT: Compress → HX → throttle → separator → liquid
   Needs T < T_inversion (Air: 607K ✓, H₂: 202K, He: 43K)

2. Claude: Expansion engine instead of throttle → more reversible → better yield

3. Pre-cooling: Liquid N₂ for H₂; Liquid H₂ for He

4. Cascade: Multiple refrigerants (propane→ethylene→methane) for LNG

## Inversion Temperatures
- Air: ~607 K (fine at room temperature)
- N₂: ~621 K (fine at room T)
- H₂: ~202 K (MUST pre-cool first)
- He: ~43 K (MUST pre-cool with liquid H₂)

## Common Mistakes
- °C not K in Carnot formula
- 5°C approach temperature: T_refrig = T_process ± 5
- Throttle: H₃=H₄ (H does NOT change)
- ω > 10 → you used °C instead of K
