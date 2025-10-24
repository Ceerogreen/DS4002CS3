# DS4002-Project-2
## Contents
This repository contains all files and documentation for our analysis of how U.S. university admissions criteria have shifted from 2014–2023, particularly in response to the COVID-19 pandemic. It includes data preprocessing scripts, merged IPEDS Admissions (ADM) and Institutional Characteristics (HD) datasets, exploratory data analysis visuals, and logistic regression modeling notebooks used to quantify post-pandemic changes in admissions priorities. Supporting materials such as data dictionaries, references, and visual outputs are organized in dedicated folders for clarity and reproducibility.

## Software and Platform
This project was developed in Python 3 using a combination of Google Colab and Visual Studio Code for data analysis and model development. Core libraries include pandas and numpy for data cleaning and manipulation, matplotlib and seaborn for visualization, and statsmodels and scikit-learn for logistic regression modeling and evaluation. Both environments ensured reproducibility and flexibility, with Colab supporting collaborative work and VS Code used for local testing and refinement. Overleaf, an online LaTeX editor, was used for the creation of DS4002_Project_2_Logit_Outputs.pdf.

## Documentation Map
```text
DS4002-Project-2/
│
├── Data/
│   ├── ADM2014-2023/               # Yearly raw admissions CSVs (IPEDS ADM files)
│   ├── HD2014-2023/                # Institutional characteristics datasets (IPEDS HD files)
│   ├── Dictionaries/               # IPEDS codebooks & variable description files
│   ├── Cleaned/                    # Processed and merged datasets ready for analysis
│   └── Data Instructions.txt       # Download links and instructions for raw data
│
├── Notebooks/
│   ├── 00_Run.ipynb                # Master notebook that executes the full pipeline
│   ├── 01_Data_Cleaning.ipynb      # Data import, cleaning & harmonization
│   ├── 02_Merging.ipynb            # Join ADM and HD datasets via UNITID+year
│   ├── 03_Logit_Model.ipynb        # Logistic regression modeling of admissions criteria
│   └── 04_Visualizations.ipynb     # Trend, coefficient, and summary visualizations
│
├── Results/
│   ├── admcon_trends_subplot.png   # Visualization of admissions criteria trends
│   ├── satpct_trends_control.png   # SAT/ACT requirement trends by institution control
│   ├── coefficients_summary.csv    # Output of logit regression models (coefficients, p-values)
│   └── cleaned_admissions.csv      # Final cleaned/merged dataset used for modeling
│
├── Docs/
│   ├── AnalysisPlan.pdf            # Project plan, hypothesis, methodology document
│   ├── References.txt              # List of sources and citations used in project
│   └── README.md                   # This file (repository overview)
│
└── requirements.txt                 # Python packages required to reproduce the analysis

```

## Instructions for Reproducibility 
1. Clone the Repository: Create a local copy of the repository, or access it through the GitHub extension in VS Code
2. Run the 00_Run file: Run the 00_Run script in the Scripts folder. This will run all other scripts in the folder, and should take around 30 seconds.
3. Compile the Tex files: Using a Tex editor such as Overleaf, use the DS4002_Project_2_Logit_Outputs.Tex file (with the other Tex files as inputs) to produce DS4002_Project_2_Logit_Outputs.pdf, an easy visual file of the Logit regression output tables. 
