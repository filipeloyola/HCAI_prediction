# Healthcare-associated infection (HCAI) prediction
This repository contains files about the article "Healthcare-associated infection prediction on hospitalized COVID-19 patients" submitted to the Brazilian Congress on Biomedical Engineering. In this repository, you can find a DatasetsConstruction folder containing the files used in the datasets construction. In the leading directory of this repository, there is the "ML_notebook," which provides training and testing of machine learning models and SHAP analysis.


## RawDatasets
The raw data is available in three ".csv" files, containing data from patients who were tested for COVID-19 from 2020-02-26 to 2020-12-29: 

- (1) "HSL_Pacientes_3.csv": Spreadsheet with anonymized data about patients;
- (2) "HSL_Exames_3.csv": Respective laboratory test results, including the anonymized patient identifier and a service identifier; 
- (3) "HSL_Desfechos_3.csv": Outcomes - each record includes describes a patient's care, and the corresponding outcome, when applicable. 

This data was downloaded from the COVID-19 Data Sharing FAPESP open repository (https://repositoriodatasharingfapesp.uspdigital.usp.br/).

## DatasetsConstruction
In the "DatasetConstruction" directory, you can check the notebooks used to connect the raw datasheets. These notebooks are:

- "Covid_exploratory_analysis.ipynb": In this file, all patients diagnosed with COVID-19 via PCR are identified and a first patient filter is performed. At the end of the code, the following spreadsheet is generated: "lista_covid_positivito.xlsx";

- "Patients_selection.ipynb": This file checks positive and non-positive patients for hospital infections. At the end of the code, the following spreadsheets are generated: "pacientes_positivos.xlsx" and "pacientes_negativos.xlsx";

- "Datasets_construction.ipynb": In this dataset, we select the desired variables for the research datasets. First, we discarded variables with more than 50% null values. Next, we perform manual attribute selection. We did a manual selection with a doctor specialized in the field. In manual selection, we discard variables that are correlated with each other. In the end, two datasets were generated: "original_dataset.xlsx" and "discreted_dataset.xlsx".


The "DatasetsConstruction" directory also has the following files:

- "exames_COVID19_considerados.xlsx" and "exames_infeccoes.xlsx": These are manually constructed spreadsheets that contain the list of tests considered for the COVID-19 and hospital infection diagnosis, respectively;

- "negative_patients.xlsx" and "positive_patients.xlsx": these files were generated in "Patients_selection.ipynb" and refer to patients' labels as negative and positive, respectively;

- "agrupado.xlsx" is a spreadsheet containing the reference values for each exam. These values were taken from the original data, and it is used to date discretization in the "Datasets_construction.ipynb";

- "describe.xlsx": This spreadsheet contains a statistical description of the variables selected in the "Datasets_construction.ipynb";

- "describe_2.xlsx": It is the summarized spreadsheet of "describe.xlsx".

## Citation
In construction. 

## Acknowledgements
This research was supported in part by the Coordenação de Aperfeiçoamento de Pessoalde Nível Superior - Brasil (CAPES) - Finance Code 001. The authors gratefully acknowledge the Brazilian funding agency FAPESP (Fundação Amparo à Pesquisa do Estado de São Paulo) for the COVID-19 Data Sharing repository.
