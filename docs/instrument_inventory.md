# I. Creating an Instrument Inventory

Before documenting experiments and measurements, register your lab instruments as dedicated ELN entries. This creates reusable metadata records for provenance, so later measurement entries can reference the exact instrument used. In this tutorial, we demonstrate the workflow with one example entry using the built-in **Instrument ELN**.

## Instructions
1. **Create the Instrument ELN entry**:
    * Open the **Your uploads** page (`Publish` > `Uploads`) and open your working upload.
    * Click **CREATE A NEW UPLOAD**
    * Click **CREATE FROM SCHEMA**.
    * Select the built-in **Instrument ELN** schema.
    * Give the entry a clear name, e.g. `JEOL-SEM-01`.
    * After creation, NOMAD opens the entry directly in the **DATA** tab.

2. **Inspect the DATA view**:
    * In the left tree, open `data` and inspect the Instrument ELN content there.

3. **Fill core instrument metadata**:
    * In the Instrument ELN quantities, fill key quantities such as **name**, **id**, **description**, etc.

4. **Add instrument identifiers**:
    * Open the `instrument_identifiers` subsection underneath the key quantities.
    * Fill the identifier fields used by your group (e.g. institute, owner, short name).
    * Note: the lab ID will be auto-generated upon save.

5. **Save**:
    * Click the **Save** icon after editing.

6. **Rename you Inventory Upload**
    * Navigate to the upload page: Click **Upload** in the navigation list at the top, or go to **Overview** and then click on the **Upload id** link in the left-hand column.
    * Click the edit (pencil) icon to the left of "unamed upload" at the top, and rename the upload "Instrument Inventory".

Now this instrument entry can be referenced in measurement entries that used this instrument. We will demonstrate this explicitly later in the tutorial.

In practice (outside this tutorial), you should publish instrument inventory entries so they are immutable and citable. Recommended workflow:

* Create one upload containing the currently available instruments in your lab.
* Publish that upload as the current instrument inventory snapshot.
* Add new instruments later as separate uploads and publish those as new snapshots.