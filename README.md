# 🚀 PROJETO: Análise de Impacto Macroeconômico no E-commerce Brasileiro (2020-2025)

## 1. 🎯 Objetivo Principal

Identificar, analisar e prever como as principais variáveis macroeconômicas do Brasil (Selic, IPCA, Desemprego, etc.) impactam o desempenho financeiro (Receita Líquida) e operacional (Margem EBITDA) dos principais *players* de e-commerce listados na B3 (Magazine Luiza, Via, Mercado Livre), gerando *insights* estratégicos e um modelo preditivo simples.

---

## 2. ❓ Perguntas-Chave de Negócio (O Nosso Norte)

Este projeto se propõe a responder 4 perguntas centrais:

1.  **[Impacto Direto]:** Como a variação da **Taxa Selic** e do **IPCA** impacta diretamente o crescimento da **Receita Líquida** das varejistas?
2.  **[Eficiência Operacional]:** Qual é a correlação entre a **Taxa de Desocupação** (Desemprego) e a **Margem EBITDA** das empresas? A eficiência operacional é comprimida em períodos de alto desemprego?
3.  **[Análise de Resiliência]:** Quais empresas demonstraram maior **resiliência** (menor queda na Margem EBITDA) durante os períodos de maior aperto monetário (ciclos de alta da Selic)?
4.  **[Análise Preditiva]:** O **Índice de Confiança do Consumidor** e o **IBC-Br** (Proxy do PIB) funcionam como *indicadores antecedentes* para a **Receita Líquida** do trimestre seguinte?

---

## 3. 💾 Fontes de Dados (Data Sources)

| Dado | Categoria | Fonte | Ferramenta de Coleta |
| :--- | :--- | :--- | :--- |
| **Receita Líquida (Trimestral)** | E-commerce | Yahoo Finance | Python (`yfinance`) |
| **Margem EBITDA (Trimestral)** | E-commerce | Yahoo Finance | Python (`yfinance`) |
| **Interesse de Busca** | E-commerce | Google Trends | Python (`pytrends`) |
| **Taxa Selic (Meta Mensal)** | Macroeconômico | Banco Central (SGS) | Python (API do BCB) |
| **IPCA (Var. % Mensal)** | Macroeconômico | Banco Central (SGS) | Python (API do BCB) |
| **IBC-Br (Proxy do PIB)** | Macroeconômico | Banco Central (SGS) | Python (API do BCB) |
| **Confiança do Consumidor** | Macroeconômico | Banco Central (SGS) | Python (API do BCB) |
| **Taxa de Desocupação** | Macroeconômico | IBGE (SIDRA) | Python (`sidrapy`) |

---

## 4. 🛠️ Tech Stack (Ferramentas)

* **Coleta (ETL):** `Python` (`pandas`, `requests`, `yfinance`, `sidrapy`, `pytrends`)
* **Armazenamento e Modelagem:** `SQL` (via `SQLite` e `DBeaver`)
* **Análise Exploratória (EDA):** `Python` (`matplotlib`, `seaborn`, `Jupyter Notebooks`)
* **Análise Rápida e Simulações:** `Excel` (Fórmulas Avançadas, Power Query)
* **Visualização e Storytelling:** `Power BI` (DAX, Modelagem, Layout)
* **Versionamento e Portfólio:** `Git` / `GitHub`
* **Divulgação:** `LinkedIn`

---

## 5. 💡 Habilidades e Conceitos-Chave

Este projeto foi desenhado para desenvolver e demonstrar domínio sobre:

* **Business Acumen:**
    * Tradução de problemas de negócio em perguntas analíticas.
    * Análise de DRE (Demonstração do Resultado do Exercício).
    * Interpretação de KPIs (EBITDA, Receita Líquida, Margens).
    * Compreensão de conceitos macroeconômicos (Juros, Inflação, PIB).
* **Engenharia de Dados (Leve):**
    * Consumo de APIs (REST) para coleta de dados públicos (BCB).
    * Uso de *wrappers* de API (`yfinance`, `sidrapy`).
    * Criação de um pipeline ETL simples (Extração, Transformação, Carga).
    * Modelagem de dados relacional (criação de tabelas Fato e Dimensão em `SQLite`).
* **Análise de Dados:**
    * Limpeza e tratamento de dados (`pandas`).
    * Padronização e transformação de séries temporais (agregação de Mensal para Trimestral).
    * Análise Exploratória de Dados (EDA) e Estatística Descritiva.
    * Análise de Correlação (Pearson, Spearman) e *Heatmaps*.
    * Análise de Causalidade (simples) e defasagem (*lag analysis*).
* **Análise Preditiva (Foco em Negócio):**
    * Modelagem de Regressão Linear Simples (em Python e Excel).
    * Análise de Tendência e Sazonalidade.
    * Criação de Cenários "E Se" (Simulação).
* **Business Intelligence & Storytelling:**
    * Cálculos em DAX (`CALCULATE`, `SAMEPERIODLASTYEAR`, etc.).
    * Criação de Dashboards executivos interativos.
    * Uso de visuais adequados para cada tipo de dado (Séries Temporais, Correlação).
    * Comunicação de *insights* complexos de forma simples.

---

## 6. 🏁 Entregáveis do Projeto

1.  **Repositório no GitHub:** Contendo todo o código (`.py`, `.ipynb`), o banco de dados (`.db`) e a documentação (`README.md`).
2.  **Banco de Dados:** Um arquivo `SQLite` (`ecommerce_macro.db`) com os dados limpos e modelados.
3.  **Dashboard Executivo:** Um painel publicado no `Power BI Service` (link público).
4.  **Artigo de Portfólio:** Uma postagem no `LinkedIn` detalhando a metodologia, os principais *insights* e as conclusões de negócio, com link para o GitHub e para o Dashboard.