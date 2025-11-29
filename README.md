# Análise COVID-19 x Google Trends – São Paulo

Este repositório contém os dados e o notebook usados na análise da relação entre casos de COVID-19 no estado de São Paulo e o interesse pelo tema medido via Google Trends.

## Arquivos

- `analise_covid_trends_sp_corrigido_final-1.ipynb`  
  Notebook em Python com toda a análise (limpeza básica, agregações, gráficos, correlações etc.).  
- `Dados_Covid_e_Trends/`  
  - `sp_2020.xlsx` … `sp_2025.xlsx`: arquivos semanais com casos novos de COVID-19 em São Paulo.  
    - Colunas típicas: `Ano_Semana` e `Casos Novos`.
  - `saopaulo_timeline.csv`: série mensal do Google Trends para o termo “COVID-19” em São Paulo, com colunas `Mês` e `COVID-19: (São Paulo)`.

## Como rodar a análise

Pré-requisitos:

- Python 3.x instalado
- Jupyter Notebook ou JupyterLab
- Pacotes básicos: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `scipy`

Passos:

1. Clonar ou baixar este repositório.  
2. Garantir que a estrutura esteja assim:  
   - `analise_covid_trends_sp_corrigido_final-1.ipynb`  
   - `dados/sp_2020.xlsx` … `dados/sp_2025.xlsx`  
   - `dados/saopaulo_timeline.csv`.
3. (Opcional, mas recomendado) criar um ambiente virtual e instalar dependências:  
   - `pip install pandas numpy matplotlib seaborn statsmodels scipy jupyter`  
4. Abrir o notebook:  
   - `jupyter notebook analise_covid_trends_sp_corrigido_final-1.ipynb`  
5. Rodar as células de cima para baixo.  
   - O notebook lê diretamente os arquivos de `dados/` (ajuste os caminhos se necessário).  
   - As figuras e estatísticas usadas no artigo são geradas a partir desse notebook.

## Reprodutibilidade

Qualquer pessoa com os arquivos da pasta `Dados_Covid_e_Trends/` e este notebook consegue reproduzir os resultados seguindo os passos acima. Caso algum arquivo seja atualizado (por exemplo, inclusão de novos anos), basta substituir na pasta `dados/` e reexecutar o notebook.
