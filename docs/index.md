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

### Create a NOMAD account at the [NOMAD Central Deployment](https://nomad-lab.eu/prod/v1/gui/search/entries){:target="\_blank"}

Click `LOGIN/REGISTER` at the top right.

!!! warning "Attention"
    This is a public database for sharing your research data. For day to day usage, you may want to use your institute's NOMAD Oasis Installation, depending on your group's research data management protocols.
