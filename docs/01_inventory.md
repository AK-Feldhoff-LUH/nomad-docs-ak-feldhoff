# I. Creating an Instrument Inventory

Before we can document our specific experiments, we need to register the instruments used in the lab. This creates a persistent "Digital Twin" of our lab equipment, allowing us to track which samples were measured on which machine across any future experiment. For this purpose, we will use NOMAD's built-in **Instrument** schema. This standardizes our data and ensures it is fully compatible with the broader FAIRmat ecosystem.

## Instructions
1.  **Create a New Entry**:
    * Navigate to your upload and click the **CREATE FROM SCHEMA** button.
    * In the dropdown list, search for and select the built-in **Instrument** (or **Instrument ELN**) schema.
    * Give your entry a clear, identifiable name: `JEOL-SEM-01`.
    
2.  **Fill in the Details**:
    * Explore the built-in fields provided by NOMAD. 
    * Fill in the **Manufacturer** (e.g., `JEOL`) and the **Model** (e.g., `JSM-7610F Plus`).
    * Add a brief **Description**: "High-resolution SEM used for microstructure analysis."
    
3.  **Save**:
    * Click the **Save** (floppy disk) icon.

!!! info "Linking to Future Experiments"
    This entry acts as an independent asset. It will be referenced directly in the **SEM Characterization** step later to link our images to this specific microscope, ensuring full provenance of our measurement data.

