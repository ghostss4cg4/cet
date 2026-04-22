# 🏆 PRIORITY ORDER — END-SEM 2026

## P1 (Master First)

### P1-A: Residual Properties from 2nd Virial EOS
Formulas:
```
H^R = P[B - T(dB/dT)]
S^R = -P × (dB/dT)
G^R = BP
```
Derivation: Z=1+BP/RT → (∂Z/∂T)_P → integrate

### P1-B: Kirchhoff Heat of Reaction
Formula:
```
ΔH°_T = ΔH°_298 + R[ΔA(T-298) + (ΔB/2)(T²-298²) + (ΔC/3)(T³-298³) - ΔD(1/T-1/298)]
```
Algorithm: ΔH298 → ΔA,B,C,D → integrate (M+ for 4 blocks)

### P1-C: Entropy of Ideal Gas Flow
Formula:
```
ΔS = nR[A·ln(T₂/T₁) + B(T₂-T₁) + (C/2)(T₂²-T₁²) - D(1/T₁-1/T₂)] - nR·ln(P₂/P₁)
```

## P2 (High Priority)

### P2-A: Adiabatic Turbine/Compressor
```
Step 1 (Isentropic): ΔS=0 → solve T₂_ideal iteratively
Step 2 (W_ideal): W = R[A·ΔT + (B/2)·ΔT² + ...]
Step 3 (Efficiency):
  Turbine: W_actual = η × W_ideal
  Compressor: W_actual = W_ideal / η
```

### P2-B: VdW Isothermal ΔU ΔH ΔS
```
a = 27R²Tc²/(64Pc)
b = RTc/(8Pc)
ΔU = a(1/V₁ - 1/V₂)
ΔS = R·ln[(V₂-b)/(V₁-b)]
ΔH = ΔU + P₂V₂ - P₁V₁
```

## P3 (Medium)
- Carnot: η = 1 - Tc/Th
- Entropy generation: ΔS_gen = ΔS_system + ΔS_surr
- VdW a,b derivation

## P4 (Theory Only)
- Throttling: isenthalpic, JT coefficient
- Liquefaction approaches
- Vapor compression cycle

## MISTAKE PREVENTION TABLE

| # | Mistake | Fix |
|---|---------|-----|
| 1 | °C not K | T(K) = T(°C) + 273.15 always |
| 2 | R = kJ not J | R = 8.314 J/mol·K |
| 3 | η direction | Turbine: ×η; Compressor: /η |
| 4 | S^R sign | Negative at high P |
| 5 | D term sign | ΔH: -D(1/T₂-1/T₁); ΔS: -D/T term |
| 6 | B×10⁻³ | Write full number before substituting |
| 7 | Throttle H=const | H₁=H₂ always |

## 5-MINUTE CRISIS CHEATSHEET

```
SENSIBLE HEAT:  ΔH = R[A·ΔT + (B/2)·ΔT²+...] | ΔS = R[A·ln(T₂/T₁)+B·ΔT+...]
KIRCHHOFF:     ΔH_T = ΔH_298 + R·∫ΔCp·dT
RESIDUAL:      H^R = P[B-T·dB/dT] | S^R = -P·dB/dT
VdW CONST:     a = 27R²Tc²/64Pc | b = RTc/8Pc
VdW ISO:       ΔU = a(1/V₁-1/V₂) | ΔS = R·ln[(V₂-b)/(V₁-b)]
CARNOT:        η = 1-Tc/Th | ω = Tc/(Th-Tc)
TURBINE:       W×η | T₂_actual > T₂_ideal
COMPRESSOR:    W/η | T₂_actual > T₂_ideal
ISOENTROPIC:   ΔS=0 → iterate T₂
THROTTLE:      H₁=H₂
```
