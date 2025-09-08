#  IMDB Movies

<!------------------------------------------------------>
## 1 - Descrição do Projeto

O projeto desenvolvido foi um desafio proposto pela Indicium Lighthouse. O desafio, conforme a descrição da própria indicium consiste em realizar uma análise em um banco de dados cinematográfico com o objetivo de orinetar qual o tipo de filme deve ser o próximo a ser desenvolvido. 

<!------------------------------------------------------>
## 2 - Entregas

As  entregas exigidas para este projeto são:
1.	Faça uma análise exploratória dos dados (EDA), demonstrando as principais características entre as variáveis e apresentando algumas hipóteses relacionadas. Seja criativo!
2.	Responda também às seguintes perguntas:
  - a.	Qual filme você recomendaria para uma pessoa que você não conhece?
  - b.	Quais são os principais fatores que estão relacionados com alta expectativa de faturamento de um filme? 
  - c.	Quais insights podem ser tirados com a coluna Overview? É possível inferir o gênero do filme a partir dessa coluna?
3.	Explique como você faria a previsão da nota do imdb a partir dos dados. Quais variáveis e/ou suas transformações você utilizou e por quê? Qual tipo de problema estamos resolvendo (regressão, classificação)? Qual modelo melhor se aproxima dos dados e quais seus prós e contras? Qual medida de performance do modelo foi escolhida e por quê?
4.	Supondo um filme com as seguintes características:
```python
   {'Series_Title': 'The Shawshank Redemption',
  	'Released_Year': '1994',
  	'Certificate': 'A',
  	'Runtime': '142 min',
  	'Genre': 'Drama',
  	'Overview': 'Two imprisoned men bond over a number of years, finding solace and eventual redemption through acts of common decency.',
  	'Meta_score': 80.0,
  	'Director': 'Frank Darabont',
  	 'Star1': 'Tim Robbins',
  	'Star2': 'Morgan Freeman',
  	'Star3': 'Bob Gunton',
  	'Star4': 'William Sadler',
  	'No_of_Votes': 2343110,
  	'Gross': '28,341,469'}
```
   Qual seria a nota do IMDB?

6.	Salve o modelo desenvolvido no formato .pkl. 



<!------------------------------------------------------>
## 3 - Descrição da Database

A base de dados de treinamento contém 15 colunas. A descrição das colunas é:

- `Series_Title`: Nome do filme
- `Released_Year`: Ano de lançamento
- `Certificate`: Classificação etária
- `Runtime`: Tempo de duração
- `Genre`: Gênero
- `IMDB_Rating `: Nota do IMDB
- `Overview`: Overview do filme
- `Meta_score`: Média ponderada de todas as críticas 
- `Director`: Diretor
- `Star1`: Ator/atriz #1
- `Star2`: Ator/atriz #2
- `Star3`: Ator/atriz #3
- `Star4`: Ator/atriz #4
- `No_of_Votes`: Número de votos
- `Gross`: Faturamento


<!------------------------------------------------------>
## 4 - Pipeline de Solução

O seguinte pipeline foi utilizado, com base no framework CRISP-DM:

1. EDA
  - Definir o problema de negócio.
  - Coletar os dados e obter uma visão geral dos mesmos.
  - Explorar os dados (análise exploratória de dados)
  - Limpeza e pré-processamento de dados.
2. Modelagem
  - Comparação
    - Dividir os dados em conjuntos de treinamento e teste.
    - Comparar Modelos
  - Ajuste Fino (Fine Tunning)
    - Seleção e Ajuste de Recursos.
    - Exportar o modelo.
  - Testar
    - Teste e avaliação do modelo de produção final.
    - Concluir e interpretar os resultados do modelo.
    - Deploy.


<!------------------------------------------------------>
## 5 - Tecnologias e Ferramentas
Este projeto foi desenvolvido utilizando um conjunto de ferramentas e bibliotecas amplamente utilizadas em ciência de dados e aprendizado de máquina:

📊 Bibliotecas para Análise de Dados
- Pandas – Manipulação e análise de dados tabulares.

- NumPy – Operações matemáticas e manipulação de matrizes.

- Matplotlib and Seaborn – Criação de gráficos e visualizações exploratórias.

🤖 Machine Learning
- Scikit-learn (sklearn) – Estrutura principal para aprendizado de máquina, usada para:

   - Modelos: DummyClassifier, LogisticRegression, KNeighborsClassifier, DecisionTreeClassifier.

   - Cross-validation: KFold, cross_validate.

   - Otimização de hiperparâmetros: GridSearchCV.

- XGBoost (XGBClassifier) ​​– Algoritmo baseado em árvore focado em desempenho.

- LightGBM (LGBMClassifier) ​​– Algoritmo de aumento rápido e eficiente para grandes volumes de dados.

🧪 Ambiente de Desenvolvimento
- Jupyter Notebook – Ambiente interativo para visualização de desenvolvimento, testes e análise.

- Anaconda – Gerenciador de pacotes e ambientes, usado para organizar o ambiente de desenvolvimento.

🌐 Controle de versão
- GitHub – Plataforma para controle de versão, hospedagem e documentação de projetos.

<!------------------------------------------------------>
## 6 - Principais Insights do EDA


<!------------------------------------------------------>
## 7 - Principais Insights da Modelagem


<!------------------------------------------------------>
## 8 - Execute este projeto em sua máquina local


<!------------------------------------------------------>
## 9 - Próximos Passos
