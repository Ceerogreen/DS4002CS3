# Data Set Establishment Details

## Summary
Our dataset is composed of institutional-level CSV files from the U.S. Department of Education’s Integrated Postsecondary Education Data System (IPEDS), spanning the years 2014–2023. We use data from two survey components: Admissions (ADM) and Institutional Characteristics (HD). The ADM files provide annual information on undergraduate admissions policies and outcomes—such as test score requirements, GPA consideration, and application counts—while the HD files contain institutional descriptors including control (public/private), size, region, and degree level. Together, these datasets allow us to examine year-over-year trends in college admissions practices, particularly before and after the onset of the COVID-19 pandemic.

## Provenance
All data were downloaded directly from the National Center for Education Statistics (NCES) via the IPEDS Data Center (https://nces.ed.gov/ipeds/datacenter/). The data are institution-reported and federally maintained, ensuring comprehensive coverage and standardized variable definitions across years. We retrieved the Admissions (ADM2014–ADM2023) and Institutional Characteristics (HD2014–HD2023) CSV files along with their official codebooks. These files have not been altered, and all cleaning steps were performed solely for analysis reproducibility and consistency across years.

## License
IPEDS data are public domain materials under U.S. Government Work status. They are freely available for non-commercial, educational, and research purposes without restriction. No proprietary or confidential data were accessed or used. All project usage complies fully with NCES data access and citation requirements.

---

## Data Dictionary

[A partial data dictionary can be found at this link](https://myuva-my.sharepoint.com/:w:/g/personal/htn9hj_virginia_edu/EUfPWumAh45Mn94s3wUH02YBZE7mZRWQt09m84uChxkYfg?e=acPSpy)

Files containing full descriptions and dictionaries of data are located in [/Data/Dictionaries](https://github.com/Raj6881/DS4002-Project-2/tree/main/Data/Dictionaries)


---

## Ethical Statement
This project exclusively uses aggregate, publicly available institutional data with no personally identifiable information. All analyses are conducted for academic purposes in compliance with NCES policies and University of Virginia research ethics standards. The team maintains transparency in all data processing and modeling steps and accurately reports findings and limitations. No attempt is made to infer or disclose any information about individual students or institutions beyond what is publicly reported.

---

## Question We Explored
How have U.S. university admissions criteria changed from 2014 to 2023?

We investigated how the importance and prevalence of different admissions factors—such as standardized test scores, GPA, essays, and recommendations—have evolved over the past decade. Our analysis focused on identifying trends across all institutions and assessing whether the COVID-19 pandemic accelerated a shift toward holistic admissions policies.
- The most significantly changing admissions variable from 2014–2023 was whether standardized test scores (SAT/ACT) were required.
- Standardized testing requirements dropped sharply after 2020, reflecting widespread adoption of test-optional policies.
- Institutional control type (public vs. private) showed significant differences in standardized test requirements, with private institutions generally moving toward test-optional policies more rapidly than public ones.

---

## Exploratory Data Plots
[Figure 1: Trends in Admission Considerations Over Time](https://github.com/Raj6881/DS4002-Project-2/blob/main/Output/admcon_trends_subplot.png)

[Figure 2: Effect of Control Type of University on Test Score Criteria](https://github.com/Raj6881/DS4002-Project-2/blob/main/Output/controlVsTestScores.png)

---

## Unknown Question
**Can shifts in U.S. university admissions criteria be predicted using institutional characteristics and historical data?**

We will explore whether a predictive model can accurately anticipate changes in admissions requirements—particularly standardized testing policies—based on institutional control type and temporal trends.
