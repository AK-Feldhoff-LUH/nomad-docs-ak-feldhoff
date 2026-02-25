In NOMAD, data is best organized as an interconnected graph. Before we document the synthesis parameters, we must set up our **Experiment** (the umbrella linking all steps) and our **Substance** (the chemical identity).

## 1. Create the Experiment Entry (The "Umbrella")
The `Experiment` entry acts as the central hub. It collects references to all the individual steps in your workflow.

1. Navigate to the **Uploads** page and open your current upload.
2. Click the **CREATE FROM SCHEMA** button.
3. Select the built-in **Experiment ELN** schema.
4. Fill in the **Title** (e.g., `Synthesis and Characterization of HeOx-1 Ceramic`) and click **Save**. 

!!! tip "Looking Ahead"
    As we complete the Sol-Gel synthesis, Sintering, and Characterization steps, we will link them all back to this central hub!

## 2. Create a Substance Entry (The Material Identity)
A **Substance** entry acts as the fundamental chemical identity that can be reused across multiple different physical samples.

1. Go back to your Upload overview and click **CREATE FROM SCHEMA**.
2. Select the built-in **Substance ELN** schema.
3. Name it `HeOx-1 Powder` and provide its target stoichiometry. Click **Save**.

