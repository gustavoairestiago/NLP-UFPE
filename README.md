# Classificador de Avaliações de Produto

Este repositório contém um projeto voltado para análise de avaliações de um produto específico, utilizando técnicas de aprendizado de máquina e processamento de linguagem natural para classificação de sentimentos. O projeto inclui três abordagens distintas de classificação.

## Link para o vídeo de apresentação
https://youtu.be/AC6o_nZEEeg

## Objetivos

1. **Treinar classificadores:** Comparar diferentes técnicas de classificação de sentimentos:
   - SVM + Bag of Words (BoW)
   - SVM + Embeddings
   - BERT (Bidirectional Encoder Representations from Transformers)

---

## Estrutura do Projeto

```
📂 projeto
├── 📁 data            # Diretório para armazenamento dos dados coletados
├── 📁 notebooks       # Notebooks Jupyter para exploração e treinamento
├── 📁 apresentação    # Apresentação com resultados e métricas de avaliação dos modelos
└── 📄 README.md       # Este arquivo
```

---

## Etapas do Projeto

### 1. Coleta de Dados
- **Fonte:** Avaliações coletadas da Amazon.
- **Campos:** Texto da avaliação, nota atribuída pelo usuário.

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
