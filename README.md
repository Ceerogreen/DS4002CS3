# DS4002-Project-2
## Contents
This repository contains all files and documentation for our analysis of how U.S. university admissions criteria have shifted from 2014–2023, particularly in response to the COVID-19 pandemic. It includes data preprocessing scripts, merged IPEDS Admissions (ADM) and Institutional Characteristics (HD) datasets, exploratory data analysis visuals, and logistic regression modeling notebooks used to quantify post-pandemic changes in admissions priorities. Supporting materials such as data dictionaries, references, and visual outputs are organized in dedicated folders for clarity and reproducibility.

## Software and Platform
This project was developed in Python 3 using a combination of Google Colab and Visual Studio Code for data analysis and model development. Core libraries include pandas and numpy for data cleaning and manipulation, matplotlib and seaborn for visualization, and statsmodels and scikit-learn for logistic regression modeling and evaluation. Both environments ensured reproducibility and flexibility, with Colab supporting collaborative work and VS Code used for local testing and refinement. Overleaf, an online LaTeX editor, was used for the creation of DS4002_Project_2_Logit_Outputs.pdf. Local coding and production was done on and supports both Windows and Mac.

## Documentation Map
```text
DS4002-Project-2/
│
├── Data/
│   ├── Dictionaries/                   # IPEDS codebooks & variable description files
|   |   ├── HD2024_dict.xlsx            # Dictionary for each HD/hd file
|   |   ├── adm2021.xlsx                # Dictionary for each adm file from 2021 and earlier
|   |   ├── adm2022.xlsx                # Dictionary for the adm file from 2022
|   |   ├── adm2023.xlsx                # Dictionary for the adm file from 2023
│   ├── HD2023.csv                      # Institutional characteristics dataset for 2023
│   ├── Metadata.md                     # Download links and instructions for raw data
│   ├── adm[2014-2023].csv              # Yearly raw admissions CSVs (IPEDS ADM files)
│   ├── adm[2014-2022]_rv.csv           # Yearly revised admissions CSVs (IPEDS ADM files)
│   ├── combined_admissions_characteristics.csv # Processed and merged dataset ready for analysis
│   └── hd[2014-2022].csv               # Institutional characteristics datasets (IPEDS HD files)

│
├── Scripts/
│   ├── 00_Run.ipynb                # Master notebook that executes the full pipeline
│   ├── 01_data_cleaning.ipynb      # Data import, cleaning & harmonization
│   ├── 02_eda.ipynb                # Join ADM and HD datasets via UNITID+year
│   └── 03_regression.ipynb         # Logistic regression modeling of admissions criteria
│
├── Output/
│   ├── DS4002_Project_2_Logit_Outputs.pdf   # PDF of Logit Outputs
│   ├── DS4002_Project_2_Logit_Outputs.tex   # LaTeX file to reproduce PDF
│   ├── actual_vs_predicted_admcon7.png      # Visualizations of logit models for SAT/ACT sore usage
│   ├── admcon_trends_subplot.png   # Visualization of admissions criteria trends
│   ├── controlVsTestScores.png     # Visualization of test score usage by University type
|   ├── logit_summary_[ADMCON].tex  # Tabular output for each logit regression in LaTeX format
│   └── satpct_trends_control.png   # SAT/ACT requirement trends by institution control
│
├── LICENSE.txt                     # MIT License
│
└── README.md                       # This ReadMe

```

## Instructions for Reproducibility 
1. Clone the Repository: Create a local copy of the repository, or access it through the GitHub extension in VS Code
2. Run the 00_Run file: Run the 00_Run script in the Scripts folder. This will run all other scripts in the folder, and should take around 30 seconds.
3. Compile the Tex files: Using a Tex editor such as Overleaf, use the DS4002_Project_2_Logit_Outputs.Tex file (with the other Tex files as inputs) to produce DS4002_Project_2_Logit_Outputs.pdf, an easy visual file of the Logit regression output tables. 
