# Sol-Gel Synthesis

Now, we transform liquid precursors into a solid powder. For this step, we use the NOMAD graphical user interface (GUI) with a custom schema and fill it from the provided spreadsheet.

[⬇️ Download synthesis_schema.archive.yaml](assets/synthesis_schema.archive.yaml){ .md-button .nomad-button .md-button--primary }

[⬇️ Download HeOx-1-sg-synthesis.xlsx](assets/HeOx-1-sg-synthesis.xlsx){ .md-button .nomad-button .md-button--primary }

## Workflow: Manual GUI Entry
1. **Inspect the custom schema**:
    * Open `synthesis_schema.archive.yaml` and briefly inspect its structure (`definitions`, section definitions, quantities, and subsections such as `reagents`).
    * For details on creating custom YAML schemas in NOMAD, see: [NOMAD docs - Create custom schema definitions](https://nomad-lab.eu/prod/v1/docs/howto/manage/gui/yaml.html){:target="_blank"}.
2. **Upload the custom schema file**:
    * Starting from our container Experiment Upload (or create a new upload, whichever you prefer), click **DROP FILES HERE OR CLICK TO OPEN DIALOG**, drop in or select `synthesis_schema.archive.yaml`.
    * In practice, this schema can be uploaded and published once, then reused for future syntheses.
3. **Create from custom schema**:
    * Click **CREATE FROM SCHEMA**.
    * Choose **Custom schema**.
    * Click the search icon (magnifying glass)
    * Select the uploaded `synthesis_schema.archive.yaml` (**Sol-gel Synthesis Schema**).
    * Select `SolGelSynthesis` as the section definition.
    * Provide a clear name for the entry, e.g., `SolGel Synthesis`, and click **CREATE**.
    * You will then be on the Sol-Gel ELN **DATA** page.
4. **Fill Reagents (PubChem subsection)**:
    * In the `reagents` subsection, click **+** to add a reagent item.
    * Open [PubChem](https://pubchem.ncbi.nlm.nih.gov/){:target="_blank"} in a separate browser tab.
    * Copy the full molecular formula from your source (e.g. `La(NO3)3*6H2O`) and paste it into the PubChem search.
    * From the PubChem result, copy the **Compound CID**.
    * Back in the ELN reagent item, paste that value into `pub_chem_cid`.
    * Click **Save**. NOMAD queries PubChem and fills the remaining metadata fields automatically.
    * Repeat for each reagent, then set the `role` (`reactant`, `complexing_agent`, `additive`, `solvent`, or `product`) and copy the amount/purity values.
5. **Fill Remaining Quantities**:
    * Using the second tab of the spreadsheet, fill the main process variables in `SolGelSynthesis` (target product info, water settings, pH range, stirring, and calcination/ramp values).
6. **Save and Link**:
    * Save the Sol-Gel entry.
    * Open your **Experiment ELN** entry (**DATA** tab), go to `steps`, and add this Sol-Gel entry as a step reference via the `activity` field: click the edit (pencil) icon, click the SolGel Synthesis entry, save your entry.
    * Navigate to the **OVERVIEW** page of your experiment ELN entry. Scroll down to the bottom to find the **Workflow Graph** card. You will now see the SolGel step and also the corresponding entry reference in the **Entry References** card.
    * Continue to [**c. Sample Entry**](sample_entry.md) to create the physical sample directly from this Sol-Gel entry and link it as process output.
