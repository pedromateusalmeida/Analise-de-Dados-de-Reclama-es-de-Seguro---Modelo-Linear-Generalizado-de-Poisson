 Análise de Dados de Reclamações de Seguro - Modelo Linear Generalizado de Poisson

## Organização
**Seguradora XYZ**

## Descrição do Projeto
Este repositório contém um projeto de análise de dados e modelagem preditiva com o objetivo de ajustar um modelo linear generalizado de Poisson para prever o número de reclamações de seguro automotivo. Utilizamos dados do arquivo `motorins.dat` que contém informações sobre quilometragem, zona geográfica, bônus, tipo de automóvel, número de veículos segurados e o número de reclamações.

## Base de Dados
O arquivo **motorins.dat** contém as seguintes variáveis:
- **Kilometers**: Quilômetros percorridos em um ano.
  - 1: menos de 1000
  - 2: de 1000 a 15 000
  - 3: 15 000 a 20 000
  - 4: 20 000 a 25 000
  - 5: mais de 25 000
- **Zone**: Região Geográfica (Zona).
  - 1: Estocolmo, Gotemburgo, Malmö e arredores
  - 2: Outras grandes cidades e arredores
  - 3: Cidades menores e arredores no sul da Suécia
  - 4: Áreas rurais no sul da Suécia
  - 5: Cidades menores e arredores no norte da Suécia
  - 6: Áreas rurais no norte da Suécia
  - 7: Gotland
- **Bonus**: Igual ao número de anos sem reclamações mais 1.
- **Make**: Representa 8 tipos de modelos de automóveis mais o tipo 9 (outros).
- **Insured**: Número de veículos segurados.
- **Claims**: Número de reclamações.

## Objetivo do Projeto
O principal objetivo deste projeto é desenvolver um modelo linear generalizado de Poisson para estimar o número de reclamações de seguro automotivo com base nas variáveis preditoras fornecidas no dataset.

## Roteiro da Atividade

Roteiro da análise:

1. **Carregando Bibliotecas**
2. **Informações Básicas do Dataset**
    - Print das 5 primeiras linhas
    - Tipo de dado em cada coluna
    - Descrição das colunas numéricas (contagem, média, mediana, desvio padrão)
3. **Análise Exploratória**
    - Dados missing
    - Distribuição da variável `Claims`
    - Scatter plot das variáveis numéricas com `Claims`
4. **Modelagem**
    - Correlação de Spearman
    - Teste de Shapiro-Wilk
    - Teste de Kruskal-Wallis
    - Teste Mann-Whitney U
    - Teste de qui-quadrado
5. **Treinamento do Modelo**
6. **Análise dos Resíduos**
7. **Conclusão**
