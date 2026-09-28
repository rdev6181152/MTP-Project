# ANSYS Fluent Simulation Setup

## 1. Project Objective

The objective of the CFD simulation is to investigate multiphase flow behaviour in a 2D fluidized-bed reactor containing an internal Y-shaped liquid collector.

The simulation focuses on phase distribution, multiphase flow behaviour, non-Newtonian fluid behaviour, and liquid-phase collection.

---

## 2. CFD Software

- **Software:** ANSYS Fluent
- **Version:** ANSYS Fluent 2026 R1
- **Geometry:** 2D planar
- **Solver:** To be finalized
- **Flow:** Multiphase
- **Fluid behaviour:** Non-Newtonian liquid

---

## 3. Computational Domain

The computational domain represents a 2D vertical fluidized-bed reactor.

The domain contains:

- Reactor fluid region
- Gas phase
- Liquid phase
- Solid phase
- Internal Y-shaped liquid collector

The Y-shaped structure is designed to collect liquid only.

---

## 4. Mesh

### Mesh Generation

The geometry is meshed before importing the case into ANSYS Fluent.

The mesh development will consider:

- Element size
- Local refinement
- Boundary-layer resolution
- Mesh quality
- Skewness
- Orthogonal quality
- Aspect ratio

### Local Refinement

Additional refinement may be applied near:

- Y-shaped collector
- Liquid collection region
- Inlet regions
- Outlet regions
- Regions with expected high velocity gradients
- Phase-interface regions

---

## 5. Materials

The simulation will contain the required materials for:

### Gas Phase

Properties to be specified:

- Density
- Viscosity
- Molecular properties, where applicable

### Liquid Phase

Properties to be specified:

- Density
- Viscosity
- Non-Newtonian rheological parameters

### Solid Phase

Properties to be specified:

- Density
- Particle diameter
- Particle distribution, where applicable

---

## 6. Multiphase Model

A suitable multiphase model will be selected based on the physical characteristics of the reactor.

The model selection will consider:

- Gas-liquid interaction
- Gas-solid interaction
- Liquid-solid interaction
- Three-phase interaction
- Expected phase distribution
- Flow regime
- Computational requirements

The final multiphase model will be documented after model selection.

---

## 7. Non-Newtonian Model

The liquid phase will be represented using an appropriate non-Newtonian rheological model.

The selected model and parameters will be documented after determining the rheological behaviour of the working fluid.

Parameters may include:

- Consistency index
- Flow behaviour index
- Yield stress, where applicable
- Apparent viscosity
- Shear-rate dependence

---

## 8. Boundary Conditions

The following boundary conditions will be defined:

### Gas Inlet

- Boundary type: To be finalized
- Location: Reactor inlet
- Phase: Gas
- Flow condition: To be finalized

### Liquid Inlet

- Boundary type: To be finalized
- Location: Reactor inlet/recirculation inlet
- Phase: Liquid
- Flow condition: To be finalized

### Solid Phase

- Particle properties and inlet/initial conditions: To be finalized

### Reactor Walls

- Boundary type: Wall
- No-slip condition: To be evaluated according to the selected model

### Main Outlet

- Boundary type: To be finalized
- Phase behaviour: To be defined

### Liquid Collector Outlet

- Function: Liquid collection
- Intended phase: Liquid
- Connection: Liquid recirculation system

---

## 9. Initialization

The initial solution will be established according to the selected multiphase modelling approach.

Initialization may include:

- Initial velocity field
- Pressure field
- Gas volume fraction
- Liquid volume fraction
- Solid volume fraction
- Initial bed region
- Initial liquid distribution

The final initialization procedure will be documented after the multiphase model is finalized.

---

## 10. Solution Methods

The following numerical settings will be selected based on the solver and multiphase model:

- Pressure-velocity coupling
- Pressure discretization
- Momentum discretization
- Volume-fraction discretization
- Turbulence discretization
- Transient formulation, if required

The selected schemes will be documented with the corresponding simulation case.

---

## 11. Convergence Monitoring

Simulation convergence will be monitored using:

- Residuals
- Mass imbalance
- Pressure behaviour
- Velocity behaviour
- Phase volume fractions
- Liquid collection rate
- Other relevant physical monitors

Convergence will not be judged using residuals alone; important physical quantities will also be monitored.

---

## 12. Simulation Type

The simulation may be performed as:

### Steady-State

Used where the physical system permits a statistically steady solution.

### Transient

Used where transient multiphase behaviour, phase-interface movement, particle motion, or liquid collection dynamics need to be resolved.

The final choice will depend on the selected multiphase model and research objective.

---

## 13. Post-Processing

The following quantities will be analysed:

- Gas volume fraction
- Liquid volume fraction
- Solid volume fraction
- Velocity distribution
- Pressure distribution
- Pressure drop
- Shear rate
- Apparent viscosity
- Wall shear stress
- Liquid collection rate
- Phase distribution
- Interphase interactions

---

## 14. Validation

The CFD model will be validated using appropriate:

- Published literature
- Experimental data, where available
- Analytical solutions for simplified cases
- Mesh independence studies
- Sensitivity studies

The validation methodology will be documented once reference data are identified.

---

## 15. Simulation Development Stages

The simulation will be developed progressively:

1. Geometry verification
2. Mesh generation
3. Single-phase validation
4. Gas-liquid simulation
5. Gas-solid simulation
6. Gas-liquid-solid simulation
7. Non-Newtonian liquid modelling
8. Y-shaped liquid collection
9. Liquid recirculation
10. Model validation
11. Parametric studies
12. Reactor-performance analysis

---

## 16. Case Management

Each major simulation case will be stored separately.

Example:

```text
Cases/
├── Case_01_Single_Phase/
├── Case_02_Gas_Liquid/
├── Case_03_Gas_Solid/
├── Case_04_Gas_Liquid_Solid/
├── Case_05_Non_Newtonian/
├── Case_06_Y_Collector/
└── Case_07_Recirculation/
