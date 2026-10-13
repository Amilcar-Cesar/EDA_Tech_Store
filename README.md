# Análise Exploratória de Vendas - Tech Store

Este repositório contém uma Análise Exploratória de Dados (EDA) realizada no Jupyter Notebook [`analise_vendas.ipynb`](analise_vendas.ipynb), utilizando a base de transações da loja (`data/vendas.csv`).

---

## 📊 Base de Dados

O arquivo [`data/vendas.csv`](data/vendas.csv) reúne registros de transações com as seguintes colunas:

- **`data`**: Data em que a venda foi realizada.
- **`produto`**: Nome do item vendido.
- **`categoria`**: Categoria do produto (*Eletrônicos*, *Periféricos*, *Móveis*, *Vestuário*).
- **`quantidade`**: Número de unidades vendidas no pedido.
- **`preco_unitario`**: Preço unitário do produto (em R$).
- **`cliente`**: Nome do cliente.
- **`regiao`**: Região de entrega (*Sudeste*, *Sul*, *Nordeste*, *Norte*, *Centro-Oeste*).

---

## 🔍 O que foi analisado no Notebook

No notebook [`analise_vendas.ipynb`](analise_vendas.ipynb), foram desenvolvidas as seguintes análises principais:

1. **Carregamento e Inspeção Inicial**:
   - Leitura do arquivo CSV usando a biblioteca `pandas`.
   - Visualização das primeiras linhas e verificação dos tipos de dados.

2. **Cálculo de Faturamento / Receita**:
   - Criação da coluna de receita total por item (`quantidade * preco_unitario`).
   - Apuração do volume financeiro total gerado pelas vendas.

3. **Filtragem e Segmentação de Dados**:
   - Aplicação de filtros por categoria de produto (ex.: *Eletrônicos*).
   - Filtros por faixas de preço unitário e por localização geográfica (regiões).

4. **Produtos Mais Vendidos**:
   - Agrupamento (`groupby`) por produto e agregação pela soma de unidades vendidas.
   - Identificação do ranking (Top produtos) com maior volume de saída.

5. **Desempenho por Categoria e Região**:
   - Avaliação da distribuição de vendas e desempenho entre as diferentes categorias e regiões.

---

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Pandas**
- **Jupyter Notebook**

---

## 🚀 Como Executar

1. Abra a pasta do projeto no VS Code ou terminal.
2. Com o ambiente virtual ativado, garanta as dependências instaladas:
   ```bash
   pip install pandas
   ```
3. Abra o arquivo [`analise_vendas.ipynb`](analise_vendas.ipynb) e execute as células em ordem (`Shift + Enter`).
