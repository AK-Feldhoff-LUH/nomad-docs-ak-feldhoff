# SEM Characterization

Next, we characterize the microstructure of our sintered ceramic using Scanning Electron Microscopy (SEM). 

## 1. Uploading Raw Data
Starting from our container Experiment Upload, upload the contents of the provided `.zip` archive, which contains multiple JEOL SEM scans (paired or standalone `.TXT` and `.BMP` files).

<a class="md-button nomad-button md-button--primary" href="assets/HeOx-1_SEM_scans.zip" download>⬇️ Download SEM Scans Archive (.zip)</a>

## 2. Exploring Parsed Data
Take the following steps to store and visualize your data on NOMAD:

* **Create an Entry**: Click **CREATE FROM SCHEMA**. In the built-in schemas field, select the **SEM Experiment (JEOL)** schema and give it a proper name, e.g., `SEM_HeOx-1`. Click **CREATE**.
* **Review the Data**: NOMAD will automatically create the entry, populate it with data from the uploaded files, and open the **DATA** tab. Look for the `events` subsection to find the parsed data for all of your uploaded SEM files (both paired and standalone). For each event, you can inspect the corresponding `settings` and its relevant plot. Here, you can add or adjust any additional information for your scans. Be sure to click the **Save** icon in the top right corner when finished.
* **Analyze the Images**: Switch to the **OVERVIEW** tab to analyze the images generated from your `.bmp` files in the plot panel. Since you have multiple scans, you can easily switch between them using the toggle icon in the top-left corner of the panel.


## 3. Linking the Data 
Just as with the XRD data, we must establish our provenance graph.

* **Sample Reference:** In the SEM entry (**DATA** tab), click the + next to `samples` to add a sample reference, then link it to the ceramic sample we created using the edit (pencil) icon in the `composite system reference` field.
* **Instrument Reference:** Click the + next to `instruments`, add/select the instrument used for this SEM measurement from your Instrument Inventory entries.
* **Experiment Reference:** In your **Experiment ELN** (**DATA** tab), open `steps` and add this SEM entry as a step reference.
