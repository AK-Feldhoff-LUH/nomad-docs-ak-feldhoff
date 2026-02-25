# Sol-Gel Synthesis

Now, we transform liquid precursors into a solid powder. Accurate documentation here is critical for reproducibility. For this step, we will use the NOMAD graphical user interface (GUI) to manually fill out a custom schema based on our lab notes.

[⬇️ Download synthesis_schema.archive.yaml](assets/synthesis_schema.archive.yaml){ .md-button .md-button--primary }
[⬇️ Download HeOx-1-sg-synthesis.xlsx](assets/HeOx-1-sg-synthesis.xlsx){ .md-button .md-button--primary }

## Workflow: Manual GUI Entry
1. **Upload the Schema**: Ensure `synthesis_schema.archive.yaml` is uploaded to your workspace.
2. **Create the Entry**: Click **CREATE FROM SCHEMA** and select your custom **SolGelPowder** template.
3. **Populate Data**: Open the provided `HeOx-1-sg-synthesis.xlsx` Excel file: 
    * Read the Water Volume (e.g., 200 ml).
    * Read the Calcination Temperature (e.g., 750 °C).
    * Read the Calcination Time (e.g., 5 h).
    * Type these values manually into the corresponding fields in the NOMAD interface.
4. **Link it**: Ensure you link this synthesis step to your overarching **Experiment** using the reference fields.

!!! tip "The Value of the GUI"
    Using the graphical interface is great for one-off syntheses. However, in the next step (Sintering), we will learn how to bypass manual typing by providing NOMAD directly with a data file!