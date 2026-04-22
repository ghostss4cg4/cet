# 🔬 CHAPTER 6: THERMODYNAMIC PROPERTIES OF FLUIDS

## Residual Properties — DEFINITION
```
M^R = M - M^ig (at same T, P)
H^R = H - H^ig  (accounts for intermolecular forces)
S^R = S - S^ig
```

## Residual Properties from 2nd Virial EOS (⭐ EXAM Q1)

Given: Z = 1 + BP/(RT)

Derivation:
```
(∂Z/∂T)_P = (P/RT)(dB/dT - B/T)

H^R/RT = -T ∫₀ᴾ [(∂Z/∂T)_P / P] dP = -(T/RT)(dB/dT - B/T)×P
→ H^R = P[B - T(dB/dT)]     ← MEMORIZE

G^R/RT = ∫₀ᴾ (Z-1)/P dP = BP/RT → G^R = BP

S^R/R = H^R/RT - G^R/RT = [B-T(dB/dT)]P/RT - BP/RT = -P(dB/dT)/R
→ S^R = -P(dB/dT)           ← MEMORIZE
```

## Pitzer Generalized Correlation
```
BPc/(RTc) = B⁰ + ω·B¹
B⁰ = 0.083 - 0.422/Tr^1.6
B¹ = 0.139 - 0.172/Tr^4.2
dB⁰/dTr = 0.675/Tr^2.6
dB¹/dTr = 0.722/Tr^5.2

H^R/(RTc) = Pr[(B⁰ - Tr·dB⁰/dTr) + ω(B¹ - Tr·dB¹/dTr)]
S^R/R = -Pr[dB⁰/dTr + ω·dB¹/dTr]
```

## Van der Waals — Constants
```
a = 27R²Tc²/(64Pc)
b = RTc/(8Pc)
Vc = 3b
Zc = 3/8 = 0.375
```

Derivation: At critical point (∂P/∂V)_Tc = 0 AND (∂²P/∂V²)_Tc = 0

## VdW Isothermal (⭐ EXAM Q4ii)
```
ΔU = a(1/V₁ - 1/V₂)        [from (∂U/∂V)_T = a/V²]
ΔS = R·ln[(V₂-b)/(V₁-b)]   [from (∂P/∂T)_V = R/(V-b)]
ΔH = ΔU + P₂V₂ - P₁V₁
```

Physical sense:
- Compression (V₂<V₁): ΔU<0 (attractive forces → lower PE), ΔS<0 (less disorder)
- Expansion: opposite signs

## Common Mistakes
- S^R sign: NEGATIVE (-P·dB/dT)
- B (2nd virial, T-dependent) ≠ b (VdW, constant)
- Units: R=83.14 cm³·bar/mol·K when using cm³ and bar
