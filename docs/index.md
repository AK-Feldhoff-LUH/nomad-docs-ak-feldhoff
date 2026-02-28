# Tutorial: Sol-Gel Synthesis and Characterization Workflow in NOMAD

This tutorial walks through a complete **HeOx ceramic** workflow in NOMAD, from process documentation to measurement provenance. You will create an experiment hub, document synthesis and sintering with structured ELN schemas, and connect parsed XRD/SEM data to the same workflow graph.

## What you'll do:

- 🔧 [**Create an instrument inventory**](01_inventory.md) for reusable provenance links.
- 🧭 [**Set up an experiment hub**](02_experiment_substance.md) to connect all workflow steps.
- 🧪 [**Document synthesis and sintering**](03_sol_gel_synthesis.md) with custom schemas and structured quantities.
- 📥 [**Upload and parse XRD/SEM raw files**](05_xrd.md) and link measurements to experiment context.
- 🔎 [**Search and filter your results**](07_finding_data.md) using structured metadata.

## At the end of this tutorial, you will be able to:
- Create and maintain an **Experiment-centered ELN graph** across process and measurement entries.
- Capture synthesis inputs via repeatable **reagents** and key process variables in a custom schema.
- Use both **manual GUI entry** and **data-instantiated schema entries**.
- Preserve provenance by linking **raw files**, **parsed metadata**, **sample context**, and **instrument records**.
- Efficiently **search and filter** entries using methods, ELN sections, materials, and instrument metadata.

## ⚙️ Tutorial Preparation

### Open the Feldhoff NOMAD Oasis

Start the tutorial by opening the [Feldhoff NOMAD Oasis](https://nomad.pci.uni-hannover.de/nomad-oasis/gui/about/information){:target="\_blank"} and logging in with your existing account.

!!! warning "Attention"
    This tutorial is intended for the Feldhoff group Oasis environment. If you are working in a different NOMAD deployment, adapt the upload and sharing steps to your local setup.
