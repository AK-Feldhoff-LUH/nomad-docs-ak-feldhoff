# Sintering Process

This section documents the sintering of the **HeOx-1** powder into a ceramic using the sintering method.

## Workflow
1.  **Create Entry:** Create a new `Sintering` entry.
2.  **Link Sample:** Select the **HeOx-1** powder from the previous task in the `Input Powder Sample` field.
3.  **Upload Data:** Upload the `sintering.parameters.xlsx`.
4.  **Manual Entry:** * Open the Excel file.
    * Read the values for Temperature and Time.
    * Manually enter them into the `Temperature` and `Duration` fields.

> **Note on Automation:** The current Excel file format is unstructured. Automatic parsing is pending a file re-format or a custom Python parser.