# I. Creating an Instrument Inventory

Before documenting experiments and measurements, register your lab instruments as dedicated ELN entries. This creates reusable metadata records for provenance, so later measurement entries can reference the exact instrument used. In this tutorial, we demonstrate the workflow with one example entry using the built-in **Instrument ELN**.

## Instructions
1. **Create the Instrument ELN entry**:
   * In your upload, click **CREATE FROM SCHEMA**.
   * Select the built-in **Instrument ELN** schema.
   * Give the entry a clear name, e.g. `JEOL-SEM-01`.
   * After creation, NOMAD opens the entry directly in the **DATA** tab.

2. **Inspect the DATA view**:
   * In the left tree, open `data` and inspect the Instrument ELN content there.

3. **Fill core instrument metadata**:
   * In the Instrument ELN quantities, fill key fields such as **name**, **description**, and the instrument-specific fields (e.g. manufacturer/model, when available in your deployment).

4. **Add instrument identifiers**:
    * In the DATA view, open the `instrument_identifiers` / **Readable Identifiers** subsection.
    * Fill the identifier fields used by your group (e.g. institute, owner, short name, lab ID).
    * Use a stable lab ID so this instrument can be found and reused later.

5. **Save**:
    * Click the **Save** icon after editing.

Now this instrument entry can be referenced in measurement entries that used this instrument (for example in SEM/XRD instrument reference fields).

In practice (outside this tutorial), you should publish instrument inventory entries so they are immutable and citable. Recommended workflow:

1. Create one upload containing the currently available instruments in your lab.
2. Publish that upload as the current instrument inventory snapshot.
3. Add new instruments later as separate uploads and publish those as new snapshots.
