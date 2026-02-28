# XRD Characterization

Once our ceramic is sintered, we characterize its phase composition using X-Ray Diffraction (XRD). In this step, we use NOMAD's automated parsers to extract data directly from the raw instrument files.

## 1. Uploading Raw Data
Navigate to your Upload overview. Upload the Bruker `.RAW` file by dragging and dropping it into the NOMAD upload box.

[⬇️ Download Example XRD .RAW File](assets/TwoTheta_scan_scrambled.raw){ .md-button .md-button--primary }

## 2. Exploring Parsed Data
NOMAD will automatically recognize the `.RAW` extension and trigger the built-in XRD parser. Click on the generated Entry to see the extracted diffractogram and metadata visualized automatically!

## 3. Linking the Data 
To ensure FAIR tracking, we must link this measurement to our physical sample and the broader experiment.

* **Sample Reference:** Locate the `Sample` reference field and select your synthesized material/sample.
* **Experiment Reference:** Navigate back to your overarching **Experiment ELN** and link this XRD Characterization entry to the project graph.
