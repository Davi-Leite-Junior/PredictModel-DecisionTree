# DecisionTree

Este README descreve o notebook `DecisionTree.ipynb`, que implementa um modelo de árvore de decisão usando o conjunto de dados `Credit.csv`.

## Objetivo

Treinar e avaliar um classificador `DecisionTreeClassifier` para prever a classe de crédito com base em atributos do dataset.

## Requisitos

- Python 3.x
- pandas
- scikit-learn
- yellowbrick (opcional, para visualização)

## Como usar

1. Abra o notebook `DecisionTree.ipynb` em Jupyter ou VS Code.
2. Verifique o caminho do arquivo `Credit.csv` e ajuste se necessário.
3. Execute as células na ordem.

## O que o notebook faz

1. Importa as bibliotecas necessárias: `pandas`, `LabelEncoder`, `train_test_split`, `DecisionTreeClassifier`, `export_graphviz`, `confusion_matrix` e `accuracy_score`.
2. Lê os dados de `Credit.csv`.
3. Separa os atributos (`previsores`) e a classe alvo (`classe`).
4. Converte colunas categóricas em valores numéricos usando `LabelEncoder`.
5. Divide os dados em conjuntos de treino e teste com `train_test_split`.
6. Treina o modelo `DecisionTreeClassifier`.
7. Exporta a árvore para arquivo `tree.dot`.
8. Faz previsões com o conjunto de teste.
9. Calcula a matriz de confusão e a taxa de acerto.

## Observações

- A importação `from yellowbrick.classifier import ConfusionMatrix` é opcional e pode ser removida se o módulo `yellowbrick` não estiver instalado.
- A visualização da árvore pode ser gerada a partir do arquivo `tree.dot` usando ferramentas como Graphviz.

## Licença

Projeto para estudo pessoal.
