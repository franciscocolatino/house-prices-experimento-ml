🏠 Experimento de Regressão - House Prices

Este repositório contém um experimento de Aprendizado de Máquina aplicado ao conjunto de dados Ames Housing Dataset, com o objetivo de prever o preço de imóveis a partir de suas características.

------------------------------------------------------------
🎯 Objetivo

Avaliar e comparar o desempenho de diferentes algoritmos de regressão na tarefa de predição de preços de imóveis. 
O experimento busca identificar o modelo que oferece o melhor equilíbrio entre erro e capacidade preditiva.

------------------------------------------------------------
📦 Dataset

• Fonte: Kaggle – Ames Housing Dataset
• Tamanho: ~500 amostras  
• Descrição: Inclui variáveis como área construída, número de quartos, banheiros, localização, entre outras.  
• Variável alvo: Preço de venda

------------------------------------------------------------
⚙️ Modelos testados

Modelo               | RMSE          | MAE           | R²
----------------------|---------------|---------------|---------
Linear Regression     | 8.48e+08      | 15711.5       | 0.894
Ridge                 | 8.27e+08      | 16158.6       | 0.897
Lasso                 | 8.41e+08      | 15674.4       | 0.895
Random Forest         | 7.11e+08      | 15906.5       | 0.911
XGBoost               | 6.85e+08      | 15534.9       | 0.914
Random Forest (Optuna)| 7.22e+08      | 15831.6       | 0.910
XGBoost (Optuna)      | 6.06e+08      | 13766.8       | 0.924

------------------------------------------------------------
🔍 Conclusões iniciais

• O XGBoost tunado apresentou o melhor desempenho geral, alcançando o maior valor de R² (0.924) e o menor erro (RMSE e MAE).  
• Modelos lineares (Ridge e Lasso) apresentaram resultados consistentes, mas inferiores aos modelos baseados em árvores.  
• O Random Forest também se destacou, com desempenho próximo ao do XGBoost.

------------------------------------------------------------
🧪 Tuning e otimização

Foi utilizada a biblioteca Optuna para otimização de hiperparâmetros, com foco em maximizar o R² e reduzir o RMSE.  
O experimento pode ser facilmente reproduzido ajustando os parâmetros no notebook principal:

    experimento_house_prices.ipynb

------------------------------------------------------------
🧰 Tecnologias utilizadas

• Python 3  
• Pandas, NumPy  
• Scikit-Learn  
• XGBoost  
• Optuna  
• Matplotlib / Seaborn  

------------------------------------------------------------
🚀 Execução

1. Clone o repositório:
```bash
   git clone https://github.com/franciscocolatino/house-prices-ml-experimento.git
   cd house-prices-ml-experimento
```

2. Instale as dependências:
```bash
   pip install -r requirements.txt
```

3. Execute o notebook no Jupyter ou Google Colab:
```bash
   experimento_house_prices.ipynb
```

------------------------------------------------------------
✍️ Autores

Anderson Passos  
Francisco Colatino  
Jônatas Duarte  

------------------------------------------------------------
Universidade Federal de Alagoas — 2025  
Disciplina: Planejamento de Experimentos
