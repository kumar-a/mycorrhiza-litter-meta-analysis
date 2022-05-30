# Effects of mycorrhizal fungi on litter decomposition rate in the forest ecosystems: A meta-analysis
**Authors:** Meenu Patil, [Abhishek Kumar](https://akumar.netlify.app/), Pardeep Kumar, Anand Narain Singh[\*](mailto:dranand1212@gmail.com)  
**Affiliation:** *Soil Ecosystem and Restoration Ecology Lab, Department of Botany, Panjab University, Chandigarh 160014, India*

## Directory structure
```
.
|-- data
      |-- bib
            |-- gs-md.bib
            |-- gs-mna.bib
            |-- scopus.bib
            |-- uniqueref.ris
            |-- wos1.bib
            |-- wos2.bib
            |-- wos3.bib
      |-- Fig1.svg
      |-- mass_remaining.csv
      |-- phylo.tre
      |-- raw_entry1991.csv
      |-- species_classification.csv
      |-- study_metadata.csv
|-- meta-analysis.rmd
|-- refs.bib
```            

## Description of files

| File name	                                                     | Description |  
|----------------------------------------------------------------|-------------|  
| [gs-md.bib](/data/bib/gs-md.bib)                               | Bibliographic records obtained from Google Scholar after searching *“mycorrhiza decomposition”* |  
| [gs-mna.bib](/data/bib/gs-mna.bib)	                       | Bibliographic records obtained from Google Scholar after searching *“mycorrhiza nutrient acquisition”* |
| [scopus.bib](/data/bib/scopus.bib)	                       | Bibliographic records obtained from Scopus using the search string: *(mycorrhiza\* OR ectomycorrhiza\* OR "saprotrophic fungi" OR plant-fung\*) AND (litter OR "litter decay" OR (litter AND decompos\*) OR decomposition OR "nutrient acquisition") AND (forest)* |
| [uniqueref.ris](/data/bib/uniqueref.ris)	                 | Unique records after de-duplication |
| [wos1.bib](/data/bib/wos1.bib)	                             | Bibliographic records (1-500) obtained from Web of Science Core Collection using the search string: *(mycorrhiza\* OR ectomycorrhiza\* OR "saprotrophic fungi" OR plant-fung\*) AND (litter OR "litter decay" OR (litter AND decompos\*) OR decomposition OR "nutrient acquisition") AND (forest)* |
| [wos2.bib](/data/bib/wos2.bib)	                             | Bibliographic records (501-1,000) obtained from Web of Science Core Collection using the search string: *(mycorrhiza\* OR ectomycorrhiza\* OR "saprotrophic fungi" OR plant-fung\*) AND (litter OR "litter decay" OR (litter AND decompos\*) OR decomposition OR "nutrient acquisition") AND (forest)* |
| [wos3.bib](/data/bib/wos3.bib)	                             | Bibliographic records (1,001-1,293) obtained from Web of Science Core Collection using the search string: *(mycorrhiza\* OR ectomycorrhiza\* OR "saprotrophic fungi" OR plant-fung\*) AND (litter OR "litter decay" OR (litter AND decompos\*) OR decomposition OR "nutrient acquisition") AND (forest)* |
| [Fig1.svg](/data/Fig1.svg)                                     | Schematic flow diagram for literature search, screening and inclusion process |
| [mass_remaining.csv](/data/mass_remaining.csv)                 | Extracted raw mass remaining data from eligible studies (See codebook for details) |
| [phylo.tre](/data/phylo.tre)                                   | Phylogenetic tree for plant species included in eligible studies |
| [raw_entry1991.csv](/data/raw_entry1991.csv)                   | Extracted raw data for litter decomposition rates from Entry et al 1991 | 
| [species_classification.csv](/data/species_classification.csv) | Taxonomic classification of plant species included |
| [study_metadata.csv](/data/study_metadata.csv)                 | Study characteristics such as number of experiments, duration of experiment, mycorrhizal type, forest type, etc. |
| [meta-analysis.Rmd](/meta-analysis.Rmd)	                       | Reproducible manuscript written with `RMarkdown` which includes all the `R` codes used and initial draft of manuscript |
| [refs.bib](/refs.bib)                                          | Bibliographic entries for literature cited in the manuscript |

## Codebook for [mass_remaining.csv](/data/mass_remaining.csv)

| Column  | Description | Units  |
|---------|-------------|--------|
| id      | ID assigned to each observation in the dataset | NA |
| author  | Authors of the study (in *in-text* citation style) | NA |
| year    | Year in which the study was published | NA |
| species | Botanical name of the plant species to which the litter belongs | NA |
| time    | Time interval at which litter weight was estimated | years |
| mean_ab | Mean value of litter weight in control (absence of mycorrhizal fungi) | %<sup>**a**</sup> |
| se_ab1  | Upper bound of standard error (mean + SE) associated with litter weight in control (absence of mycorrhizal fungi) | % |
| se_ab2  | Lower bound of standard error (mean - SE) associated with litter weight in control (absence of mycorrhizal fungi) | % |
| mean_pr | Mean value of litter weight in experimental (presence of mycorrhizal fungi) | % |
| se_pr1  | Upper bound of standard error (mean + SE) associated with litter weight in experimental (presence of mycorrhizal fungi) | % |
| se_pr2  | Lower bound of standard error (mean - SE) associated with litter weight in experimental (presence of mycorrhizal fungi) | % |

<sup>**a**</sup> % of initial litter weight

## Codebook for [raw_entry1991.csv](/data/raw_entry1991.csv)

| Column  | Description | Units  |
|---------|-------------|--------|
| id      | ID assigned to each observation in the dataset | NA |
| author  | Authors of the study (in *in-text* citation style) | NA |
| year    | Year in which the study was published | NA |
| species | Botanical name of the plant species to which the litter belongs | NA |
| n       | Total number of replicates used | NA |
| w0_g    | Inital weight of litter in grams | grams |
| t_yr    | Time duration of experiment | years |
| k_pr    | Litter decay constant in experimental (presence of mycorrhizal fungi) | year<sup>-1</sup> |
| sd_pr   | Standard deviation associated with litter decay constant in experimental (presence of mycorrhizal fungi) | year<sup>-1</sup> |
| k_ab    | Litter decay constant in control (absence of mycorrhizal fungi) | year<sup>-1</sup> |
| sd_ab   | Standard deviation associated with litter decay constant in control (absence of mycorrhizal fungi) | year<sup>-1</sup> |

