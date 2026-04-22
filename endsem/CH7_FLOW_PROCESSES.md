# ⚙️ CHAPTER 7: FLOW PROCESSES

## SFEE Master Equation
```
ΔH + (u₂²-u₁²)/2000 + g·Δz/1000 = Q + Ws    [all in kJ/kg]

For turbine/compressor (neglect KE, PE):
ΔH = Q + Ws
Adiabatic: ΔH = Ws
```

## Throttling
```
H₁ = H₂ (isenthalpic)
Ideal gas: T unchanged
Real gas: μ_JT = (∂T/∂P)_H = [T(∂V/∂T)_P - V]/Cp
μ_JT > 0: cooling on throttle (useful for liquefaction)
```

## Adiabatic Turbine (⭐ EXAM T-F)

```
Step 1: Isentropic condition (ΔS = 0)
R[A·ln(T₂/T₁) + B(T₂-T₁) + (C/2)(T₂²-T₁²) - D(1/T₁-1/T₂)] = R·ln(P₂/P₁)
→ Cancel R, solve iteratively for T₂_ideal

Step 2: W_ideal = -R[A(T₂-T₁) + (B/2)(T₂²-T₁²) + (C/3)(T₂³-T₁³)]
(positive for turbine expansion)

Step 3: η_turbine = W_actual/W_ideal
W_actual = η × W_ideal

Step 4: T₂_actual from W_actual = ΔH equation
(T₂_actual > T₂_ideal for real turbine)
```

## Adiabatic Compressor
```
Same isentropic calculation for T₂_ideal
η_comp = W_ideal/W_actual → W_actual = W_ideal/η
T₂_actual > T₂_ideal (more heating in real compressor)
```

## EFFICIENCY TRAP (Most Common Mistake!)
```
TURBINE:    η = W_actual/W_ideal  → W_actual = η × W_ideal (multiply)
COMPRESSOR: η = W_ideal/W_actual  → W_actual = W_ideal/η  (divide)
```

## Quick T₂ Estimate (for checking)
```
T₂_ideal ≈ T₁ × (P₂/P₁)^((γ-1)/γ)
γ = Cp/Cv; for diatomic γ≈1.4; polyatomic γ≈1.2-1.3
```

## EXAM: CO₂ Expander (2024 Q6)
T₁=673.15K, P₁=8bar→P₂=1bar, η=0.75
Cp/R = 5.457 + 1.045×10⁻³T - 1.157×10⁵T⁻²

Isentropic ΔS = 0:
5.457·ln(T₂/673.15) + 1.045×10⁻³(T₂-673.15) + 1.157×10⁵(1/T₂-1/673.15) = ln(1/8) = -2.079
Solve: T₂_ideal ≈ 471 K

W_actual = 0.75 × W_ideal

## Pump Work (Liquid)
```
W_pump = V_liquid × (P₂-P₁)    [in J/mol if V in m³/mol and P in Pa]
For water: V ≈ 0.001 m³/kg → W = 0.001×ΔP
ΔT_pump = W_actual/Cp
```

## Steam Tables (If used)
- Saturated: given T → read P_sat, H_f, H_g, S_f, S_g
- Superheated: given T,P → H and S directly
- Quality x: H = H_f + x·H_fg; S = S_f + x·S_fg
