# SIDE-cubit-axis v0.1

SIDE-cubit-axis compiles equalities among natural numbers defined in its own file. Statements at e0a2aec:

    theorem cubit_unification : cubitCardinality = cubeVertices ∧ cubitCardinality = phi_24 ∧ cubitCardinality = formationCount + 1 ∧ cubeEdges = spectralVolume ∧ cubeEdges = tower2 ∧ cubitNonTrivial = steaneN (SIDECubitAxis/Basic.lean :203)

The file imports no sibling, so nothing it states of another kernel is checked, and no statement names (ℤ/2)³.

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

Per federation discipline, individual kernels carry no Lake cross-dependencies — each is independently auditable. The cubit substrate (ℤ/2)³ nevertheless appears in four sibling kernels with related numerical content.

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
- `nontrivial_eq_card_minus_one` — 7 non-trivial elements
- `cube_euler` — V − E + F = 2

### §2 — The {2,3}-doubling tower
- `doubling_tower` — 6 → 12 → 24
- `tower2_eq_cube_edges` — level 2 = cube edges (12)
- `tower3_factorization` — level 3 = cubit × 3 (24 = 8 · 3)

### §3 — Three cube decompositions
- `edge_stratum_sum` — (3, 6, 3) → 12 edges (spinor calibration view)
- `vertex_stratum_sum` — (3, 3, 1) → 7 non-trivial vertices (Steane / class-number view)
- `middle_terms_related` — 6 = 2 · 3 connects the two strata

### §4 — Class A formation tuple
- `spectral_volume_eq_cube_edges` — λ = n₁·n₂·n₃ = 12 = cube edges
- `formation_count_eq_nontrivial` — n₁ + n₂ + n₃ + n₄ = 7
- `wall_squared_condition` — n₁ = n₃ (Class A)
- `element_level_obstruction` — Hamming (3,3,1) ≠ Formation (2,3,2) at element level
- `middle_stratum_matches` — But the middle strata DO match (weight 2 ↔ n₂)

### §6 — Steane connection
- `steane_stabilizer_count` — n − k = 6 = 2·n₂

## Federation kernel count: 14

| # | Kernel | Role |
|---|---|---|
| 1 | SIDE-kernel | Day 1 RH proof (Zenodo) |
| 2–10 | SIDE-meta, -bijection, -omega-b, -substrate-cluster, -coupling, -orchestrator, -formation-arithmetic, -residual-bridge, -class-coupling | Matter-as-remainder spiral (8/8) |
| 11 | SIDE-spinor-calibration | Calibration ‖v‖²·ζ(−1) = −1 |
| 12 | SIDE-steane-arithmetic | Fano plane / Steane [[7,1,3]] origin |
| 13 | SIDE-dirichlet-mod-24 | Identity-Formation count bijection |
| 14 | SIDE-class-number-anomaly | Diagonal three-way distinction |

(14 with two parallel additions this turn.)

## License

CC-BY 4.0. Cite as:

> Seale, J. Y. (2026). *SIDE-cubit-axis v0.1: Cross-federation coherence of the cubit substrate.* A PLACE TO STAND Research Programme.

---

`:: → · ← ::`

