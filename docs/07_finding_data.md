# III. Finding Previous Experiments

The value of structured ELNs appears when you need to retrieve specific entries later. Because we linked experiment steps, instruments, and measurements, the full workflow is queryable.

## 1. Start Search from Your uploads
1. On the **Your uploads** page, open one of your entries.
2. Use the search action (Search ELN / Explore Entries) to jump into **EXPLORE** with your current upload context.

## 2. Search by Quantities in EXPLORE
In EXPLORE, use the quantity search bar to add filters.

1. Click the quantity search input and start typing the quantity name.
2. Use autocomplete suggestions to select the exact indexed quantity.
3. Add filter values and combine multiple filters.

Typical useful quantities for this tutorial include:
* `results.eln.sections` (e.g. `SolGelSynthesis`, `SinteringProcess`, measurement ELNs)
* `results.eln.tags`
* method/instrument/material-related quantities available in your deployment
* custom process quantities from your schemas (e.g. sintering temperature/pressure fields)

## 3. Demo Searches (Copy/Paste)
Use the quantity search input with autocomplete. For each example:

1. Type the quantity name.
2. Select it from autocomplete.
3. Enter the value shown.

Try these first:

* `results.eln.sections=SolGelSynthesis`
* `results.eln.sections=SinteringProcess`
* `results.eln.sections=ELNInstrument`
* `results.eln.names=JEOL-SEM-01`
* `results.eln.instruments=JSM-7610F Plus`
* `results.eln.names=sintering data`

Then combine filters, for example:

* `results.eln.sections=SinteringProcess` + `results.eln.names=sintering data`
* `results.eln.sections=ELNInstrument` + `results.eln.names=JEOL-SEM-01`

You can also search with high-level metadata, for example:

* `authors.name=Markus Scheidgen`
* `entry_name=sintering_data.archive.yaml`
* `mainfile=sintering_data.archive.yaml`
* `upload_id=...` (copy from entry metadata on OVERVIEW)
* `entry_create_time>=2026-02-01` (date/range style queries)

Use autocomplete to confirm the exact quantity names available in your deployment.

For custom schema quantities, use autocomplete to find the exact indexed path in your deployment, then filter by value (for example sintering temperature or pressure fields).

## 4. Notes on Apps and Customization
The default **Entries** app is generic and not optimized for all experimental workflows.

For production usage, you can build custom search apps/views tailored to your ELN schemas and lab workflows (see NOMAD documentation on developing plugins and apps).

If we had uploaded only raw files without structured metadata and links, search would be limited mostly to filenames and free text. By keeping an Experiment-centered ELN graph, your data remains findable and reusable.
