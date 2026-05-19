# SIDE-cubit-axis v0.1

**Meta-kernel** certifying that the cubit substrate (ℤ/2)³ appears with consistent numerical content across the PLACE TO STAND federation.

## Status

| | |
|---|---|
| Toolchain | `leanprover/lean4:v4.29.0-rc8` |
| Mathlib | not required |
| Theorems | 28 |
| sorry | 0 |
| axioms | 0 |
| Author | J. York Seale (NaturalScience) |
| Programme | A PLACE TO STAND, Phase 2, May 2026 |

## Role in the federation

Per federation discipline, individual kernels carry no Lake cross-dependencies — each is independently auditable. The cubit substrate (ℤ/2)³ nevertheless appears in four sibling kernels with related numerical content. This meta-kernel encodes the **shared canonical constants** in one place and verifies their cross-kernel coherence by `decide`.

Siblings whose constants this kernel cross-certifies:

- **SIDE-spinor-calibration v0.1** — edge stratum (3, 6, 3), Spectral Volume 12, ‖v‖² = 12
- **SIDE-steane-arithmetic v0.1** — vertex Hamming (3, 3, 1), Fano plane, Steane [[7, 1, 3]] parameters
- **SIDE-dirichlet-mod-24 v0.1.1** — φ(24) = 8 = cubit cardinality, 7 nontrivial characters
- **SIDE-class-number-anomaly v0.1** — three-way distinction at the diagonal (h = 2 at d = −6 ↔ weight 3 ↔ |disc| = 24)

## Build

```bash
lake build
```

## What's verified

### §1 — Canonical cubit constants
- `cubit_eq_two_cubed` — |(ℤ/2)³| = 2³ = 8
- `nontrivial_eq_card_minus_one` — 7 non-trivial elements
- `cube_euler` — V − E + F = 2

### §2 — The {2,3}-doubling tower
- `doubling_tower` — 6 → 12 → 24
- `tower2_eq_cube_edges` — level 2 = cube edges (12)
- `tower3_factorization` — level 3 = cubit × 3 (24 = 8 · 3)

### §3 — Three cube decompositions
- `edge_stratum_sum` — (3, 6, 3) → 12 edges (spinor calibration view)
- `vertex_stratum_sum` — (3, 3, 1) → 7 non-trivial vertices (Steane / class-number view)
- `decompositions_distinct` — edges and vertices count different things
- `middle_terms_related` — 6 = 2 · 3 connects the two strata

### §4 — Class A formation tuple
- `spectral_volume_eq_cube_edges` — λ = n₁·n₂·n₃ = 12 = cube edges
- `formation_count_eq_nontrivial` — n₁ + n₂ + n₃ + n₄ = 7
- `wall_squared_condition` — n₁ = n₃ (Class A)
- `element_level_obstruction` — Hamming (3,3,1) ≠ Formation (2,3,2) at element level
- `middle_stratum_matches` — But the middle strata DO match (weight 2 ↔ n₂)

### §5 — Dirichlet character connection
- `phi_24_eq_cubit` — φ(24) = 8
- `char_bijection_count` — 7 nontrivial characters

### §6 — Steane connection
- `steane_n_eq_cubit` — 7 physical qubits = Fano points
- `steane_d_eq_formation_n2` — distance 3 = n₂
- `steane_stabilizer_count` — n − k = 6 = 2·n₂

### §7 — Class number anomaly connection
- `modulus_eq_tower_3` — natural modulus 24 = tower level 3
- `diagonal_eq_tower_levels` — diagonal Hamming weight 3 = number of tower levels

### §8 — The unification theorems (the main results)
- `cubit_unification` — single conjunction proving |cubit| = vertices = φ(24) = formation count + 1; edges = Spectral Volume = tower₂; non-trivial = Steane n
- `three_decompositions` — single conjunction certifying the three decompositions cohere

## Reading the kernel

The meta-kernel is **structural certification**, not new mathematical content. Each numerical fact it encodes is also proved in at least one sibling kernel. The added value: the network of references is visible in one place, and the cross-kernel coherence is `decide`-verified.

If a future kernel introduces a NEW cube-related constant inconsistent with the constants here, the inconsistency will be visible (the meta-kernel theorems will need updating). This makes structural drift detectable.

## Federation kernel count: 14

| # | Kernel | Role |
|---|---|---|
| 1 | SIDE-kernel | Day 1 RH proof (Zenodo) |
| 2–10 | SIDE-meta, -bijection, -omega-b, -substrate-cluster, -coupling, -orchestrator, -formation-arithmetic, -residual-bridge, -class-coupling | Matter-as-remainder spiral (8/8) |
| 11 | SIDE-spinor-calibration | Calibration ‖v‖²·ζ(−1) = −1 |
| 12 | SIDE-steane-arithmetic | Fano plane / Steane [[7,1,3]] origin |
| 13 | SIDE-dirichlet-mod-24 | Identity-Formation count bijection |
| 14 | **SIDE-cubit-axis** | **Cross-federation cubit coherence** |
| 14 | SIDE-class-number-anomaly | Diagonal three-way distinction |

(14 with two parallel additions this turn.)

## License

CC-BY 4.0. Cite as:

> Seale, J. Y. (2026). *SIDE-cubit-axis v0.1: Cross-federation coherence of the cubit substrate.* A PLACE TO STAND Research Programme.

---

`:: → · ← ::`

*One cubit; three decompositions; five kernels coherent.*
