# Setting Up the Experiment

In NOMAD, data is best organized as an interconnected graph. Instead of keeping synthesis, processing, and characterization in separate, isolated files, we use an overarching **Experiment** entry to link them all together. 

This ensures complete provenance tracking (FAIR data): we know exactly *which* material was made, *how* it was processed, and *what* instruments were used to measure it. 

## 1. Create the Experiment Entry (The "Umbrella")

The `Experiment` entry acts as the central hub. It doesn't contain the raw data itself; rather, it collects references to all the individual steps in your workflow.

1. Navigate to the **Uploads** page and open your current upload.
2. Click the **CREATE FROM SCHEMA** button.
3. In the dropdown, select the built-in **Experiment ELN** schema.
4. Fill in the general metadata:
    - **Title:** e.g., `Synthesis and Characterization of HeOx-1 Ceramic`
    - **Description:** A brief overview of the project goals.
5. Click **Save** (the floppy disk icon). 

> **Note:** We will return to this Experiment entry later. As we complete the Sol-Gel synthesis, Sintering, and SEM/XRD steps, we will link them all back to this central hub!

## 2. Create a Substance Entry (The Material Identity)

Before we describe *how* we made a material, we must define *what* the material is. A **Substance** entry acts as the fundamental chemical identity that can be reused across multiple different experiments.

1. Go back to your Upload overview and click **CREATE FROM SCHEMA**.
2. Select the built-in **Substance ELN** schema.
3. Fill in the identifying details:
    - **Name:** `HeOx-1 Powder`
    - **Description:** (Enter the target stoichiometry, e.g., `La0.5Pr...`)
4. Click **Save**.

> **Why a Substance Entry?** By separating the *Substance* (the identity) from the *Process* (the synthesis), we avoid duplicating chemical information. If you run five different sintering tests on the exact same powder, they all simply link back to this single Substance entry.