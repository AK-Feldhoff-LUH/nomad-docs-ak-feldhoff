# SEM Characterization

Next, we characterize the microstructure of our sintered ceramic using Scanning Electron Microscopy (SEM). 

## 1. Uploading Raw Data
On the **Your uploads** page, upload the JEOL `.TXT` and `.BMP` file pair to your working upload.

[⬇️ Download SEM metadata .TXT File](assets/HeOx-1004-sg-sps-900C-15min-polished-01.txt){ .md-button .nomad-button .md-button--primary }
[⬇️ Download SEM image .BMP File](assets/HeOx-1004-sg-sps-900C-15min-polished-01.bmp){ .md-button .nomad-button .md-button--primary }

## 2. Exploring Parsed Data
NOMAD's SEM parser will automatically pair these files together. Click on the generated entry. Notice how the image, scale bar, and magnification details are automatically extracted and visualized.

## 3. Linking the Data 
Just as with the XRD data, we must establish our provenance graph.

* **Sample Reference:** In the SEM entry (**DATA** tab), set the sample link in `samples` (or `Sample`) to your synthesized material/sample context.
* **Instrument Reference:** In `instruments`, add/select the **JEOL-SEM-01** entry you created in Step I.
* **Experiment Reference:** In your **Experiment ELN** (**DATA** tab), open `steps` and add this SEM entry as a step reference. Your digital workflow is now complete.
