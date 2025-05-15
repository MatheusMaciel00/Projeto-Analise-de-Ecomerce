# Projeto-Analise-de-Ecomerce
# Análise de Dados de Comércio Eletrônico - Projeto de Portfólio

## Sobre o Projeto

Este projeto consiste na análise exploratória e segmentação de clientes de um dataset real de comércio eletrônico, contendo transações entre 2010 e 2011 de uma loja online sediada no Reino Unido. O objetivo principal é extrair insights relevantes sobre o comportamento dos clientes e produtos, identificar padrões de vendas e segmentar os clientes com base em métricas de valor.

---

## Sobre o Dataset

- **Fonte:** Repositório UCI Machine Learning - Dataset "Online Retail"
- **Período:** 01/12/2010 a 09/12/2011
- **Descrição:** Transações reais de uma loja online que vende principalmente presentes exclusivos para várias ocasiões.
- **Tamanho:** Aproximadamente 400 mil registros e 9 colunas, incluindo informações como número da fatura, código do produto, descrição, quantidade, data da transação, preço unitário, ID do cliente e país.

---

## Objetivos da Análise

- Limpeza e pré-processamento dos dados para garantir a qualidade.
- Análise exploratória para identificar os produtos mais vendidos, receita por país e padrões de devolução.
- Cálculo da receita total da empresa.
- Segmentação de clientes utilizando a metodologia RFM (Recency, Frequency, Monetary).
- Aplicação de clusterização (K-Means) para identificar grupos de clientes com comportamento semelhante.
- Visualização dos principais insights para facilitar a compreensão.

---

## Metodologia

### 1. Pré-processamento

- Tratamento de valores ausentes e duplicados.
- Conversão dos dados de data para formato datetime.
- Cálculo da coluna `TotalPrice` (Quantidade x Preço Unitário).
- Identificação e exclusão de devoluções (quantidades negativas).

### 2. Análise Exploratória

- Receita total calculada: **£8,911,407.90**
- Top 10 produtos por quantidade vendida e por receita.
- Receita por país, destacando o Reino Unido como maior consumidor.
- Análise do número e volume de devoluções para identificar possíveis problemas com produtos.

### 3. Segmentação RFM

- Cálculo dos valores Recency (dias desde última compra), Frequency (número de compras) e Monetary (total gasto) para cada cliente.
- Aplicação do algoritmo K-Means para clusterizar os clientes em grupos baseados em RFM.
- Análise dos clusters para entender perfis de clientes, como clientes frequentes e valiosos, clientes ocasionais, e clientes inativos.

---

## Resultados e Insights

- Clientes do Reino Unido representam a maior parte da receita, mas há mercado em outros países como Holanda, Irlanda e Alemanha.
- Alguns produtos, como "PAPER CRAFT , LITTLE BIRDIE" e "WHITE HANGING HEART T-LIGHT HOLDER", são os que mais contribuem para as vendas.
- Existem cerca de 10.624 devoluções, muitas ligadas a produtos danificados ou insatisfatórios.
- A segmentação identificou 4 grupos principais de clientes, desde os muito valiosos (alta frequência e gasto) até os inativos.
- Insights estratégicos para focar campanhas de marketing e retenção em grupos de clientes com maior potencial.

---

## Tecnologias e Bibliotecas Utilizadas

- Python
- Pandas, NumPy (manipulação de dados)
- Matplotlib, Seaborn (visualização)
- Scikit-learn (clusterização K-Means)
- Jupyter Notebook (documentação e experimentação)

---

## Como Executar

1. Clone este repositório.
2. Instale as dependências listadas em `requirements.txt`:
