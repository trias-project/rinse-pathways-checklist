# RINSE - registry of pathways and vectors of biological invasions in Northwest Europe


## Rationale

This repository contains the functionality to standardize the data of [Zieritz et al. (2017)](https://link.springer.com/article/10.1007/s10530-016-1278-z) (Supplementary Table 2) to a [Darwin Core checklist](https://www.gbif.org/dataset-classes) that can be harvested by [GBIF](http://www.gbif.org). The repository also contains the code for a [website](http://trias-project.github.io/rinse-pathways-checklist/map.html) to explore the checklist data. It was developed for the [TrIAS project](http://trias-project.be).

## Workflow

[source data](https://github.com/trias-project/rinse-pathways-checklist/blob/master/data/raw/copy_of_10530_2016_1278_MOESM2_ESM.xlsx) (transcribed from original) → Darwin Core [mapping script](http://trias-project.github.io/rinse-pathways-checklist/dwc_checklist.html) → generated [Darwin Core files](https://github.com/trias-project/rinse-pathways-checklist/blob/master/data/processed)

## Published datasets

* Checklist dataset on the IPT
* Checklist dataset on GBIF

## Repo structure

The repository structure is based on [Cookiecutter Data Science](http://drivendata.github.io/cookiecutter-data-science/). Files and directories indicated with `GENERATED` should not be edited manually.

```
├── README.md         : Description of this repository
├── LICENSE           : Repository license
├── .gitignore        : Files and directories to be ignored by git
│
├── data
│   ├── raw           : Source data, input for mapping script
│   └── processed     : Darwin Core output of mapping script GENERATED
│
├── docs              : Repository website GENERATED
│
├── specifications    : Data specifications for the Darwin Core files
│
└── src
    ├── dwc_checklist.Rmd  : Darwin Core mapping script for checklist dataset
    └── src.Rproj          : RStudio project file
```

## Installation

1. Clone this repository to your computer
2. Open the RStudio project file
3. Open the `dwc_checklist.Rmd` [R Markdown file](https://rmarkdown.rstudio.com/) in RStudio
4. Install any required packages
5. Click `Run > Run All` to generate the processed data
6. Alternatively, click `Build > Build website` to generate the processed data and build the website in `/docs`

## Contributors

[List of contributors](https://github.com/trias-project/rinse-pathways-checklist/contributors)

## License

[MIT License](https://github.com/trias-project/rinse-pathways-checklist/blob/master/LICENSE)
