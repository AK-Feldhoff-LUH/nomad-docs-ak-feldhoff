# Sample Entry

After documenting the Sol-Gel process, create the physical sample entry directly from the **SolGelSynthesis** ELN and link it as process output.

## Workflow
1. **Open Sol-Gel entry in DATA tab**:
    * Open your `SolGelSynthesis` entry and go to **DATA**.

2. **Add sample output reference**:
    * In the `samples` subsection, click **+**.
    * Go to the `composite system reference` field an click **+** to create a new referenced entry.
    * Select `ELNSample` as inheriting class.
    * Give the new sample a name, e.g. `He01-powder`.
    * Click **CREATE**.

4. **Fill sample identifiers and save**:
    * In the created sample entry, fill at least `name` and `lab_id`.
    * Save the sample entry.

5. **Verify process output in OVERVIEW**:
    * Open the **OVERVIEW** tab of the Sol-Gel entry.
    * Scroll to the **Workflow Graph** card.
    * Confirm the powder sample appears as an output of the synthesis step.
