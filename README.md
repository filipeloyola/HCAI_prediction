# Healthcare-associated infection (HCAI) prediction

This repository contains files relating to the article "Prediction of healthcare-associated infection in hospitalized patients with COVID-19" submitted to American Journal of Infection Control. In this repository you can find a folder called Datasets, containing the row data files used in the research, as explained in the item *Datasets*. You can also find the files used in the datasets construction as explained in the item *DatasetsConstruction*. In the main directory of this repository there are the following files:

- "mainNotebook.ipynb": this is the main notebook with descriptive statistical analysis, data discretization, preprocessing, training and testing of machine learning models and SHAP analysis.

- "exames_COVID19_considerados.xlsx" and "exames_infeccoes.xlsx": These are manually constructed spreadsheets that contain the list of tests considered for the COVID 19 and hospital infection diagnosis, respectively.

- "negative_patients.xlsx" and "positive_patients": these files were generated in "DatasetsConstruction" and refer to patients labels, as negative and positive respectively. These two spreadsheets are used by "mainNotebook.ipynb".

- "agrupado.xlsx": this is a spreadsheet containing the reference values for each exam. These values were taken from the original data and it be used to date discretization in the "mainNotebook.ipynb".

- "describe.xlsx": This is a spreadsheet containing a statistical description of the variables selected in the "mainNotebook.ipynb".


## Datasets
Os datasets estão disponíveis em três arquivos ".csv", contendo dados dos exames, desfechos e pacientes. Esses dados foram baixados do repositório aberto COVID-19 Datasharing FAPESP (https://repositoriodatasharingfapesp.uspdigital.usp.br/) 

Pasta de arquivos, com dados anonimizados de pacientes que fizeram teste para COVID-19 a partir de 1/11/2019, compactada em formato .zip. Contem 3 arquivos em formato .csv e um arquivo em formato .xlsx: (1) Planilha com dados anonimizados sobre pacientes que fizeram teste para o COVID-19 (sorologia ou PCR), incluindo: identificador anonimizado do paciente, genero, pais, estado, municipio e regiao de residencia; (2) Respectivos resultados de exames laboratoriais, incluindo dentre outros o identificador anonimizado do paciente e um identificador de atendimento; (3) Desfechos - cada registro inclui dentre outros o identificador anonimizado do paciente e um identificador de atendimento; descreve um atendimento de um paciente, e o desfecho correspondente, quando aplicavel; e (4) Dicionario de dados: planilha em que cada aba descreve respectivamente todos os campos das planilhas de Pacientes, Exames e Desfechos. As planilhas Pacientes, Exames e Desfechos sao interligaveis pelo identificador anonimizado do paciente. As planilhas Exames e Desfechos sao interligaveis pelo par (identificador do paciente, identificador do atendimento). Devido ao grande numero de registros, nem sempre as planilhas poderao ser importadas diretamente para EXCEL ou semelhantes.

## Datasets construction




## Citation
Para citar a metodologia proposta, utilize as informações abaixo:
Em construção.

## Acknowledgements
This research was supported in part by the Coordenação de Aperfeiçoamento de Pessoalde Nível Superior - Brasil (CAPES) - Finance Code 001. The authors gratefully acknowledge the Brazilian funding agencies FAPESP (Fundação Amparo à Pesquisa do Estado de São Paulo) pela disponibilização do repositório COVID-19 Datasharing

