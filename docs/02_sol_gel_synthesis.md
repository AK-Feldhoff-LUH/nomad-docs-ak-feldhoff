# Sol-Gel Synthesis of Oxide Powders

This section of the tutorial guides you through documenting the primary stage of material preparation: the **Sol-Gel Synthesis**. Before a material can be sintered into a dense ceramic, its chemical "DNA" is established during the powder synthesis phase. 

## Overview
In this step, we transform liquid precursors into a solid powder (e.g., the **HeOx-1** sample). Accurate documentation at this stage is critical for reproducibility, as the stoichiometry and mass yield of the powder directly influence the properties of the final ceramic.

## The Synthesis Schema
We have provided a custom NOMAD schema: `synthesis_schema.archive.yaml`. This schema is built upon the **Sample ELN** base class, which allows it to integrate seamlessly with NOMAD’s search and laboratory management tools. 

### Key Features:
* **Sample Tracking**: Assign unique Lab IDs to maintain a clear lineage from powder to ceramic. 
* **Precursor Management**: Log the specific chemical "building blocks" (Nitrates, Oxides, etc.) used in the reaction. 
* **Quantitative Data**: Record the precise mass yield of the synthesized powder in grams.

## How to Proceed
1. **Upload the Schema**: Ensure `synthesis_schema.archive.yaml` is in your NOMAD upload.
2. **Create the Entry**: Select "New Entry" and choose **SolGelPowder** as the definition.
3. **Populate Data**: Use your synthesis log (see `HeOx-1-sg-synthesis.xlsx` for reference) to fill in the precursor list and the final mass.