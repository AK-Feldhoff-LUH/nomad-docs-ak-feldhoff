# Finding Your Data

The true power of NOMAD's structured ELNs and automated parsers becomes apparent when you need to find specific data months or years later. Because we used custom schemas, linked our entries, and parsed our raw files, everything is now completely searchable.

## 1. The Explore Interface
Navigate to the **Explore** section in the main NOMAD navigation bar. This dashboard allows you to search through all data. 

## 2. Basic Search and Filtering
On the left side of the Explore page, you will find the filtering panel. Let's find the specific data we just processed:

* **By Method:** Under the "Method" filter, select **XRD** or **SEM**. This will immediately narrow down the results to only those specific measurement types.
* **By Material:** Under the "Material" or "Elements" filter, you can type the chemical formula (e.g., `La`, `Pr`) to find data specifically related to your Sol-Gel synthesis.
* **By Instrument:** Because we linked our data to the Instrument inventory, you can filter by the specific `Instrument model` (e.g., `JSM-7610F Plus`).

## 3. Advanced Faceted Search
Since we created a custom schema for the Sintering process, you can even search by the exact parameters used during that process!
* Try searching for a specific **Temperature range** to find all samples sintered between, for example, 800 °C and 1000 °C.

## The "FAIR" Payoff
If we had simply uploaded a folder of `.RAW` and `.BMP` files with no metadata, we could only search by file name (Free text). By taking the time to build a workflow graph (**Substance → Process → Measurement → Instrument**), our data is now fully AI-ready and FAIR (Findable, Accessible, Interoperable, and Reusable).