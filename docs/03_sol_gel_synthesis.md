# Sol-Gel Synthesis

Now, we transform liquid precursors into a solid powder. Accurate documentation here is critical for reproducibility. For this step, we will use the NOMAD graphical user interface (GUI) to manually fill out a custom schema.

[⬇️ Download synthesis_schema.archive.yaml](assets/synthesis_schema.archive.yaml){ .md-button .md-button--primary }
[⬇️ Download HeOx-1-sg-synthesis.xlsx](assets/HeOx-1-sg-synthesis.xlsx){ .md-button .md-button--primary }

## Workflow: Manual GUI Entry
1. **Upload the Schema**: Ensure `synthesis_schema.archive.yaml` is uploaded to your workspace.
2. **Create the Entry**: Click the **CREATE FROM SCHEMA** button. Because you uploaded the schema, NOMAD will let you choose **SolGelPowder** from the dropdown.
3. **Populate Data**: Open the provided `HeOx-1-sg-synthesis.xlsx` Excel file. Read the precursor list and the final mass yield, and type them manually into the NOMAD interface.
4. **Link it**: Ensure you link this synthesis step to both your overarching **Experiment** and your target **Substance**.


!!! tip "The Value of the GUI"
    Using the graphical interface is great for one-off syntheses. However, in the next step (Sintering), we will learn how to bypass manual typing by providing NOMAD directly with a data file!