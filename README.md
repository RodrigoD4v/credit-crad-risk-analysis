# Credit Card Approval Prediction

## Descrição do Projeto

Este projeto tem como objetivo criar um modelo de classificação utilizando o algoritmo Random Forest para prever a aprovação de cartões de crédito com base em dados pessoais dos candidatos e informações históricas. O modelo auxilia os bancos na tomada de decisão sobre quem deve receber um cartão de crédito, quantificando o risco de inadimplência de maneira objetiva.

## Conjuntos de Dados

O projeto utiliza dois conjuntos de dados principais:

- **application_record.csv**: Contém informações pessoais dos candidatos, como gênero, idade, renda anual, nível de educação, estado civil, entre outros.
- **credit_record.csv**: Registra o histórico de crédito dos clientes, incluindo o status de pagamento ao longo do tempo.

## Pré-processamento e Análise

### Principais Etapas:

1. **Carregamento e Mesclagem dos Dados**: Os conjuntos de dados são carregados e mesclados com base no ID comum.
2. **Tratamento de Valores Ausentes**: Identificação e tratamento de valores nulos para garantir a qualidade dos dados.
3. **Análise Exploratória**: Exploração das características dos dados para entender distribuições, correlações e possíveis outliers.
4. **Transformação de Dados**: Codificação de variáveis categóricas e normalização de variáveis numéricas.
5. **Engenharia de Features**: Criação de novas variáveis para melhorar o desempenho do modelo.

## Modelagem

### Algoritmo Utilizado:
- **Random Forest**: Um algoritmo de ensemble que combina múltiplas árvores de decisão para melhorar a precisão e robustez das previsões.

### Métricas de Avaliação:
- **Acurácia**: Proporção de previsões corretas em relação ao total.
- **Precision**: Proporção de verdadeiros positivos entre todas as previsões positivas.
- **Recall**: Proporção de verdadeiros positivos identificados corretamente.
- **F1-Score**: Média harmônica entre precision e recall.

## Resultados

O modelo foi avaliado utilizando as métricas mencionadas, demonstrando boa performance na previsão de aprovações de cartões de crédito. Os resultados detalhados podem ser encontrados no notebook `credit_card_approval.ipynb`.

## Como Executar o Projeto

### Pré-requisitos:
- **Python 3.11**
- **Bibliotecas Python**: pandas, numpy, scipy, matplotlib, seaborn, scikit-learn

### Instalação:
```bash
pip install pandas numpy scipy matplotlib seaborn scikit-learn
```
### Execução:
1. Baixe os conjuntos de dados `application_record.csv` e `credit_record.csv` e coloque-os na pasta `data`.
2. Execute o notebook Jupyter `credit_card_approval.ipynb` para reproduzir a análise e o modelo.

## Estrutura do Projeto

credit_card_approval/
- data/
  - application_record.csv
  - credit_record.csv
- notebooks/
  - credit_card_approval.ipynb
- README.md


