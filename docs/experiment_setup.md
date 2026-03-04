# Experiment Setup

In NOMAD, one can provide context to steps in an experiment by linking them together an interconnected graph (i.e., a workflow graph). Before documenting synthesis and characterization details, create one **Experiment ELN** entry that serves as the central hub for this experiment workflow.

## 1. Create the Experiment ELN entry
The Experiment entry collects references to all process and measurement steps that belong to the same study. On the **Your uploads** page:

a. Click **CREATE A NEW UPLOAD**.

b. Give the Upload a clear name, e.g., `Synthesis and Characterization of HeOx-1 Ceramic`.

b. Click **CREATE FROM SCHEMA**.

c. Select the built-in **Experiment ELN** schema.

d. Give it a clear name, e.g. `Synthesis and Characterization of HeOx-1 Ceramic`.

e. Click **Create**.

f. After creation, the entry opens directly in the **DATA** tab.

## 2. Complete metadata in the DATA tab

a. In the left tree, open `data` and edit the main Experiment quantities.

b. Fill the core fields visible in your Experiment ELN, especially:
    * `name`
    * `startingTime`
    * `tags`
    * `ID`
    * `location`
    * `description`

c. Fill the `experiment_identifiers` subsection analogous to the instrument identifiers in the previous section.

d. Use consistent naming/identifier conventions so this experiment can be found and reused later.

## 3. Use the Experiment as your workflow hub

a. Keep this Experiment entry accessible while working on the next tutorial steps.

b. After each new step (Sol-Gel, Sintering, XRD, SEM), return to the Experiment entry (**DATA** tab), open the `steps` subsection, and add a step reference to that entry.

c. This keeps your full provenance graph in one place.

In practice (outside this tutorial), publish the Experiment entry when the workflow is complete so the final record is immutable and shareable.

