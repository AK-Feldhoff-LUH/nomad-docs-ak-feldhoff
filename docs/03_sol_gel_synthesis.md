# Sol-Gel Synthesis

Now, we transform liquid precursors into a solid powder. Accurate documentation here is critical for reproducibility. For this step, we use the NOMAD graphical user interface (GUI) with a custom schema and fill it from the provided spreadsheet.

[⬇️ Download synthesis_schema.archive.yaml](assets/synthesis_schema.archive.yaml){ .md-button .md-button--primary }
[⬇️ Download HeOx-1-sg-synthesis.xlsx](assets/HeOx-1-sg-synthesis.xlsx){ .md-button .md-button--primary }

## Workflow: Manual GUI Entry
1. **Upload the Schema**: Ensure `synthesis_schema.archive.yaml` is uploaded to your workspace.
2. **Create the Entry**: Click **CREATE FROM SCHEMA** and select your custom **SolGelSynthesis** template.
3. **Fill Reagents**:
    * In the repeating `reagents` subsection, add one item per substance column from the **HeOx-1** tab (e.g., nitrates, EDTA, citric acid, and the target product formula column).
    * For each reagent, set its role (`reactant`, `complexing_agent`, `additive`, `solvent`, or `product`) and transfer the amount/purity values from the spreadsheet.
    * Use the built-in PubChem fields where useful (e.g., CID, names, formula metadata).
4. **Fill Remaining Quantities**:
    * Still using the same spreadsheet, fill the main process variables in `SolGelSynthesis` (target product info, water settings, pH range, stirring, and calcination/ramp values).
    * The **Tabelle1** tab describes the fixed protocol; you only enter its key variable parameters as quantities.
5. **Link it**: Ensure you link this synthesis step to your overarching **Experiment** using the reference fields.

!!! tip "The Value of the GUI"
    Using the graphical interface is great for one-off syntheses. However, in the next step (Sintering), we will learn how to bypass manual typing by providing NOMAD directly with a data file!
