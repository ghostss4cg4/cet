# 🔥 CHAPTER 4: HEAT EFFECTS

## Core Formulas

```
Cp/R = A + BT + CT² + DT⁻²

ΔH = R[A(T₂-T₁) + (B/2)(T₂²-T₁²) + (C/3)(T₂³-T₁³) - D(1/T₂-1/T₁)]

ΔS = R[A·ln(T₂/T₁) + B(T₂-T₁) + (C/2)(T₂²-T₁²) + D(1/2T₁²-1/2T₂²)]
```

## Kirchhoff Law

```
ΔH°_T = ΔH°_298 + R[ΔA(T-298) + (ΔB/2)(T²-298²) + (ΔC/3)(T³-298³) - ΔD(1/T-1/298)]

ΔCp = Σ(ν·Cp)_products - Σ(ν·Cp)_reactants
ΔA = Σ(ν·A)_products - Σ(ν·A)_reactants  [same for B, C, D]
```

## EXAM QUESTION: Heat of Reaction at 723.15 K (2025 Q2iii)

Reaction: CH₃CHO(g) + H₂(g) → C₂H₅OH(g)
ΔH°_f: CH₃CHO = -166190, C₂H₅OH = -277690, H₂ = 0 (J/mol)

Step 1: ΔH°_298 = -277690 - (-166190) - 0 = -111500 J/mol

Step 2: ΔCp constants
| Species | ν | A | B×10³ | C×10⁶ | D×10⁻⁵ |
|---------|---|----|-------|--------|--------|
| C₂H₅OH | +1 | 3.518 | 20.001 | -6.001 | 0 |
| CH₃CHO | -1 | 1.693 | 17.978 | -6.158 | 0 |
| H₂ | -1 | 3.249 | 0.422 | 0 | 0.083 |
ΔA = 3.518-1.693-3.249 = -1.424
ΔB = (20.001-17.978-0.422)×10⁻³ = 1.601×10⁻³
ΔC = (-6.001-(-6.158)-0)×10⁻⁶ = 0.157×10⁻⁶
ΔD = (0-0-0.083)×10⁵ = -0.083×10⁵

Step 3: Kirchhoff at T=723.15 K
```
ΔH°_723 = -111500 + 8.314×[(-1.424)(425.15) + (1.601×10⁻³/2)(523266-88804) + ...]
         ≈ -113355 J/mol
```

## Calculator Trick (M+ for 4 blocks)
```
Block 1: ΔA×(T-298) → M+
Block 2: (ΔB/2)×(T²-298²) → M+
Block 3: (ΔC/3)×(T³-298³) → M+
Block 4: -ΔD×(1/T-1/298) → M+
Sum: RCL M+ → ×8.314 → + ΔH°_298
```

## Common Mistakes
- B coefficient: always ×10⁻³! Write full number.
- D integrates to -D/T (NOT -D/T²)
- Products MINUS reactants (with stoichiometry ν)
- Temperature in KELVIN
