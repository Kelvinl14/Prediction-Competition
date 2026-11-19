# Competição de Puns

Projeto de Aprendizado de Máquina para detecção automática de trocadilhos em textos escritos em português.

## Objetivo

Desenvolver um modelo de classificação binária capaz de identificar se um texto contém um trocadilho.

## Problema

- Tipo: Classificação binária.
- Entrada: Texto em português.
- Saída:
  - `1`: Contém trocadilho.
  - `0`: Não contém trocadilho.
- Métrica: Accuracy (Acurácia).

## Dataset

| Arquivo | Descrição |
|---|---|
| train.csv | Dados de treinamento, com rótulos |
| test.csv | Dados para previsão |
| sample_submission.csv | Modelo do arquivo de submissão |

## Tecnologias

- Python 3.11+
- Pandas e NumPy
- Scikit-learn
- Matplotlib e Seaborn
- NLTK / spaCy
- Transformers (Hugging Face)

## Metodologia

1. Análise exploratória dos dados (EDA).
2. Pré-processamento dos textos.
3. Construção de modelos baseline.
4. Treinamento e validação.
5. Otimização dos modelos.
6. Geração do arquivo de submissão.

## Modelos planejados

- TF-IDF + Regressão Logística.
- TF-IDF + SVM.
- Naive Bayes.
- BERTimbau (Fine-tuning).

## Submissão

O arquivo final deve ser salvo como `submission.csv`, contendo:

```csv
id,label
5.445.N,1
4.554.H,0
```

## Execução

Instale as dependências:

```bash
pip install -r requirements.txt
```

Execute os notebooks na ordem numérica definida na pasta `notebooks/`.

## Avaliação

A avaliação utiliza a acurácia entre as previsões e os rótulos reais do conjunto de teste.
