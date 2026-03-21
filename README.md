# PET – Anonymization of Datasets with Privacy, Utility and Risk Analysis

Projeto da UC **Tecnologias de Reforço da Privacidade (PET)**.

## 1. Objetivo do projeto

Este projeto tem como objetivo estudar o processo de anonimização de um dataset real, avaliando o equilíbrio entre:

- **privacidade**
- **utilidade**
- **risco de reidentificação**

O trabalho segue o enunciado da unidade curricular e inclui:

1. seleção, sanitização e caracterização do dataset;
2. definição de coding models e hierarquias de generalização;
3. aplicação e comparação de pelo menos dois modelos de privacidade;
4. análise de utilidade, privacidade e risco;
5. elaboração de relatório final.

## 2. Dataset escolhido

Foi escolhido o dataset **Adult / Census Income**, extraído da base de dados do Census Bureau de 1994.

### Descrição resumida
O dataset contém informação demográfica, educacional e profissional de indivíduos, com o objetivo preditivo de determinar se uma pessoa aufere rendimento anual **superior a 50K USD**.

### Motivação para a escolha
Este dataset foi escolhido porque:

- possui número suficiente de registos e atributos;
- contém atributos categóricos e numéricos;
- inclui vários potenciais **quasi-identifiers**;
- permite experimentar diferentes estratégias de anonimização;
- facilita a avaliação de utilidade através de análises estatísticas comparativas.

## 3. Objetivo de libertação do dataset anonimizado

Pretende-se libertar uma versão anonimizada do dataset que permita estudar a relação entre características sociodemográficas/laborais e a variável de rendimento (`income`), sem possibilitar a reidentificação de indivíduos.

### Perguntas analíticas alvo
O dataset anonimizado deverá preservar, tanto quanto possível, a capacidade de responder a perguntas como:

- Qual a proporção de indivíduos com rendimento superior a 50K?
- Como varia essa proporção com o nível de educação?
- Como varia essa proporção com o género?
- Como varia essa proporção com grupos etários?

## 4. Estrutura do repositório (IDEIA INICIAL)

```text
.
├── README.md
├── docs/
├── data/
│   ├── raw/
│   ├── processed/
│   └── anonymized/
├── arx/
│   ├── projects/
│   ├── hierarchies/
│   └── exports/
├── analysis/
│   ├── notebooks/
│   ├── scripts/
│   └── results/
└── presentation/
