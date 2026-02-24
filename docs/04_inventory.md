# Instrument Inventory

Before we can document our characterization experiments, we need to register the instruments used. This creates a "Digital Twin" of our lab equipment, allowing us to track which samples were measured on which machine.

## The Schema
We use a custom `Instrument` schema that records:

* **Manufacturer**: Who made the device (e.g., JEOL).
* **Model**: The specific device model.
* **Serial Number**: For unique identification.

## Instructions
1.  **Create a New Entry**:
    * Navigate to your upload and click **CREATE FROM SCHEMA**.
    * Select **Instrument** from the dropdown list.
    * Name the entry: `JEOL-SEM-01`.
2.  **Fill in the Details**:
    * **Manufacturer**: `JEOL`
    * **Model**: `JSM-7610F Plus` (or whichever specific model is used in the AK Feldhoff lab).
    * **Description**: "High-resolution SEM used for microstructure analysis."
3.  **Save**:
    * Click the **Save** icon.
    
> **Note**: This entry will be referenced directly in the **Characterization** step to link our SEM images to this specific microscope, ensuring full provenance of our measurement data.