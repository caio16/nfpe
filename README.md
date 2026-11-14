# Predição de Não Funcionamento Primário do Enxerto (NFPE) em Transplante Hepático

Repositório para o projeto de Iniciação Científica da Universidade Federal do ABC, focado em aplicar e comparar algoritmos de Machine Learning (Regressão Logística Penalizada, Random Forest e Gradient Boosting) para prever o NFPE.

## Tecnologias e Ferramentas
- **R (>= 4.1)**: Pipeline de Análise Exploratória (EDA), completude e importância de permutação[cite: 4].
- **Python**: Tutorial de aplicação de ML com `scikit-learn`, `PyTorch` e explicabilidade com `SHAP`[cite: 1, 3].
- **Ollama**: Revisão local utilizando LLMs (ex: gemma2:9b)[cite: 4].
- **renv**: Gerenciamento de dependências no R[cite: 4].

## Como executar o pipeline atual (R)
1. Instale as dependências: `renv::restore()`[cite: 4].
2. Copie `.Renviron.example` para `.Renviron` e preencha as variáveis de ambiente necessárias (como a `SHEET_URL` do Google Sheets)[cite: 4].
3. Execute a extração e EDA:
   ```bash
   Rscript scripts/run_completeness.R
   Rscript scripts/run_eda.R

   
