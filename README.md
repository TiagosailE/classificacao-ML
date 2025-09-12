# 📊 Classificação com Machine Learning – Dataset Breast Cancer

## 👤 Autor
- Nome: Tiago Elias dos Santos Jovencio
- Disciplina: Inteligência Artificial
- Professor: Ronierison de Souza Maciel
- Curso: Sistemas de Informação – VI Período, Noturno

---

## 🎯 Objetivo da Atividade
Implementar e comparar algoritmos de **classificação supervisionada** utilizando um dataset real, aplicando:
- Pré-processamento
- Modelagem
- Avaliação de desempenho

Os resultados devem ser versionados em um repositório no GitHub, com commits graduais e descritivos.

---

## 📂 Dataset Utilizado
- Fonte: `sklearn.datasets.load_breast_cancer`
- Tamanho: **569 amostras × 30 features**
- Variável alvo: diagnóstico do tumor (`0 = maligno`, `1 = benigno`)
- Features: medidas obtidas de exames de mama (raio médio, textura, perímetro, área, suavidade etc.)

**Justificativa da escolha:**  
É um dataset clássico, balanceado e de tamanho adequado para experimentos de aprendizado de máquina supervisionado.

---

## ⚙️ Modelos de Classificação
Foram testados três algoritmos:

1. **Decision Tree**  
2. **K-Nearest Neighbors (KNN)**  
3. **Logistic Regression**  

---

## 📈 Resultados Obtidos

### Métricas principais (dados de teste)
| Modelo               | Acurácia | Precisão | Recall | F1-Score |
|----------------------|----------|----------|--------|----------|
| Decision Tree        | ~0.918   | ~0.919   | ~0.918 | ~0.918   |
| KNN                  | ~0.930   | ~0.931   | ~0.930 | ~0.930   |
| Logistic Regression  | ~0.959   | ~0.960   | ~0.959 | ~0.959   |

### Comparação de acurácia
O gráfico gerado no notebook mostra que **Logistic Regression** obteve o melhor desempenho.

---

## 📝 Conclusão
- O melhor modelo foi a **Regressão Logística**, com maior acurácia.  
- Isso faz sentido, pois o dataset é majoritariamente linearmente separável.  
- O KNN teve desempenho próximo, mas poderia melhorar com normalização dos dados.  
- Árvores de decisão também se saíram bem, mas com menor precisão.  

**Possíveis melhorias:**
- Normalização das features (especialmente útil para KNN).  
- Ajuste de hiperparâmetros via Grid Search.  
- Testar outros algoritmos, como Random Forest ou SVM.  

