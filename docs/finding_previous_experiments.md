# III. Finding Previous Experiments

The value of structured ELNs appears when you need to retrieve specific entries later. Because we linked experiment steps, instruments, and measurements, the full workflow is queryable.

## 1. Search by Quantities in EXPLORE
In EXPLORE, use the quantity search bar to add filters.

1. Click the quantity search input and start typing the quantity name.
2. Use autocomplete suggestions to select the exact indexed quantity.
3. Add filter values.
4. Add as many filter tokens as needed to increase search specificity.

Useful quantities for this tutorial include:
* `results.eln.sections` (e.g. `SolGelSynthesis`, `SinteringProcess`, measurement ELNs)
* `results.eln.tags`
* method/instrument/material-related quantities available in your deployment
* custom process quantities from your schemas (e.g. sintering temperature/pressure fields)

Try these example searches (copy/paste):

* `results.eln.sections=SolGelSynthesis`
* `results.eln.sections=SinteringProcess`
* `results.eln.sections=ELNInstrument`
* `results.eln.names=JEOL-SEM-01`
* `results.eln.instruments=JSM-7610F Plus`
* `results.eln.names=sintering data`
* `authors.name=<your name>`
* `entry_name=sintering_data.archive.yaml`
* `mainfile=sintering_data.archive.yaml`
* `upload_id=...` (copy from entry metadata on OVERVIEW)
* `entry_create_time>=2026-02-01` (date/range style queries)

Use the quantity search input with autocomplete. For each example:

1. Type the quantity name.
2. Select it from autocomplete.
3. Enter the value shown.

Use autocomplete to confirm the exact quantity names available in your deployment.

For custom schema quantities, use autocomplete to find the exact indexed path in your deployment, then filter by value (for example sintering temperature or pressure fields).

## 2. Create a Filter Widget with +TERMS
You can create a quick filter widget directly in EXPLORE:

1. Click **+TERMS**.
2. In **X AXIS Search quantity**, enter `entry_type`.
3. Click **Done**.
4. Use the new widget to filter entries by type.

## 3. Notes on Apps and Customization
The default **Entries** app is generic and not optimized for all experimental workflows. However, it is possible to build custom search apps/views tailored to your ELN schemas and lab workflows (see [NOMAD documentation on developing app plugins](https://nomad-lab.eu/prod/v1/develop/docs/howto/plugins/apps.html){:target="_blank"}). A concrete example on NOMAD Central is the [Solar Cell search app](https://nomad-lab.eu/prod/v1/gui/search/solarcells){:target="_blank"}.
