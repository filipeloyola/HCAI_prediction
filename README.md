# Healthcare-associated infection (HCAI) prediction
This repository contains files about the article "Healthcare-associated infection prediction on hospitalized COVID-19 patients" submitted to the Brazilian Congress on Biomedical Engineering. In this repository, you can find a folder called Datasets, containing the row data files used in the research, as explained in the item *Datasets*. You can also find the files used in the dataset construction as explained in the item *DatasetsConstruction*. In the main directory of this repository, there are the following files:

- "mainNotebook.ipynb": this is the main notebook with descriptive statistical analysis, data discretization, preprocessing, training and testing of machine learning models and SHAP analysis.

- "exames_COVID19_considerados.xlsx" and "exames_infeccoes.xlsx": These are manually constructed spreadsheets that contain the list of tests considered for the COVID-19 and hospital infection diagnosis, respectively.

- "negative_patients.xlsx" and "positive_patients": these files were generated in "DatasetsConstruction" and refer to patients' labels as negative and positive, respectively. These two spreadsheets are used by "mainNotebook.ipynb".

- "agrupado.xlsx" is a spreadsheet containing the reference values for each exam. These values were taken from the original data, and it is used to date discretization in the "main notebook.ipynb".

- "describe.xlsx": This spreadsheet contains a statistical description of the variables selected in the "mainNotebook.ipynb".


## Datasets
The row data is available in three ".csv" files, containing data from patients who were tested for COVID-19 from 2020-02-26 to 2020-12-29: 

- (1) "HSL_Pacientes_3.csv": Spreadsheet with anonymized data about patients;
- (2) "HSL_Exames_3.csv": Respective laboratory test results, including the anonymized patient identifier and a service identifier; 
- (3) "HSL_Desfechos_3.csv": Outcomes - each record includes describes a patient's care, and the corresponding outcome, when applicable. 

This data was downloaded from the COVID-19 Data Sharing FAPESP open repository (https://repositoriodatasharingfapesp.uspdigital.usp.br/).

## Dataset construction
In the "DatasetConstruction" directory, you can check the notebook used to connect the row datasheets. Exams and Outcomes spreadsheets are interlinkable by pair (patient identifier, service identifier). In the "Datasets_construction.ipynb", the study was carried out together with the medical professional to select the essential variables for the research and eliminate correlated variables with each other. In this directory, it is also possible to check the list of tests considered for the diagnosis of COVID-19 and hospital infection in the files "exames_COVID19_considerados.xlsx" and "exames_infeccoes.xlsx." Furthermore, the spreadsheets "lista_covid_positivity.xlsx" and "lista_infec_positivity.xlsx" are files only used in the dataset construction process, not the main steps.


## Citation
In construction. 

## Acknowledgements
This research was supported in part by the Coordenação de Aperfeiçoamento de Pessoalde Nível Superior - Brasil (CAPES) - Finance Code 001. The authors gratefully acknowledge the Brazilian funding agency FAPESP (Fundação Amparo à Pesquisa do Estado de São Paulo) for the COVID-19 Data Sharing repository.
