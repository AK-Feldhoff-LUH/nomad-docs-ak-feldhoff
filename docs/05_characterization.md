# Characterization: XRD and SEM

Once our ceramic is sintered, we characterize its microstructure and phase composition. In this step, we will use NOMAD's automated parsers to extract data directly from raw instrument files.

## 1. Uploading Raw Data
Navigate to your Upload overview. Select your raw files:
* **XRD:** Upload the Bruker `.RAW` file.
* **SEM:** Upload the JEOL `.TXT` and `.BMP` file pair.
Simply **drag and drop** these files into the NOMAD upload box.

## 2. Exploring Parsed Data
NOMAD will automatically recognize these file extensions and trigger the corresponding parsers. 
* Click on the generated Entry for the SEM image. 
* Notice how the image and its details are automatically extracted and visualized!

## 3. Linking the Data (Placeholder)
To ensure FAIR tracking, we must link these measurements to our physical sample and the specific microscope used.
* **Sample Reference:** [TODO: Add instructions to link to the Sintered Pellet]
* **Instrument Reference:** [TODO: Add instructions to link to the JEOL SEM created in the Inventory step]

## 3. Linking the Data 
To ensure FAIR tracking, we must link these measurements to our physical sample and the specific microscope used. 

1. **Sample Reference:** In the parsed measurement entry, locate the `Sample` reference field. Search for and select the **HeOx-1** Substance you created earlier.
2. **Instrument Reference:** Locate the `Instrument` reference field and select the **JEOL-SEM-01** entry you created in the Inventory step.
3. **Experiment Reference:** Finally, navigate back to your overarching **Experiment ELN**. Under its process/measurement steps, link this new Characterization entry to connect it to your main project graph.