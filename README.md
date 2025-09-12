# 📌 Classificação com Machine Learning – Dataset Breast Cancer

## 👨‍🏫 Disciplina
Inteligência Artificial  
Professor: Ronierison de Souza Maciel  
Aluno: Tiago Elias dos Santos 
Curso: Sistemas de Informação – VI Período, Noturno  

---

## 🎯 Objetivo da Atividade
Implementar e comparar algoritmos de classificação supervisionada utilizando um dataset real, aplicando técnicas de pré-processamento, modelagem e avaliação de desempenho.

---

## 📊 Dataset Escolhido
- **Fonte:** `sklearn.datasets.load_breast_cancer`  
- **Descrição:** O dataset contém características de tumores de mama, utilizados para prever se são **malignos (1)** ou **benignos (0)**.  
- **Tamanho:** 569 amostras × 30 features.  
- **Variável alvo:** diagnóstico (`maligno` ou `benigno`).  
- **Features:** raio, textura, perímetro, área, suavidade, compacidade, concavidade, simetria, entre outros.  

**Justificativa da escolha:**  
É um dataset clássico e muito utilizado em Machine Learning. Ele é balanceado, tem apenas duas classes (classificação binária), e contém variáveis numéricas que permitem aplicar diferentes algoritmos.

---

## ⚙️ Etapas Realizadas
### 🔹 4.2 – Preparação dos Dados
- Carregamento e exploração inicial (`head`, `info`, `describe`).  
- Separação entre atributos (`X`) e variável alvo (`y`).  
- Divisão em treino e teste com `train_test_split`.  

### 🔹 4.3 – Modelagem
Foram treinados e avaliados três algoritmos:
- DecisionTreeClassifier  
- KNeighborsClassifier  
- LogisticRegression  

Métricas avaliadas:
- Acurácia  
- Precisão  
- Recall  
- F1-score  
- Matriz de confusão  

Foi gerado também um **gráfico comparativo de acurácia** entre os modelos.

### 🔹 4.4 – Conclusão
O modelo com melhor desempenho foi a **Logistic Regression**, que atingiu a maior acurácia entre os três algoritmos.  
Esse resultado faz sentido, pois o dataset é relativamente bem separado linearmente, o que favorece modelos lineares.  

Possíveis melhorias:
- Aplicar normalização dos dados (melhora o desempenho do KNN).  
- Realizar tuning de hiperparâmetros (GridSearchCV ou RandomizedSearchCV).  
- Testar outros algoritmos, como Random Forest e SVM.  

---

## 📈 Resultados Obtidos (exemplo)
- **Decision Tree:** Acurácia ≈ 0.91  
- **KNN:** Acurácia ≈ 0.88  
- **Logistic Regression:** Acurácia ≈ 0.95  

> ⚠️ Os valores podem variar um pouco devido à aleatoriedade da divisão entre treino e teste.


