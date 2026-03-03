# Tutorial: Sol-Gel Synthesis and Characterization Workflow in NOMAD
<span style="display: block; margin-top: -0.55em; margin-bottom: 0.45em; font-size: 1.150em; color: gray;"><em>Created by</em> <img src="assets/glaide_logo_long_white.png" alt="Glaide logo" style="height: 1.986em; vertical-align: middle;" /></span>

This tutorial walks through a complete **HeOx ceramic** workflow in NOMAD, from process documentation to measurement provenance. You will create an experiment hub, document synthesis and sintering with structured ELN schemas, and connect parsed XRD/SEM data to the same workflow graph.

## What you'll do:

- [**I. Creating an Instrument Inventory**](01_inventory.md)
- **II. Documenting an Experiment**
    - [**a. Experiment Setup**](02_experiment_substance.md)
    - [**b. Sol-Gel Synthesis**](03_sol_gel_synthesis.md)
    - [**c. Sintering Process**](04_sintering_process.md)
    - [**d. XRD Characterization**](05_xrd.md)
    - [**e. SEM Characterization**](06_sem.md)
- [**III. Finding Previous Experiments**](07_finding_data.md)

## At the end of this tutorial, you will be able to:
- Create and maintain an **Experiment-centered ELN graph** across process and measurement entries.
- Capture synthesis inputs via repeatable **reagents** and key process variables in a custom schema.
- Use both **manual GUI entry** and **data-instantiated schema entries**.
- Preserve provenance by linking **raw files**, **parsed metadata**, **sample context**, and **instrument records**.
- Efficiently **search and filter** entries using methods, ELN sections, materials, and instrument metadata.

## ⚙️ Tutorial Preparation

### Open the Feldhoff NOMAD Oasis

Start the tutorial by opening the [Feldhoff NOMAD Oasis](https://nomad.pci.uni-hannover.de/nomad-oasis/gui/about/information){:target="\_blank"} and logging in with your existing account.
