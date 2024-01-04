# Python para Engenharia de Dados

# Bibtext Extractor

## Como funciona
Este projeto é um extrator de arquivos que pode ser usado para extrair arquivos BibTeX e convertê-los em Json, CSV ou Yaml com base no arquivo config.yaml.

#### Requisitos
- Python 3+
- Pip
- Lib Pandas
- Lib Bibtexparser (https://bibtexparser.readthedocs.io/)
- Lib Yaml

#### config.yaml
type: <output file type, available options: json, csv or yaml>
file_name: <output file name>

#### main.py
Contém o código principal do fluxo
  * 1 - Lê todos os arquivos BibTeX
  * 2 - Organiza as colunas 
  * 3 - Concatena o dataframe do Ieee, ScientDirect e Dl ACM
  * 4 - Lê o arquivo config.yaml
  * 5 - Escreve o arquivo de saída json, csv ou yaml.

#### Pasta File
Contém os arquivos BibTex que foram salvos dos sites ieee, scientdirect e dl acm.
  
#### Usando
```
python main.py
```
