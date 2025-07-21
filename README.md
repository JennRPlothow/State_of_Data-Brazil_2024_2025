<p align="center">
  <img src="https://github.com/JennRPlothow/State_of_Data-Brazil_2024_2025/blob/main/state_of_data_banner.png" alt="Capa - State of Data Brazil 2024–2025" width="600"/>
</p>

# 📊 State of Data Brasil 2024–2025 — Análise Exploratória

Este projeto realiza uma **Análise Exploratória de Dados (EDA)** sobre a pesquisa _State of Data Brasil 2024–2025_, promovida pela [Data Hackers](https://www.datahackers.com.br/). A pesquisa visa mapear o perfil, os desafios, as competências e as ambições de profissionais da área de dados no Brasil.

> 🔗 Fonte dos dados:  
> https://www.kaggle.com/datasets/datahackers/state-of-data-brazil-20242025

---

## 🎯 Objetivo

Compreender as nuances da comunidade de dados no Brasil por meio de:

- Perfis demográficos (gênero, raça, região)
- Formação acadêmica
- Cargos e níveis hierárquicos
- Setores de atuação
- Desafios enfrentados por líderes
- Conhecimentos técnicos em Engenharia, Análise e Ciência de Dados

---

## 💾 Como carregar o dataset via código

Se estiver usando o pacote [`kagglehub`](https://pypi.org/project/kagglehub/), você pode carregar a base assim:

```python
import kagglehub

df = kagglehub.load_dataset(
  kagglehub.KaggleDatasetAdapter.PANDAS,
  "datahackers/state-of-data-brazil-20242025",
  "df_survey_2024.csv"
)
```

---

## 🧪 Metodologia

O notebook foi estruturado em etapas temáticas, baseadas nas **8 partes principais** do questionário da pesquisa:

1. **Dados Demográficos**: perfil pessoal (gênero, raça, região)  
2. **Carreira**: cargo atual, cargo como gestor, setor de atuação  
3. **Desafios dos Gestores**: dificuldades na liderança de times  
4. **Conhecimentos Gerais**: ferramentas, linguagens, conceitos  
5. **Objetivos Profissionais**: aspirações de carreira  
6. **Engenharia de Dados (DE)**: pipelines, bancos, cloud, etc.  
7. **Análise de Dados (DA)**: dashboards, KPIs, storytelling  
8. **Ciência de Dados (DS)**: estatística, machine learning, modelagem  

Cada coluna da base de dados é codificada com o padrão: `P[parte][letra]_[opção]` (ex: `P2f_1` → Parte 2, pergunta f, opção 1).

---

## 📊 O que foi analisado

- **Distribuição de gênero por cargo e por setor**
- **Presença de mulheres em cargos de gestão**
- **Comparativo entre setores (TI, Educação, Finanças, etc.)**
- **Relação entre formação acadêmica e cargo**
- **Desigualdades regionais**
- **Proporções raciais nas posições de liderança**
- **Gráficos de pizza e barras para composição de setores, formação e cargos**
- **Análise cruzada entre variáveis para entender padrões sociais e técnicos**

---

## 📁 Estrutura do Projeto

```
📦 state-of-data-2024-eda
├── EDA_State_of_Data_2024_2025.ipynb  # Notebook principal com toda a análise
├── README.md                          # Este arquivo
└── requirements.txt                   # Bibliotecas utilizadas
```

---

## 🧰 Bibliotecas Utilizadas

As bibliotecas abaixo já estão disponíveis no Google Colab:

```
pandas
numpy
matplotlib
seaborn
```

---

## ✅ Como Executar

1. Acesse o [Google Colab](https://colab.research.google.com/)
2. Faça upload do notebook `EDA_State_of_Data_2024_2025.ipynb`
3. Faça upload do dataset CSV baixado do Kaggle
4. Execute o notebook célula por célula


---

## 📌 Principais Insights

- A região Sudeste domina em representatividade.
- Profissionais de TI são maioria nos cargos de liderança.
- A presença feminina e de pessoas negras é reduzida em níveis mais altos.
- O setor financeiro lidera em empregabilidade, seguido por tecnologia e educação.
- Formação acadêmica ainda influencia fortemente a ocupação de cargos estratégicos.

---

## 📄 Licença

Distribuído sob a Licença MIT.

---

## ✍️ Autor

Desenvolvido por **Jennifer Plothow**  
🧠 Com dados, clareza e propósito.

---

> _“Explorar os dados é compreender a sociedade com lentes estatísticas.”_
