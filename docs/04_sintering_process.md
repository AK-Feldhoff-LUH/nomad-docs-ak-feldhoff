# Sintering Process

This section documents the thermal treatment used to sinter the **HeOx-1** powder into a dense ceramic. 

Instead of manually typing values into the graphical interface like we did for the Sol-Gel synthesis, we will use a more advanced NOMAD feature: **instantiating a schema via a Data file**. 

## The Two-File Approach
In NOMAD, a schema is just a blank template. You can create a separate file that contains your actual data and tells NOMAD *which* template to use via an `m_def` (meta-definition) pointer.

Download these three files to see how it works:
[⬇️ Download sintering_schema.archive.yaml](assets/sintering_schema.archive.yaml){ .md-button .md-button--primary }
[⬇️ Download sintering_data.archive.yaml](assets/sintering_data.archive.yaml){ .md-button .md-button--primary }
[⬇️ Download sintering.parameters.xlsx](assets/sintering.parameters.xlsx){ .md-button }

## Workflow: Data Instantiation
1. **Upload the Files:** Drag and drop all three downloaded files (`sintering_schema.archive.yaml`, `sintering_data.archive.yaml`, and the `.xlsx` file) directly into your NOMAD upload space.
2. **Inspect the Magic:** Click on the generated `sintering_data` entry. 
    * Notice how NOMAD automatically read the `m_def` line, connected the data to your schema, and generated a fully populated graphical entry!
    * You will see the **900 °C**, **15 min**, and **50 MPa** values (extracted from the Excel file) already filled in.
3. **Save and Link**:
    * Save the generated sintering entry if needed.
    * Go back to your overarching **Experiment ELN** and link this step to your project graph.
    * If your schema provides a sample/material reference field, link it to the corresponding synthesized material context from Sol-Gel.

!!! tip "Why upload the Excel file if the YAML already has the data?"
    You might wonder why we still upload the raw `.xlsx` file if our `sintering_data.archive.yaml` already contains the numbers. This is a core principle of **FAIR data**: always keep your raw "ground truth" files linked to your extracted metadata for perfect provenance. Furthermore, in a fully automated workflow, a custom NOMAD parser would actually read this Excel file to generate that data YAML automatically!
    
