# DS4002-Project-2
## Contents
This repository contains all files and documentation for our analysis of how U.S. university admissions criteria have shifted from 2014–2023, particularly in response to the COVID-19 pandemic. It includes data preprocessing scripts, merged IPEDS Admissions (ADM) and Institutional Characteristics (HD) datasets, exploratory data analysis visuals, and logistic regression modeling notebooks used to quantify post-pandemic changes in admissions priorities. Supporting materials such as data dictionaries, references, and visual outputs are organized in dedicated folders for clarity and reproducibility.

## Software and Platform
This project was developed in Python 3 using a combination of Google Colab and Visual Studio Code for data analysis and model development. Core libraries include pandas and numpy for data cleaning and manipulation, matplotlib and seaborn for visualization, and statsmodels and scikit-learn for logistic regression modeling and evaluation. Both environments ensured reproducibility and flexibility, with Colab supporting collaborative work and VS Code used for local testing and refinement.

## Documentation Map
```text
DS4002-Project-2/
│
├── Data/
│   │
│   ├── Dictionaries/
│   │   ├── HD2024_dict.xlsx
│   │   ├── adm2021.xlsx
│   │   ├── adm2022.xlsx
│   │   ├── adm2023.xlsx
│   │   └── ~$adm2023.xlsx
│   │
│   ├── HD2023.csv
│   ├── adm2014.csv
│   ├── adm2014_rv.csv
│   ├── adm2015.csv
│   ├── adm2015_rv.csv
│   ├── adm2016.csv
│   ├── adm2016_rv.csv
│   ├── adm2017.csv
│   ├── adm2017_rv.csv
│   ├── adm2018.csv
│   ├── adm2018_rv.csv
│   ├── adm2019.csv
│   ├── adm2019_rv.csv
│   ├── adm2020.csv
│   ├── adm2020_rv.csv
│   ├── adm2021.csv
│   ├── adm2021_rv.csv
│   ├── adm2022.csv
│   ├── adm2022_rv.csv
│   ├── adm2023.csv
│   ├── combined_admissions_characteristics.csv
│   ├── hd2014.csv
│   ├── hd2015.csv
│   ├── hd2016.csv
│   ├── hd2017.csv
│   ├── hd2018.csv
│   ├── hd2019.csv
│   ├── hd2020.csv
│   ├── hd2021.csv
│   └── hd2022.csv
│
├── Output/
│
├── Scripts/
│
├── LICENSE.txt
└── README.md
```

## Instructions for Reproducibility 
1. 
