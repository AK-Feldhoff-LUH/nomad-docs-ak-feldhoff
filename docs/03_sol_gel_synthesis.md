# Sol-Gel Synthesis

Now, we transform liquid precursors into a solid powder. Accurate documentation here is critical for reproducibility. For this step, we use the NOMAD graphical user interface (GUI) with a custom schema and fill it from the provided spreadsheet.

[⬇️ Download synthesis_schema.archive.yaml](assets/synthesis_schema.archive.yaml){ .md-button .nomad-button .md-button--primary }

[⬇️ Download HeOx-1-sg-synthesis.xlsx](assets/HeOx-1-sg-synthesis.xlsx){ .md-button .nomad-button .md-button--primary }

## Workflow: Manual GUI Entry
1. **Upload the custom schema file**:
    * On the **Your uploads** page, upload `synthesis_schema.archive.yaml` to your working upload.
    * In practice, this schema can be uploaded and published once, then reused for future syntheses.
2. **Create from custom schema**:
    * Click **CREATE FROM SCHEMA**.
    * Choose **Custom schema**.
    * Select the uploaded `synthesis_schema.archive.yaml`.
    * Select `SolGelSynthesis` as the section definition.
    * You will then be on the Sol-Gel ELN **DATA** page.
3. **Fill Reagents (PubChem subsection)**:
    * In the `reagents` subsection, click **+** to add each reagent.
    * Add one reagent item per substance column in the **HeOx-1** spreadsheet tab (nitrates, EDTA, citric acid, and target product entry).
    * For each reagent, set the `role` (`reactant`, `complexing_agent`, `additive`, `solvent`, or `product`) and copy the amount/purity values.
    * In the PubChem-enabled reagent subsection, enter an identifying value (for example `molecular_formula`, or `pub_chem_cid` when available). NOMAD should fetch the remaining PubChem fields automatically.
4. **Fill Remaining Quantities**:
    * Still using the same spreadsheet, fill the main process variables in `SolGelSynthesis` (target product info, water settings, pH range, stirring, and calcination/ramp values).
    * The **Tabelle1** tab describes the fixed protocol; you only enter its key variable parameters as quantities.
5. **Save and Link**:
    * Save the Sol-Gel entry.
    * Open your **Experiment ELN** entry and add a reference to this synthesis step.
