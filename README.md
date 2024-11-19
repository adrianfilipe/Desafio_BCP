### Explicação do Projeto

Este projeto realiza a consolidação e análise de dados de negociação de debêntures extraídos do site da **ANBIMA**. Abaixo, estão as principais etapas do processo:

1. **Extração dos Dados**:
   - Os dados de negociação foram baixados para os últimos 5 dias úteis no formato `.txt` e posteriormente processados para `.xlsx`.
   - Cada arquivo foi transformado em um DataFrame.

2. **Consolidação dos Dados**:
   - Todos os DataFrames foram concatenados em um único dataset, alinhando as colunas e adicionando uma coluna de data para identificar o período de cada registro.

3. **Análise dos Dados**:
   - Foi calculada a **média da "Taxa Indicativa" por data**, utilizando agrupamento no pandas.
   - Um gráfico foi gerado para visualizar as variações médias da "Taxa Indicativa" ao longo do período analisado.

4. **Exportação**:
   - O dataset consolidado foi salvo como `dados_consolidados.xlsx` e `dados_consolidados.csv` para fácil integração com ferramentas como Power BI.

5. **Visualização**:
   - O gráfico de **"Taxa Indicativa Média por Data"** foi salvo como uma imagem para apresentações ou relatórios.


### Tecnologias Utilizadas

- **Python**: Para manipulação e análise dos dados.
  - Bibliotecas: `pandas`, `matplotlib`, `requests`
- **Jupyter Notebook**: Para desenvolvimento iterativo do projeto.
