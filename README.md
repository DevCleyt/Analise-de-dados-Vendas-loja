# 📊 Análise de Vendas de Rede de Lojas

Projeto desenvolvido em Python utilizando Pandas, NumPy e Matplotlib para realizar limpeza, tratamento, análise e visualização de dados de vendas de uma rede de lojas.

---

## 🧠 Mapa Mental do Projeto

<p align="center">
  <img src="mapa_mental.png" alt="Mapa Mental do Projeto" width="100%">
</p>

---

## 🎯 Objetivo

Realizar uma análise exploratória dos dados de vendas para identificar padrões de faturamento, desempenho das lojas, comparação com metas e geração de insights para apoio à tomada de decisão.

---

## 🛠 Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

---

## 📂 Base de Dados

O projeto utiliza dados relacionados a:

* Vendas realizadas
* Produtos comercializados
* Quantidade vendida
* Preço unitário
* Datas das vendas
* Metas dos gerentes
* Informações das lojas

---

## 🔄 Fluxo da Análise

### 1️⃣ Importação das Bibliotecas

```python
import pandas as pd
import numpy as np
from datetime import datetime
from matplotlib import pyplot as plt
```

---

### 2️⃣ Leitura dos Arquivos

```python
vendas_df = pd.read_csv('vendasTech.csv')
gerente_lojas_df = pd.read_excel('gerente_lojas.xlsx')
```

---

### 3️⃣ Limpeza e Tratamento dos Dados

* Tratamento de valores nulos
* Conversão de datas
* Padronização de texto
* Remoção de duplicados
* Ajuste de tipos de dados

---

### 4️⃣ Criação de Métricas

Criação da coluna de faturamento:

```python
vendas_df['Faturamento'] = (
    vendas_df['Qtd'] *
    vendas_df['Preco_Unitario']
)
```

Mapeamento das regiões das lojas.

---

### 5️⃣ Análises Realizadas

#### Faturamento por Loja

* Ranking das lojas
* Comparação de desempenho

#### Faturamento por Cidade

* São Paulo
* Rio de Janeiro

#### Produtos Mais Vendidos

* Quantidade por produto
* Ranking de vendas

#### Análise Temporal

* Faturamento por mês
* Evolução das vendas

#### Metas dos Gerentes

* Comparação entre faturamento e meta
* Identificação das lojas que atingiram os objetivos

---

## 📈 Principais Insights

✔ Identificação das lojas com maior faturamento

✔ Identificação das lojas com menor faturamento

✔ Produtos mais vendidos

✔ Comparação entre metas e resultados

✔ Distribuição das vendas por região

✔ Evolução do faturamento ao longo do tempo

---

## 📊 Visualizações

O projeto gera gráficos para facilitar a interpretação dos dados:

* Produtos mais vendidos
* Faturamento por mês
* Ranking de faturamento por loja

---

## 🚀 Como Executar

### Clone o repositório

```bash
git clone https://github.com/seu-usuario/analise-vendas-lojas-python.git
```

### Acesse a pasta

```bash
cd analise-vendas-lojas-python
```

### Instale as dependências

```bash
pip install pandas numpy matplotlib openpyxl
```

### Execute o Notebook

```bash
jupyter notebook
```

Abra:

```text
analiseLoja.ipynb
```

---

## 📚 Conceitos Aplicados

* Análise Exploratória de Dados (EDA)
* Limpeza de Dados
* Engenharia de Dados
* Manipulação com Pandas
* GroupBy
* Merge
* Filtros e Máscaras
* Visualização de Dados
* Indicadores de Negócio

---

## 👨‍💻 Autor

**Cleyton Pereira dos Santos**

Tecnólogo em Análise e Desenvolvimento de Sistemas.

Estudando:

* Python para Dados
* SQL
* Power BI
* Análise de Dados
* Automação com Python
