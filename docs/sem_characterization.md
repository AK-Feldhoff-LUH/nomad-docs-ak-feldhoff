# SEM Characterization

Next, we characterize the microstructure of our sintered ceramic using Scanning Electron Microscopy (SEM). 

## 1. Uploading Raw Data
Starting from our container Experiment Upload, upload the JEOL `.TXT` and `.BMP` file pair.

<a class="md-button nomad-button md-button--primary" href="assets/HeOx-1004-sg-sps-900C-15min-polished-01.txt" download>⬇️ Download SEM metadata .TXT File</a>
<a class="md-button nomad-button md-button--primary" href="assets/HeOx-1004-sg-sps-900C-15min-polished-01.bmp" download>⬇️ Download SEM image .BMP File</a>

## 2. Exploring Parsed Data
NOMAD's SEM parser will automatically pair these files together. Click on the generated entry. Notice how the image, scale bar, and magnification details are automatically extracted and visualized.

## 3. Linking the Data 
Just as with the XRD data, we must establish our provenance graph.

* **Sample Reference:** In the SEM entry (**DATA** tab), click the + next to `samples` to add a sample reference, then link it to the ceramic sample we created using the edit (pencil) icon in the `composite system reference` field.
* **Instrument Reference:** Click the + next to `instruments`, add/select the instrument used for this SEM measurement from your Instrument Inventory entries.
* **Experiment Reference:** In your **Experiment ELN** (**DATA** tab), open `steps` and add this SEM entry as a step reference.
