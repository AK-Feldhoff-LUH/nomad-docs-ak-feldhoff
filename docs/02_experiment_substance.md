# Experiment Setup

In NOMAD, data is best organized as an interconnected graph. Before documenting synthesis and characterization details, create one **Experiment ELN** entry that serves as the central hub for this workflow.

## 1. Create the Experiment ELN entry
The Experiment entry collects references to all process and measurement steps that belong to the same study.

1. On the **Your uploads** page, open your current upload.
2. Click the **CREATE FROM SCHEMA** button.
3. Select the built-in **Experiment ELN** schema.
4. Give it a clear title, e.g. `Synthesis and Characterization of HeOx-1 Ceramic`.
5. Save the entry.
6. After creation, the entry opens directly in the **DATA** tab.

## 2. Complete metadata in the DATA tab
1. In the left tree, open `data` and edit the main Experiment quantities.
2. Fill the core fields visible in your Experiment ELN, especially:
   * `name`
   * `startingTime`
   * `tags`
   * `ID`
   * `location`
   * `description`
3. Open the `experiment_identifiers` subsection (Readable Identifiers) and fill your group-specific identifiers (e.g. institute, owner, short name, lab ID).
4. Use consistent naming/identifier conventions so this experiment can be found and reused later.

## 3. Use the Experiment as your workflow hub
1. Keep this Experiment entry accessible while working on the next tutorial steps.
2. After each new step (Sol-Gel, Sintering, XRD, SEM), return to the Experiment entry (**DATA** tab), open the `steps` subsection, and add a step reference to that entry.
3. This keeps your full provenance graph in one place.

In practice (outside this tutorial), publish the Experiment entry when the workflow is complete so the final record is immutable and shareable.

