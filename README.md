# Case — Classificação de Reviews

## 📝 Descrição do Projeto

Este projeto tem como objetivo construir um modelo de **classificação de reviews de produtos** em **positivas** ou **negativas**.  
O dataset utilizado é o `olist_order_reviews_dataset.csv`, que contém informações sobre reviews de pedidos, incluindo nota, comentário e data.

O projeto segue os seguintes passos:

1. **Criação da variável alvo** (`label`):  
   - Positiva: nota >= 4  
   - Negativa: nota <= 2  
   - Neutras descartadas  

2. **Limpeza e pré-processamento de texto**:  
   - Remoção de HTML e URLs  
   - Minúsculas e remoção de caracteres especiais  
   - Lematização e remoção de stopwords em português  

3. **Exploração de dados (EDA)**:  
   - Distribuição das classes  
   - Comprimento médio das reviews  

4. **Pipeline de Machine Learning**:  
   - Vetorização TF-IDF (ngrams 1-2)  
   - Regressão Logística com `class_weight='balanced'`  
   - Validação cruzada e GridSearch para otimização de hiperparâmetros  

5. **Avaliação do modelo**:  
   - Classification report (F1, precisão, recall)  
   - Matriz de confusão  

6. **Bônus — Extração de aspectos**:  
   - Extração de palavras-chave e frases para identificar motivos de avaliação positiva ou negativa  

---

