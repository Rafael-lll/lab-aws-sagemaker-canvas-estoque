# 📊 Previsão de Estoque Inteligente na AWS com [SageMaker Canvas](https://aws.amazon.com/pt/sagemaker/canvas/)


## 🚀 Passo a Passo

### 1. Selecionar Dataset

É o ponto de partida, onde eu escolho o arquivo ou banco de dados que contém todo o histórico de vendas e movimentação que a IA vai precisar ler, escolhi o segundo arquivo na pasta de datasets.

### 2. Construção (Build)

Aqui eu defino o objetivo: prever a QUANTIDADE_ESTOQUE.

Configuro os detalhes importantes: o ID_PRODUTO para separar os itens, a DATA_EVENTO para a linha do tempo e o PRECO como uma variável que eu já sei que vai influenciar o futuro.

Uso o "Quick build" para a IA montar uma primeira versão do modelo rapidamente.

### 3. Análise (Analyze)

Nesta parte, eu confiro o "boletim" da IA através das métricas de erro (como RMSE e MAPE) para saber se os cálculos são confiáveis.

Analiso os impactos: vi que o preço é o que mais manda no estoque (51,05%), seguido pelos feriados nacionais (12,8%).

### 4. Previsão (Predict)

É onde eu vejo o resultado final. Escolho um produto e o gráfico me mostra as três linhas de previsão (P10, P50 e P90).

Isso me ajuda a decidir se compro o mínimo necessário para não sobrar (P10) ou se me preparo para uma venda muito alta (P90).
