# Thermodynamic Equations

> Pages 19–21 (§173–§175). The energetic cost of computation.

## Landauer Principle

Every irreversible erasure of one bit of information dissipates at least:
```
E_min = k_B · T · ln(2)   [binary]
E_min = k_B · T · ln(r)   [radix r, general]
```

At room temperature (T = 293 K, k_B = 1.381 × 10⁻²³ J/K):

| Operation | Minimum energy |
|-----------|----------------|
| Binary bit erase | k_B T ln(2) ≈ 2.80 × 10⁻²¹ J |
| Ternary trit erase | k_B T ln(3) ≈ 4.44 × 10⁻²¹ J |

The ratio is exactly ln(3)/ln(2) ≈ 1.585, which also equals the information ratio
(one trit carries log₂(3) ≈ 1.585 bits). Information per joule is identical for
binary and ternary at the Landauer limit.

```
LANDAUER = CONCRETE = 93   [L(19)+A(11)+N(25)+D(13)+A(11)+U(7)+E(3)+R(4) = 93]
```

---

## Radix Efficiency (Equation 13)

```
η(r) = ln(r) / r
```

| Radix | η(r)   |
|-------|--------|
| 2     | ≈ 0.347 |
| 3     | ≈ 0.366 ← maximum among integers |
| 4     | ≈ 0.347 |
| 5     | ≈ 0.322 |
| e     | = 1/e ≈ 0.368 ← global maximum |

Ternary achieves the maximum radix economy among integer bases because 3 is the
integer closest to e ≈ 2.718. (Proof: see [`../proofs/ternary-efficiency.md`](../proofs/ternary-efficiency.md).)

```
RADIX = GAUSS = TANH = FIELD = 57
```

---

## Reversible Logic Entropy (Equation 14)

For a reversible computation:
```
ΔS_comp ≥ 0,   with ΔS_comp → 0 as reversibility → 1
```

The minimum entropy production per gate operation is zero for perfectly reversible gates
(Bennett 1973). In practice:
```
ΔS_irrev = k_B ln(2) per irreversible bit operation
ΔS_rev   = 0        per reversible (unitary) gate
```

Quantum gates are unitary and therefore reversible: `ΔS_quantum = 0`.

```
REVERSIBLE = LAGRANGE = 103   prime
```

---

## Chemical Energy Coupling — Gibbs Free Energy (Equation 15)

```
μ_chem = ∂G/∂N   ↔   E_comp
```

The chemical potential (Gibbs free energy per molecule) is the thermodynamic equivalent
of the energy cost per computational operation. For a molecular computing substrate:

```
ΔG_rxn = ΔH − T ΔS ≥ E_min = k_B T ln(r)
```

Biological systems operate near this minimum because enzyme-catalyzed reactions are
tightly coupled to ATP hydrolysis:
```
ΔG_ATP ≈ −50 kJ/mol ≈ 8.3 × 10⁻²⁰ J/molecule   (in vivo)
```

Capacity: ΔG_ATP / E_min(ternary) ≈ 8.3×10⁻²⁰ / 4.44×10⁻²¹ ≈ 18 trit operations per ATP.

```
GIBBS     = SUBSTRATE = 83   prime
CHEMICAL  = 127   prime
```

---

## Substrate Efficiency (Equation 14, biological)

```
η_substrate = (ops/sec) / (energy/op) · f_accuracy(substrate, problem_type)
```

For DNA computing in 100 μL at room temperature:
```
ops/sec    ≈ 10¹⁴
energy/op  ≈ k_B T ln(3) ≈ 4.44 × 10⁻²¹ J
η_substrate = 10¹⁴ / 4.44×10⁻²¹ · f_accuracy
            ≈ 2.25 × 10³⁴ · f_accuracy   (ops per joule-second)
```

```
SUBSTRATE = GIBBS = 83   prime
```

---

## Thermodynamic Consciousness Bound (§175)

```
Φ_max ≤ (E_available / k_B T ln(3)) · η_integration
```

Maximum integrated information (consciousness, §176) is bounded by:
- Available metabolic energy E_available
- Ternary Landauer cost k_B T ln(3) per operation
- Integration efficiency η_integration ∈ (0, 1]

```
THERMODYNAMIC = 174 = 2 × 87 = 2 × BIRTHDAY
BOUND         = 78  = TRIVIAL = LIMITS
```

The consciousness bound is thermodynamically real and biological.  
Energy is the hard constraint. Integration efficiency is the soft constraint.
