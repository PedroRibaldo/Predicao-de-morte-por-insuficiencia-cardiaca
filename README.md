# Predição de Morte por Insuficiência Cardíaca  
Projeto Acadêmico – Inteligência Artificial (FACAMP)

---

## 📑 Sumário
1. [Descrição do Projeto](#descrição-do-projeto)  
2. [Contexto Acadêmico](#contexto-acadêmico)  
3. [Fonte dos Dados](#fonte-dos-dados)  
4. [Tecnologias Utilizadas](#tecnologias-utilizadas)  
5. [Como Executar o Projeto](#como-executar-o-projeto)  
6. [Pipeline do Projeto](#pipeline-do-projeto)  
7. [Modelos Utilizados](#modelos-utilizados)  
8. [Resultados](#resultados)  
9. [Conclusões](#conclusões)  
10. [Autores](#autores)

---

## 📘 Descrição do Projeto
Este projeto tem como objetivo **prever a probabilidade de morte por insuficiência cardíaca** utilizando técnicas de Machine Learning aplicadas a um conjunto de dados clínicos reais.

O foco é analisar como diferentes modelos se comportam ao tentar identificar padrões que indiquem maior risco de mortalidade, contribuindo para o entendimento de fatores relevantes na área da saúde.

---

## 🎓 Contexto Acadêmico
Este trabalho foi desenvolvido como parte da disciplina de **Inteligência Artificial** do curso de Engenharia da Computação (FACAMP).

O objetivo da atividade era aplicar conceitos estudados em aula, incluindo:

- pré-processamento de dados  
- separação de treino e teste  
- normalização  
- treinamento de modelos  
- análise comparativa de métricas  

---

## 📊 Fonte dos Dados
O dataset utilizado está disponível no Kaggle:

🔗 **Heart Failure Clinical Data**  
https://www.kaggle.com/datasets/andrewmvd/heart-failure-clinical-data

O conjunto contém informações clínicas de pacientes, como idade, pressão arterial, fração de ejeção, níveis de creatinina, entre outras variáveis relevantes.

---

## 🛠 Tecnologias Utilizadas

### Linguagem:
- **Python 3.9** (executado via Google Colab)

### Bibliotecas principais:
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

---

## ▶ Como Executar o Projeto

### **1. Executando no Google Colab (Método recomendado)**

1. Baixe o dataset no Kaggle (link acima).  
2. Faça upload do arquivo CSV na pasta onde o notebook será executado.  
3. Ajuste o caminho do arquivo no notebook, se necessário.

> Obs.: Não há integração automática com Google Drive. Caso deseje carregar o dataset do Drive, será necessário adicionar o `drive.mount()` manualmente.

---

### **2. Requisitos**

Para quem quiser rodar localmente, podem ser utilizadas as seguintes dependências:
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

---

## 📂 Pipeline do Projeto

O notebook segue a estrutura:

0. **Importação do Dataset**  
   Carregamento dos dados clínicos e leitura inicial do CSV.

1. **Sobre o Problema**  
   Contextualização da tarefa de previsão da mortalidade por insuficiência cardíaca.

2. **Carregamento e Ajuste dos Dados**  
   - Leitura do dataset.  
   - Conversão dos nomes das colunas para português para facilitar a interpretação.

3. **Exploração dos Dados (EDA)**  
   - Visualização das primeiras linhas.  
   - Análise estatística.  
   - Geração de gráficos exploratórios.

4. **Limpeza dos Dados**  
   - Separação em variáveis independentes (`X`) e dependente (`y`).  
   - Remoção de colunas consideradas desnecessárias.  
   - Tratamento de outliers.

5. **Pré-processamento**  
   - Normalização/padronização das variáveis.  
   - Separação em conjuntos de treino e teste.

6. **Treinamento dos Modelos**  
   Foram treinados três algoritmos:
   - **KNN (K-Nearest Neighbors)**  
   - **Regressão Logística**  
   - **Decision Tree Classifier**

7. **Avaliação e Comparação dos Modelos**  
   - Cálculo da acurácia.  
   - Curva ROC.
   - Métrica AUC.  
   - Comparação entre os três modelos.

8. **Conclusão Final**  
   Interpretação dos resultados e determinação do melhor modelo para o problema.

---

## 🤖 Modelos Utilizados
Foram testados três modelos clássicos de classificação:

- **K-Nearest Neighbors (KNN)**
- **Regressão Logística**
- **Árvore de Decisão** *(melhor desempenho)*

---

## 📈 Resultados

Os modelos apresentaram desempenhos próximos, porém a **Árvore de Decisão** teve o melhor resultado considerando:

- **Acurácia**
- **AUC (Area Under the Curve)**

---

## 🧠 Conclusões

- As variáveis clínicas presentes no dataset demonstram forte potencial para prever mortalidade por insuficiência cardíaca.
- A **Árvore de Decisão** apresentou desempenho levemente superior aos demais modelos, sendo a mais adequada dentro das opções avaliadas.
- O projeto mostrou que algoritmos supervisionados simples podem alcançar resultados consideravelmente satisfatórios.
- Para trabalhos futuros, recomenda-se testar:
  - Random Forest  
  - XGBoost  
  - Métodos de balanceamento (SMOTE)  
  - Otimização de hiperparâmetros (GridSearchCV)  

---

## 👥 Autores

### <a href="https://www.linkedin.com/in/gabriel-bertazzoli/" target="_blank"> **Gabriel Bertazzoli** <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/linkedin/default.svg" width="20" height="20" /> </a>

### <a href="https://www.linkedin.com/in/pedro-ribaldo-marques" target="_blank">**Pedro Marques** <img src="https://raw.githubusercontent.com/maurodesouza/profile-readme-generator/master/src/assets/icons/social/linkedin/default.svg" width="20" height="20" /> </a>
