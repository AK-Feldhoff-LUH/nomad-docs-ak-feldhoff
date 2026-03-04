# Sintering Process

This section documents the thermal treatment used to sinter the **HeOx-1** powder into a dense ceramic.

Instead of manual entry (as in Sol-Gel), this step demonstrates **schema instantiation from a data file**.

## Example Data

[⬇️ Download sintering_schema.archive.yaml](assets/sintering_schema.archive.yaml){ .md-button .nomad-button .md-button--primary }

[⬇️ Download sintering_data.archive.yaml](assets/sintering_data.archive.yaml){ .md-button .nomad-button .md-button--primary }

[⬇️ Download sintering.parameters.xlsx](assets/sintering.parameters.xlsx){ .md-button .nomad-button }

## Workflow
1. **Inspect the files first:**
    * Open `sintering_schema.archive.yaml` and `sintering_data.archive.yaml` in your editor.
    * The schema file defines the structure of the `SinteringProcess` entry (which quantities and subsections exist).
    * The data file contains the concrete values to populate those quantities for this specific run.
2. **Upload the Files:** Starting from our container Experiment Upload, click **DROP FILES HERE OR CLICK TO OPEN DIALOG** to upload the schema (`sintering_schema.archive.yaml`) and data (`sintering_data.archive.yaml`) files. The `.xlsx` file can also be uploaded for storage of original raw data as needed. Multiple files can be uploaded at once by compressing them into the `.zip` format.
3. **Open the generated entry (OVERVIEW):**
    * Click `sintering_data.archive.yaml` in your upload.
    * On the **OVERVIEW** page, confirm that NOMAD recognized the method as `SinteringProcess` and created the corresponding entry.
    * In the entry card, verify that key process quantities (e.g. final temperature, dwell time, applied pressure) are already populated.
4. **Inspect/edit in DATA tab:**
    * Open the **DATA** tab to inspect or refine the instantiated ELN fields.
    * Save if you make any edits.
5. **Create a post-sintering sample (He01 ceramic)**:
    * In the `SinteringProcess` entry (**DATA** tab), go to the `samples` subsection and click **+**.
    * Go to the `composite system reference` field and click **+** to create a new referenced entry.
    * Select `ELNSample` as inheriting class.
    * Give the new sample a name, e.g. `He01-ceramic`.
    * Click **CREATE**.
    * In the created sample entry, fill at least `name` and `lab_id`.
    * Save the sample entry.
    * Open the **OVERVIEW** tab of the sintering entry and confirm in the **Workflow Graph** card that this ceramic sample appears as output of the sintering step.

6. **Save and Link**:
    * Go back to your **Experiment ELN** (**DATA** tab), open `steps`, and add this sintering entry as a step reference by searching through `activity` field.
