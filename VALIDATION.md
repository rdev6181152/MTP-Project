# CFD Model Validation

## 1. Purpose

The purpose of validation is to establish the reliability of the CFD model by comparing numerical predictions with appropriate analytical solutions, published literature, experimental data, and/or benchmark cases.

Validation will be performed progressively as the complexity of the multiphase model increases.

---

## 2. Validation Strategy

The validation approach will follow a progressive methodology:

1. Single-phase flow validation
2. Mesh independence study
3. Multiphase flow validation
4. Non-Newtonian flow validation
5. Fluidized-bed validation
6. Liquid-collection validation
7. Final reactor-model validation

The validation complexity will be increased only after the preceding model has been adequately verified.

---

## 3. Single-Phase Flow Validation

A simplified single-phase case will be used to verify the basic CFD setup.

The validation may include comparison of:

- Velocity profile
- Pressure drop
- Mass flow rate
- Wall shear stress

The simplified case will provide a baseline before introducing multiphase physics.

### Reference

**Reference case:** To be specified

### CFD Result

| Parameter | CFD Result | Reference | Difference (%) |
|---|---:|---:|---:|
| Pressure drop | TBD | TBD | TBD |
| Maximum velocity | TBD | TBD | TBD |
| Mass flow rate | TBD | TBD | TBD |

---

## 4. Mesh Independence

A mesh independence study will be performed to determine whether further mesh refinement produces significant changes in the important physical quantities.

### Mesh Levels

| Mesh | Elements | Quantity 1 | Quantity 2 | Quantity 3 |
|---|---:|---:|---:|---:|
| Coarse | TBD | TBD | TBD | TBD |
| Medium | TBD | TBD | TBD | TBD |
| Fine | TBD | TBD | TBD | TBD |

The final mesh will be selected based on an appropriate balance between numerical accuracy and computational cost.

---

## 5. Multiphase Model Validation

After validation of the single-phase model, the multiphase model will be evaluated.

Depending on the selected multiphase formulation, validation parameters may include:

- Phase volume fraction
- Pressure drop
- Velocity
- Bed expansion
- Phase distribution
- Interphase behaviour

The selected validation quantities will depend on the available reference data.

---

## 6. Non-Newtonian Flow Validation

The non-Newtonian formulation will be validated using an appropriate benchmark or published reference case.

The comparison may include:

- Velocity profile
- Pressure drop
- Apparent viscosity
- Shear-rate distribution
- Flow rate

### Rheological Model

**Model:** To be finalized

### Rheological Parameters

| Parameter | Value |
|---|---:|
| Density | TBD |
| Consistency index | TBD |
| Flow behaviour index | TBD |
| Yield stress | TBD |
| Reference temperature | TBD |

---

## 7. Fluidized-Bed Validation

The fluidized-bed model will be evaluated using appropriate literature or experimental data.

Potential validation parameters include:

- Pressure drop across the bed
- Minimum fluidization behaviour
- Bed expansion
- Solid volume fraction
- Particle velocity
- Gas velocity
- Phase distribution

### Validation Data

| Parameter | CFD | Literature/Experiment | Difference (%) |
|---|---:|---:|---:|
| Pressure drop | TBD | TBD | TBD |
| Bed height | TBD | TBD | TBD |
| Solid volume fraction | TBD | TBD | TBD |

---

## 8. Y-Shaped Liquid Collector Validation

The liquid-collection behaviour will be evaluated after establishing the validated multiphase reactor model.

The analysis will focus on:

- Liquid flow entering the collector
- Liquid collection rate
- Liquid velocity
- Pressure distribution
- Gas behaviour near the collector
- Solid behaviour near the collector

The collector will be evaluated specifically as a **liquid-phase collection structure**.

---

## 9. Experimental Comparison

Where experimental data are available, CFD predictions will be compared against experimental measurements.

Potential comparison parameters include:

- Liquid collection rate
- Pressure drop
- Phase distribution
- Velocity
- Bed expansion
- Other measurable reactor-performance parameters

### Experimental Data

**Status:** To be identified

---

## 10. Literature Comparison

Published studies will be used to identify suitable benchmark data and modelling approaches.

The comparison will document:

- Reactor geometry
- Operating conditions
- Fluid properties
- Particle properties
- Multiphase model
- Turbulence model
- Numerical method
- Validation parameters
- CFD results
- Reference results

---

## 11. Error Analysis

The difference between CFD and reference results will be quantified where appropriate.

For a measured quantity, the percentage difference may be calculated as:

```text
Percentage Difference =
|CFD − Reference| / |Reference| × 100
