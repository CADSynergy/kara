# KĀRĀ | کارا

**Open 1D Vehicle Energy & Performance Testbench**

KĀRĀ is CADSynergy’s open-source 1D vehicle simulation testbench for powertrain architecture, drive-cycle analysis, energy use, fuel consumption, performance, range estimation, and validation.

KĀRĀ is being developed as part of **CADSynergy Open Mobility Lab** to support open, transparent, and extensible vehicle simulation workflows for real-world driving conditions, with an initial focus on Iranian roads and drive cycles.

---

## What is KĀRĀ?

KĀRĀ aims to provide a lightweight, open, and engineering-focused environment for simulating vehicle behavior over drive cycles.

The project is intended to support:

* 1D vehicle and powertrain simulation
* Drive-cycle analysis
* Fuel and energy consumption estimation
* Range and performance assessment
* Powertrain architecture comparison
* Open benchmark cases
* Validation workflows using public and private datasets
* Future ML-assisted calibration and model improvement

KĀRĀ is not intended to replace enterprise tools such as Simcenter Amesim, GT-Suite, AVL Cruise, or other industrial-grade simulation platforms. Instead, it is designed as an open and accessible testbench for early-stage analysis, research, education, benchmarking, and collaborative model development.

---

## Project status

KĀRĀ is currently in the early foundation stage.

Current status:

* Repository initialized
* Open-source governance setup in progress
* Core architecture under definition
* Initial 1D simulation MVP planned
* Drive-cycle data model planned
* CADSynergy platform integration planned

The first public technical milestone will be **KĀRĀ v0.1**, focused on a minimal working 1D simulation workflow.

---

## Roadmap

### v0.1 — Core MVP

Planned scope:

* Basic vehicle configuration schema
* Basic drive-cycle CSV parser
* Longitudinal road-load calculation
* Simple conventional vehicle simulation
* Simple BEV energy simulation
* Fuel and energy summary outputs
* Basic post-processing plots
* Example notebooks
* Initial validation examples

### v0.2 — Hybrid foundation

Planned scope:

* Simplified series hybrid model
* Simplified parallel hybrid model
* Battery equivalent-circuit model
* Motor/generator efficiency maps
* Regenerative braking
* Rule-based control strategy examples

### v0.3 — DriveCycleIR layer

Planned scope:

* Public drive-cycle metadata standard
* Initial Iranian drive-cycle examples
* Dataset contribution workflow
* Cycle quality checks
* Public benchmark cases

### v0.4 — Calibration and validation

Planned scope:

* Measured vs simulated comparison
* Parameter correction workflows
* Residual analysis
* Confidence scoring
* Initial ML-assisted calibration tools

---

## Installation

KĀRĀ is not yet packaged for installation.

Installation instructions will be added after the first working Python package structure is available.

Planned installation format:

```bash
pip install kara
```

For development, the expected workflow will be:

```bash
git clone https://github.com/CADSynergy/kara.git
cd kara
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
```

---

## Quick start

A quick-start example will be added in the first technical release.

The planned workflow is:

1. Select or define a vehicle configuration.
2. Load a drive-cycle file.
3. Run the simulation.
4. Review summary metrics and plots.
5. Compare results across vehicle configurations or drive cycles.

Example notebooks will be added under:

```text
examples/
```

---

## Repository structure

The planned repository structure is:

```text
kara/
├── src/
│   └── kara/
│       ├── schemas/
│       ├── cycles/
│       ├── vehicles/
│       ├── engines/
│       ├── adapters/
│       ├── simulation/
│       ├── postprocessing/
│       └── validation/
├── examples/
├── data/
│   └── public_cycles/
├── docs/
├── tests/
├── LICENSE
├── NOTICE
├── CONTRIBUTING.md
├── GOVERNANCE.md
└── README.md
```

This structure may evolve as the project matures.

---

## Contributing

KĀRĀ is an open-source project and welcomes contributions from engineers, researchers, students, developers, and industry practitioners.

Planned contribution areas include:

* Core simulation models
* Drive-cycle datasets
* Vehicle configuration examples
* Validation cases
* Documentation
* Test cases
* Post-processing tools
* Benchmark studies
* CADSynergy integration workflows

Before contributing data, contributors must confirm that they have the right to publish the submitted data and that it does not contain confidential, proprietary, or personally identifiable information.

A full contribution guide will be added in `CONTRIBUTING.md`.

---

## Data policy

KĀRĀ separates public open data from private or industrial data.

Public repository data may include:

* Public drive cycles
* Synthetic examples
* Educational datasets
* Open benchmark cases
* Non-confidential validation examples

The public repository must not include:

* Confidential OEM data
* Proprietary fuel maps
* Proprietary battery or motor maps
* Raw private GPS traces
* Raw CAN/OBD logs containing sensitive information
* Personally identifiable data
* Any dataset published without proper rights or permission

Private industrial data must be handled outside the public repository through controlled CADSynergy workflows and private storage.

A detailed data policy will be added under:

```text
docs/DATA_POLICY.md
```

---

## License

The KĀRĀ source code is licensed under the **Apache License 2.0**.

Documentation and public datasets may use separate open licenses, such as **CC BY 4.0**, where explicitly stated.

See `LICENSE` for source code licensing details.

---

## Maintained by

KĀRĀ is initiated and maintained by **CADSynergy** as part of the **CADSynergy Open Mobility Lab**.

CADSynergy aims to build an open engineering ecosystem connecting simulation, knowledge, validation, contributors, and industrial collaboration.
