# XRD Characterization

Once our ceramic is sintered, we characterize its phase composition using X-Ray Diffraction (XRD). In this step, we use NOMAD's automated parsers to extract data directly from the raw instrument files.

## 1. Uploading Raw Data
Starting from our container Experiment Upload, upload the Bruker `.RAW` file.

[⬇️ Download Example XRD .RAW File](assets/HeOx-1001-nsp-sps-900C-10min-01-poliert_exported.raw){ .md-button .nomad-button .md-button--primary }

## 2. Exploring Parsed Data
NOMAD will automatically recognize the `.RAW` extension and trigger the built-in XRD parser. Click the arrow next to the generated entry to access the **Overview** page. Explore this page and also the **DATA** page to investigate the parsed data and corresponding features (e.g., plots).

## 3. Linking the Data

* **Sample Reference:** In the XRD entry (**DATA** tab), a sample is automatically created under `samples`. Link this to the ceramic sample that we created using the edit (pencil) icon in the `composite system reference` field.
* **Instrument Reference:** Click the + next to `instruments`, add/select the instrument used for this XRD measurement from your Instrument Inventory entries.
* **Experiment Reference:** In your **Experiment ELN** (**DATA** tab), open `steps` and add this XRD entry as a step reference.
