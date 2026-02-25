# Sintering Process

This section documents the sintering of the **HeOx-1** powder into a ceramic using the sintering method.

## Workflow
1.  **Create Entry:** Navigate to your upload and create a new `Sintering` entry.
2.  **Link Substance/Sample:** In the `Input Powder Sample` field, search for and select the **HeOx-1** material identity you created in the previous steps. This establishes the physical provenance of what is being sintered.
3.  **Upload Data:** Drag and drop the raw parameters file into the file field.

    [⬇️ Download sintering.parameters.xlsx](assets/sintering.parameters.xlsx){ .md-button .md-button--primary }

4.  **Manual Entry:** Open the Excel file.
    * Read the values for Temperature and Time (e.g., 900 °C and 15 min).
    * Manually enter them into the `Temperature` and `Duration` fields.
5.  **Save and Link to Experiment:** Click the Save icon. Then, go back to your overarching **Experiment ELN** entry. Under its steps/processes section, reference this new Sintering entry to connect it to your main project graph.

!!! warning "Note on Automation"
    The current Excel file format is unstructured. Automatic parsing is pending a file re-format or a custom Python parser. For now, manual entry is required.