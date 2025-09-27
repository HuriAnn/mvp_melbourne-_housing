# 🏡 Projeto de Previsão de Preços de Imóveis em Melbourne
📌 Descrição Desenvolvimento de um modelo preditivo para estimar o preço de imóveis na cidade de Melbourne com base em atributos como localização, número de cômodos, área construída, tipo de imóvel e presença de vaga de garagem. O projeto inclui EDA, tratamento de dados, modelagem supervisionada e preparação para visualização em dashboard.

## 🗂️ Escopo do Trabalho
1️⃣ Carregamento e limpeza dos dados

2️⃣ Análise Exploratória (distribuições, correlações, outliers) 

3️⃣ Transformações e engenharia de atributos 

4️⃣ Separação entre treino e teste 

5️⃣ Modelagem preditiva (Linear, Ridge, Random Forest, Comitê) 

6️⃣ Validação cruzada e otimização de hiperparâmetros 

7️⃣ Preparação da base para Power BI


## 📚 Dados Utilizados

Origem: Kaggle – Melbourne Housing Market Registros: ~13.000 

Variável alvo: Preço de venda (log-transformado)

## 📖 Dicionário de Dados

| 🏷️ Variável       | 📊 Tipo      | 📝 Descrição                                                                 |
|-------------------|-------------|------------------------------------------------------------------------------|
| **Suburb**        | Categórica  | Nome do subúrbio onde o imóvel está localizado                              |
| **Address**       | Texto       | Endereço da propriedade                                                      |
| **Rooms**         | Numérica    | Número de cômodos no imóvel (exclui banheiros e espaços não residenciais)   |
| **Price**         | Numérica    | Preço de venda do imóvel em dólares australianos (AUD)                      |
| **Method**        | Categórica  | Método de venda (S, SP, PI, PN, SN, VB, W, SA)                               |
| **Type**          | Categórica  | Tipo de imóvel (h = casa, t = sobrado, u = unidade/apartamento)             |
| **SellerG**       | Categórica  | Agência imobiliária ou agente responsável pela venda                         |
| **Date**          | Categórica  | Data da venda                                                                |
| **Distance**      | Numérica    | Distância até o centro comercial de Melbourne (CBD) em quilômetros          |
| **Regionname**    | Categórica  | Nome da região geográfica (ex: Metropolitano Oriental, Norte, Sul, etc.)    |
| **Propertycount** | Numérica    | Número de imóveis existentes no subúrbio                                    |
| **Bedroom2**      | Numérica    | Número de quartos (inclui espaços não residenciais que podem ser usados)    |
| **Bathroom**      | Numérica    | Número de banheiros                                                          |
| **Car**           | Numérica    | Número de vagas de estacionamento associadas à propriedade                  |
| **Landsize**      | Numérica    | Tamanho do terreno da propriedade em metros quadrados                       |
| **BuildingArea**  | Numérica    | Área total construída da propriedade em metros quadrados                    |
| **CouncilArea**   | Categórica  | Nome da área administrativa local onde a propriedade está localizada        |



## 🧪 Variáveis Derivadas Criadas

| 🏷️ Variável           | 📊 Tipo      | 📝 Descrição                                                                 |
|------------------------|-------------|------------------------------------------------------------------------------|
| **Preço (log)**        | Numérica    | Transformação logarítmica do preço para estabilizar a variância             |
| **Faixa de Preço**     | Categórica  | Classificação do preço em categorias (Baixo, Médio, Alto, Luxo)             |
| **Erro Absoluto**      | Numérica    | Diferença absoluta entre preço real e previsto                              |
| **Erro Percentual**    | Numérica    | Diferença percentual entre preço real e previsto                            |
| **Classificação Erro** | Categórica  | Agrupamento por precisão da previsão (Preciso, Aceitável, Alto erro)        |



## 🛠️ Ferramentas Utilizadas

🐍 Python • 📊 Pandas • ➗ NumPy • 🎨 Seaborn • 📈 Matplotlib • 🤖 Scikit-learn <br>



## 📊 Principais Resultados

✅ Remoção de outliers melhorou significativamente o desempenho 

📈 Random Forest obteve R² de 0.9999 com erro mínimo 

🤝 Comitê de modelos (Voting Regressor) escolhido por robustez e estabilidade 

📊 Base final preparada para visualização em Power BI



## ⚠️ Limitações
🔍 Possível overfitting em modelos mais complexos 

📉 Dataset com valores extremos e dados faltantes 

🧠 Modelos mais avançados ainda podem ser explorados

## 🔎 Próximos Passos
🚀 Testar XGBoost e LightGBM 

📊 Criar dashboard interativo no Power BI 

📈 Aplicar o modelo em novos dados ou cenários simulados



## 🚀 Execute o Notebook no Google Colab
[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HuriAnn/mvp_riscos_financeiros/blob/main/MVP_An%C3%A1lise_Riscos_Financeiros.ipynb)
