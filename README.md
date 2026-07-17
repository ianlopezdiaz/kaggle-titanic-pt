# Titanic: Estudo de Caso Completo de Classificação

> **Idioma:** 🇧🇷 Português | 🇺🇸 [English](https://github.com/ianlopezdiaz/kaggle-titanic)

Este repositório apresenta um fluxo de trabalho completo de aprendizado de máquina utilizando o conjunto de dados **Kaggle Titanic: Machine Learning from Disaster**.

O projeto foi desenvolvido tanto como uma peça de portfólio quanto como um recurso educacional, demonstrando as etapas típicas de um projeto supervisionado de classificação - desde a análise exploratória dos dados até a engenharia de atributos, desenvolvimento de modelos, avaliação e geração de uma submissão para a competição do Kaggle.

O site desenvolvido com Quarto documenta todas as etapas do fluxo de trabalho e está disponível em:

**[https://ianlopezdiaz.github.io/kaggle-titanic-pt](https://ianlopezdiaz.github.io/kaggle-titanic-pt)**


---

## Visão Geral do Projeto

O objetivo é prever se um passageiro sobreviveu ao naufrágio do RMS Titanic utilizando informações demográficas, socioeconômicas e relacionadas à viagem.

Em vez de focar exclusivamente no desempenho na competição, este projeto enfatiza boas práticas de aprendizado de máquina, fluxos de trabalho reprodutíveis e uma engenharia de atributos cuidadosa.

O pipeline completo inclui:

* Análise Exploratória de Dados (EDA)
* Limpeza e pré-processamento dos dados
* Engenharia de atributos
* Transformações de atributos
* Codificação de atributos
* Treinamento de modelos
* Avaliação de modelos
* Geração da submissão para o Kaggle

---

## Conjunto de Dados

O projeto utiliza o conjunto de dados da competição **Titanic: Machine Learning from Disaster**, disponível no Kaggle.

* Visão geral da competição: [https://www.kaggle.com/competitions/titanic](https://www.kaggle.com/competitions/titanic)
* Conjunto de dados: [https://www.kaggle.com/competitions/titanic/data](https://www.kaggle.com/competitions/titanic/data)

---

## Estrutura do Repositório

```text
kaggle-titanic-pt/
│
├── README.md                                   # Visão geral do projeto e instruções de uso.
├── index.qmd                                   # Página inicial do site em Quarto.
├── _quarto.yml                                 # Configuração do site em Quarto.
├── environment.yml                             # Especificação do ambiente Conda.
├── LICENSE                                     # Licença do projeto.
│
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb      # Análise exploratória do conjunto de dados Titanic.
│   ├── 02_feature_engineering.ipynb            # Engenharia de atributos, transformações e codificação.
│   └── 03_modeling_and_evaluation.ipynb        # Treinamento, avaliação dos modelos e geração da submissão ao Kaggle.
│
├── data/
│   ├── raw/
│   │   ├── train.csv                           # Conjunto de treinamento do Kaggle.
│   │   ├── test.csv                            # Conjunto de teste do Kaggle.
│   │   └── gender_submission.csv               # Exemplo de arquivo de submissão do Kaggle.
│   │
│   └── processed/
│       ├── 01_data.parquet                     # Conjunto de dados produzido após a análise exploratória.
│       ├── 01_features.parquet                 # Registro de atributos após a análise exploratória.
│       ├── 02_data.parquet                     # Conjunto de dados após a engenharia de atributos.
│       ├── 02_features.parquet                 # Registro de atributos atualizado após a engenharia de atributos.
│       └── submission.csv                      # Predições finais submetidas ao Kaggle.
│
└── _site/
    └── ...                                     # Site gerado pelo Quarto.
```


---

## Executando o Projeto

### Instale as dependências

Crie o ambiente Conda:

```bash
conda env create -f environment.yml
```

Se desejar, você pode alterar o nome do ambiente no arquivo `environment.yml` antes de criá-lo.

---

## Construindo a Documentação

Este repositório utiliza **Quarto** para gerar o site do projeto.

Visualize o site localmente:

```bash
quarto preview
```

Renderize o site completo:

```bash
quarto render
```

Publique no GitHub Pages:

```bash
quarto publish gh-pages
```

---

## Licença

Este projeto é distribuído sob os termos da Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
