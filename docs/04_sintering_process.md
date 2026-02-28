# Sintering Process

This section documents the thermal treatment used to sinter the **HeOx-1** powder into a dense ceramic.

Instead of manual entry (as in Sol-Gel), this step demonstrates **schema instantiation from a data file**.

## Schema + Data Files
In NOMAD, a schema defines the structure, while a separate data file provides concrete values and points to that schema via `m_def`.

Download these three files to see how it works:
[⬇️ Download sintering_schema.archive.yaml](assets/sintering_schema.archive.yaml){ .md-button .nomad-button .md-button--primary }

[⬇️ Download sintering_data.archive.yaml](assets/sintering_data.archive.yaml){ .md-button .nomad-button .md-button--primary }

[⬇️ Download sintering.parameters.xlsx](assets/sintering.parameters.xlsx){ .md-button .nomad-button }

## Workflow: Data Instantiation
1. **Upload the Files:** Drag and drop all three downloaded files (`sintering_schema.archive.yaml`, `sintering_data.archive.yaml`, and the `.xlsx` file) directly into your NOMAD upload space.
2. **Open the generated entry (OVERVIEW):**
    * Click `sintering_data.archive.yaml` in your upload.
    * On the **OVERVIEW** page, confirm that NOMAD recognized the method as `SinteringProcess` and created the corresponding entry.
    * In the entry card, verify that key process quantities (e.g. final temperature, dwell time, applied pressure) are already populated.
3. **Inspect/edit in DATA tab:**
    * Open the **DATA** tab to inspect or refine the instantiated ELN fields.
    * Save if you make any edits.
4. **Save and Link**:
    * Go back to your overarching **Experiment ELN** and link this step to your project graph.
    * If your schema provides a sample/material reference field, link it to the corresponding synthesized material context from Sol-Gel.

Keep the accompanying parameter/raw file in the upload together with schema and instantiated data, so the provenance of extracted metadata remains transparent.

