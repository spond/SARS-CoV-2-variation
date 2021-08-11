[![DOI](https://zenodo.org/badge/378638985.svg)](https://zenodo.org/badge/latestdoi/378638985)
### SARS-CoV-2 variation data

> Data used in __The emergence and ongoing convergent evolution of the SARS-CoV-2 N501Y lineages__

>Darren P Martin, Steven Weaver, Houryiah Tegally, Emmanuel James San, Stephen D Shank, Eduan Wilkinson, Alexander G Lucaci, Jennifer Giandhari, Sureshnee Naidoo, Yeshnee Pillay, Lavanya Singh, Richard J Lessells,  NGS-SA4, COVID-19 Genomics UK (COG-UK), Ravindra K Gupta,, Joel O Wertheim, Anton Nekturenko, Ben Murrell,  Gordon W Harkins, Philippe Lemey, Oscar A MacLean, David L Robertson,Tulio de Oliveira, Sergei L Kosakovsky Pond

This repository contains compressed and anonymized meta data and sequence variants for SARS-CoV-2 genomes. It is used by as data source by a variety of visualization notebooks, including 

1. https://observablehq.com/@spond/sc2-selection-trends
2. https://observablehq.com/@spond/sc2-temporal-selection-trends
3. https://observablehq.com/@spond/spike-trends

The contents of the directory are as follows.

1. `sequence-info.json` : compressed partial sequence metadata.
2. `gene/variants-clear.json` : unique haplotypes variation for a given gene
3. `gene/duplicates-compressed.json` : sequence identifiers mapping to a unique haplotype
4. `windowed-sites-fel-*.csv`: site-level selection analysis results (FEL) for GISAID data analyzed in three-month intervals.
