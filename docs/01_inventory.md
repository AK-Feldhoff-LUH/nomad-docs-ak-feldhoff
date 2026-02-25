# I. Creating an Instrument Inventory

Before we can document our specific experiments, we need to register the instruments used in the lab. This creates a persistent "Digital Twin" of our lab equipment, allowing us to track which samples were measured on which machine across any future experiment.

## The Schema
We use a custom `Instrument` schema that records:

* **Manufacturer**: Who made the device (e.g., JEOL).
* **Model**: The specific device model.
* **Serial Number**: For unique identification.

[⬇️ Download inventory_schema.archive.yaml](assets/inventory_schema.archive.yaml){ .md-button .md-button--primary }

## Instructions
1.  **Upload the Schema**: 
    * Download the `inventory_schema.archive.yaml` file above.
    * Drag and drop it into your NOMAD upload space. NOMAD will read this file and automatically add your custom "Instrument" template to the system.
2.  **Create a New Entry**:
    * Click the **CREATE FROM SCHEMA** button.
    * Look through the dropdown list. Because you uploaded the YAML file, you will now see your custom **Instrument** available. Select it.
    * Name the entry: `JEOL-SEM-01`.
3.  **Fill in the Details**:
    * **Manufacturer**: `JEOL`
    * **Model**: `JSM-7610F Plus` (or whichever specific model is used in the AK Feldhoff lab).
    * **Description**: "High-resolution SEM used for microstructure analysis."
4.  **Save**:
    * Click the **Save** icon.
    
!!! info "Linking to Future Experiments"
    This entry acts as an independent asset. It will be referenced directly in the **SEM Characterization** step later to link our images to this specific microscope, ensuring full provenance of our measurement data.