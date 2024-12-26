# Classificador de Avaliações de Produto

Este repositório contém um projeto voltado para coleta e análise de avaliações de um produto específico, utilizando técnicas de aprendizado de máquina e processamento de linguagem natural para classificação de sentimentos. O projeto inclui três abordagens distintas de classificação.

## Objetivos

1. **Coletar dados:** Captura de textos de avaliações e suas respectivas notas para o produto selecionado.
2. **Treinar classificadores:** Comparar diferentes técnicas de classificação de sentimentos:
   - SVM + Bag of Words (BoW)
   - SVM + Embeddings
   - BERT (Bidirectional Encoder Representations from Transformers)

---

## Estrutura do Projeto

```
📂 projeto
├── 📁 data            # Diretório para armazenamento dos dados coletados
├── 📁 notebooks       # Notebooks Jupyter para exploração e treinamento
├── 📁 models          # Modelos treinados e checkpoints
├── 📁 results         # Resultados e métricas de avaliação dos modelos
└── 📄 README.md        # Este arquivo
```

---

## Etapas do Projeto

### 1. Coleta de Dados
- **Fonte:** Avaliações coletadas de plataformas públicas (e.g., Amazon, Mercado Livre).
- **Campos:** Texto da avaliação, nota atribuída pelo usuário.
- **Script:** `scripts/data_collection.py` realiza a coleta e o pré-processamento dos dados.

### 2. Pré-processamento
- Tokenização
- Limpeza de texto (remoção de stopwords, pontuações, etc.)
- Representação textual (BoW, embeddings ou tokenização do BERT).

### 3. Treinamento dos Modelos
- **SVM + BoW:** Baseado em contagem ou frequência de palavras.
- **SVM + Embeddings:** Utiliza vetores pré-treinados (e.g., GloVe, Word2Vec).
- **BERT:** Modelo pré-treinado para representação contextualizada de texto.

### 4. Avaliação
- Métricas utilizadas: Acurácia, F1-Score, Precision e Recall.
- Comparação entre as abordagens para determinar a melhor performance.

---

## Tecnologias Utilizadas

- **Linguagens:** Python
- **Bibliotecas:**
  - Pandas, NumPy (manipulação de dados)
  - Scikit-learn (SVM e validação)
  - TensorFlow / PyTorch (BERT)
  - NLTK / SpaCy (processamento de texto)
  - Matplotlib / Seaborn (visualização de dados)

---
