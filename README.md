# 🍷 Previsão de Qualidade de Vinhos com Random Forest

## 📌 Objetivo do Projeto

Desenvolver um modelo de Machine Learning capaz de prever a **qualidade de vinhos** com base em suas características físico-químicas, auxiliando processos de controle de qualidade e tomada de decisão na indústria vinícola.

---

## 📊 Base de Dados

A base contém **1.599 amostras de vinhos** com **11 variáveis numéricas** como:

* acidez
* teor alcoólico
* pH
* dióxido de enxofre
* densidade
* entre outras

A variável alvo é **quality (0 a 10)**.

---

## 🔍 Etapas do Projeto

### 1. Análise Exploratória (EDA)

* Distribuição da variável target
* Identificação de outliers
* Matriz de correlação
* Teste de hipóteses (ex: álcool vs qualidade)

---

### 2. Pré-processamento

* Split treino/teste
* Análise de desbalanceamento
* Uso de `class_weight='balanced'`

---

### 3. Modelagem

#### 🔹 Modelo 1 — Baseline

* Random Forest padrão
* Accuracy: **66%**

#### 🔹 Modelo 2 — Otimizado

* RandomizedSearchCV
* Ajuste de hiperparâmetros
* Métrica foco: **F1 Macro**
* Accuracy: **67%**
* Melhora significativa na média macro

---

## 📈 Resultados

| Métrica  | Baseline | Modelo Final |
| -------- | -------- | ------------ |
| Accuracy | 0.66     | 0.67         |
| F1 Macro | 0.36     | 0.44         |

O modelo final apresentou **melhor equilíbrio entre classes**, principalmente nas classes minoritárias.

---

## 🔬 Principais Variáveis Importantes

* Teor alcoólico
* Acidez volátil
* Sulfatos
* Dióxido de enxofre total
* Densidade

---

## 💡 Insights de Negócio

* Vinhos com maior teor alcoólico tendem a ter maior qualidade
* Alta acidez volátil impacta negativamente a qualidade
* Sulfatos estão associados a melhores avaliações
* Características químicas têm impacto direto na percepção do produto final

---

## 🛠 Tecnologias Utilizadas

* Python
* Pandas
* Matplotlib / Seaborn
* Scikit-learn

---

## 📌 Próximos Passos

* Testar outros modelos (XGBoost, LightGBM)
* Aplicar SHAP Values para interpretabilidade avançada
* Deploy do modelo

---

## 👨‍💻 Autor

**Maylson Maia**

Projeto desenvolvido para portfólio de Ciência de Dados.
