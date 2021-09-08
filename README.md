[![DOI](https://zenodo.org/badge/378638985.svg)](https://zenodo.org/badge/latestdoi/378638985)
### SARS-CoV-2 variation data

> Data used in __The emergence and ongoing convergent evolution of the SARS-CoV-2 N501Y lineages__

>Darren P Martin, Steven Weaver, Houryiah Tegally, Emmanuel James San, Stephen D Shank, Eduan Wilkinson, Alexander G Lucaci, Jennifer Giandhari, Sureshnee Naidoo, Yeshnee Pillay, Lavanya Singh, Richard J Lessells,  NGS-SA4, COVID-19 Genomics UK (COG-UK), Ravindra K Gupta,, Joel O Wertheim, Anton Nekturenko, Ben Murrell,  Gordon W Harkins, Philippe Lemey, Oscar A MacLean, David L Robertson,Tulio de Oliveira, Sergei L Kosakovsky Pond

This repository contains compressed and anonymized meta data and sequence variants for SARS-CoV-2 genomes. It is used by as data source by a variety of visualization notebooks, including 

1. https://observablehq.com/@spond/sc2-selection-trends
2. https://observablehq.com/@spond/sc2-temporal-selection-trends
3. https://observablehq.com/@spond/spike-trends
4. https://observablehq.com/@spond/sars-cov-2-selected-sites

The contents of the directory are as follows.

1. `sequence-info.json` : compressed partial sequence metadata.
2. `gene/variants-clear.json` : unique haplotypes variation for a given gene
3. `gene/duplicates-compressed.json` : sequence identifiers mapping to a unique haplotype
4. `windowed-sites-fel-*.csv`: site-level selection analysis results (FEL) for GISAID data analyzed in three-month intervals.

The `windowed-sites-fel-current.csv` file contains site-level selection data computed with FEL (3-month windows) and that have been found under selection at least once (p≤0.05). Column headers are as follows

1. `gene` : gene/ORF
2. `site` : site in gene
3. `seqs` : number of representative sequences used for analysis
4. `from` : start of the time interval
5. `to`: end of the time interval
6. `p`: p-value for non-neutrality (positve if alpha < beta, negative otherwise)
7. `alpha` : site MLE estimate for the synonymous rate
8. `beta` : site MLE estimate for the non-synonymous rate
9. `T_int`: total length of internal branches in the gene tree used for inference (subs/site)
10. `T_total`: total length of all branches in the gene tree used for inference (subs/site)
