# kNN-no-Instagram

# **Análise de Influenciadores do Instagram**

## **Descrição do Projeto**

Este projeto utiliza técnicas de aprendizado de máquina para analisar dados de influenciadores do Instagram. O objetivo principal é explorar como diferentes variáveis, como número de seguidores, engajamento e localização geográfica, influenciam o desempenho e a popularidade desses influenciadores. Além disso, foi realizada uma comparação entre modelos de regressão, incluindo k-Nearest Neighbors (k-NN), Random Forest, Gradient Boosting e Regressão Linear, para prever métricas como engajamento e pontuação de influência.

---

## **Descrição da Base de Dados**

O conjunto de dados contém informações detalhadas sobre influenciadores do Instagram, incluindo:

- **Followers**: Número de seguidores.
- **Avg Likes**: Média de likes por postagem.
- **60 Day Engagement Rate**: Taxa de engajamento nos últimos 60 dias.
- **Country**: País de origem do influenciador.
- **Influence Score**: Pontuação que reflete a importância do influenciador.
- **New Post Avg Likes**: Média de likes por post novo.

Outras variáveis categóricas e numéricas estão incluídas para complementar as análises.

---

## **Instruções para Replicação no Google Colab**

1. **Acesse o Google Colab**:

   - Entre no [Google Colab](https://colab.research.google.com).
2. **Carregue o Notebook**:

   - Faça o upload do arquivo `influencers_analysis.ipynb` no Colab ou abra o notebook diretamente do repositório, caso ele esteja disponível online.
3. **Envie o Dataset**:

   - Certifique-se de fazer o upload do arquivo de dados (ex.: `influencers_data.csv`) no Colab ou importe o dataset diretamente de uma URL se ele estiver hospedado.
4. **Execute o Notebook**:

   - Siga as células do notebook e execute-as em sequência. As dependências serão instaladas automaticamente.
5. **Instalação de Dependências no Colab**:

   - Certifique-se de que as bibliotecas necessárias estão instaladas no ambiente do Colab. O notebook já inclui os comandos para instalação:
     ```python
     !pip install pandas numpy matplotlib seaborn scikit-learn
     ```
6. **Resultados e Visualizações**:

   - Os gráficos e visualizações serão exibidos diretamente no Colab ao final de cada célula relevante.
   - As métricas de avaliação serão exibidas no console.

---

## **Resultados**

1. **Métricas de Avaliação**:

   - Melhor modelo: **Random Forest**
   - Métricas do melhor modelo:
     - **MAE**: 7.95
     - **MSE**: 210.47
     - **RMSE**: 14.51
2. **Comparação entre Modelos**:

   - O modelo k-NN apresentou desempenho inferior ao Random Forest e Gradient Boosting, mas foi uma abordagem válida para o dataset analisado.
   - A Regressão Linear teve o desempenho mais fraco, devido à sua incapacidade de capturar relações não lineares entre as variáveis.
3. **Insights**:

   - Países com maior número de influenciadores têm maior diversidade em métricas como engajamento e influência.
   - Taxas de engajamento variam significativamente entre regiões, com influenciadores de países com bases menores de seguidores frequentemente apresentando engajamento mais alto.

---

## **Estrutura do Repositório**

- `data/`: Contém os arquivos de dados.
- `notebooks/`: Contém notebooks de exploração e desenvolvimento.
- `outputs/`: Contém gráficos e relatórios gerados.
- `README.md`: Este arquivo.
