# Package Notebook

The OEA Hybrid Engagement Package includes a single python [notebook](https://github.com/cstohlmann/oea-hybrid-engagement-package/blob/main/notebook/HybridEngagement_enrichment.ipynb) with the following functionality. 
 - <strong>Create Stage 3p Student_pseudo Table:</strong> Aggregates and enriches SIS Student pseudonymized data from Stage 2p (via Microsoft Education Insights module roster tables, listed in the notebook) into a single table, written out to Stage 3p.
 - <strong>Create Stage 3np Student_lookup Table:</strong> Refines and enriches SIS Student non-pseudonymized data from Stage 2np (via Microsoft Education Insights module roster table: Person_lookup) into a single table, written out to stage 3np.
 
 This notebook is automatically imported into your Synapse workspace once you import the [Hybrid Engagement package pipeline template](https://github.com/cstohlmann/oea-hybrid-engagement-package/tree/main/pipeline).

