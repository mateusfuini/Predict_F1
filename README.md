# Predição do Campeonato de Fórmula 1

## Especialização em Ciência de Dados
#### Projeto Interdisciplinar - 2o. Semestre

Grupo:
- Mateus Guilherme Fuini
- Michelle Melo Cavalcante

# Objetivo de Negócio

Atualmente todas as equipes da Fórumal 1 (F1) utilizam de técnicas de Machine Learning em suas corridas. A própria empresa organizadora do campeonato usa dados recebidos dos carros e sensores na pista para interagir com os telespectadores. Segundo a AWS (https://aws.amazon.com/pt/f1/), cada carro possui cerca 300 sensores que geram cerca 1,1 milhão de pontos de dados por segundo, chegando a gerar mais 3Gb a cada volta por carro. Somando com os dados de outros setores da equipe, o volume de dados ultrapassa 40Tb a cada etapa do campeonato. Além de entretetimento, todos esses dados podem ser utilizados pelas equipes no planejamento e implementação de melhores estratégias de corrida, na busca de melhorar a performance dos pilotos e provocar transformações positivas no esporte. Com tantos insights, a ciência de dados tem se tornado uma das principais ferramentas da F1.

## Contexto
Ao obter dados históricos e usá-los para ensinar algoritmos de machine learning complexos, a F1 pode prever os resultados da estratégia de corrida com maior precisão para equipes, carros e pilotos. Esses modelos são então capazes de prever cenários futuros usando dados históricos conforme as corridas se desdobram para oferecer uma experiência rica e envolvente aos fãs. Este trabalho irá utilizar tais dados históricos dos campeonatos de F1 e tentar entender o que torna um piloto campeão da F1.

## Objetivo
Através dos dados históricos de diferentes campeonatos de fórmula 1, criar um modelo de aprendizado de máquina que estime quem seria os pilotos com maiores pontuação e ganhadores na F1.

# Organização do repositório

Neste repositório contém o arquivo notebook *ML_Formula1_IFSP.ipynb* com a solução que foi executada no AWS Sagemaker, as pastas *datasets* e *models*, a primeira contém a base de dados e conjuntos de dados auxiliares gerados no notebook e a outra pasta contém o deploy do melhor modelo utilizado na solução e os dicionários gerados a partir do banco de dados que auxiliam na predição.

* Técnicas e Ferramentas utilizadas:
- API Ergast como fonte de dados
- Web scraping da wikipedia
- Lambda para obter dados da API Ergast
- Bucket S3 para armazenar dados raw e armazenar features mais importantes (Feature Store)
- Sagemaker notebook como ambiente jupyter lab (incluindo ferramentas como Data Wrangler para abstrair boto3)
- Sagemaker Canvas como experimento NO-CODE
- Framework Well-Architected machine learning da AWS 
(https://docs.aws.amazon.com/wellarchitected/latest/machine-learning-lens/well-architected-machine-learning.html)
