## The repository hosts the source for neutrophil proteomics paper

```bash
.
├── 2019-01-25-neutrophil-proteomics-data-analysis-following-influenza-or-bacterial-infection.html
├── 2019-01-25-neutrophil-proteomics-data-analysis-following-influenza-or-bacterial-infection.rmd
├── README.md
└── data
    ├── Neutrophil-proteomics-data-analysis-following-influenza-or-bacterial-infection
    │   ├── 20170428-Proteomics-201611-Requant.txt
    │   ├── 20170428-Proteomics-201612-Requant.txt
    │   ├── 20180206-Proteomics-201801-Requant.txt
    │   ├── 20181018-reactome-pathway-analysis.xlsx
    │   └── all-stat-gene-DAVID-database-GO-cell-compartment.txt
    ├── Rscripts
    │   ├── load_libraries.R
    │   └── utilities.R
    └── pkg_list.txt
```

### Publication 
https://doi.org/10.4049/jimmunol.1900337

### Caution
The kmeans clustering results can't be reproduced in R 3.6 as they changed the behavior of `set.seed`. [PR#17494](https://bugs.r-project.org/bugzilla/show_bug.cgi?id=17494) 

`ComplexHeatmap 2.0` bundled in `Biocondcutor 3.9` can't reproduce the results (mainly on appearance of the order of hierarchy clusters but doesn’t affect data interpretation). 

To reproduce all results, R version should be under 3.6 and Biocondctor should be 3.8. The package information is included in the `pkg_list.txt` file under `data`
