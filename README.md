
## tratamento de dados para demandas das equipes de Machine Learnig e Desenvolvimento

Trabalhando com um base de dados de imoveis para locação foi trabalhando a base identificando as necessidade das equipes em suas demandas, inicialmente para a equipe de Machine Learning foi feito desde a analise exploratória identificando que dentro das dados
o mais relevante para trabalho de locação de imoveis residencias são imoveis de tipo apartamento, conforme gráfico 

![image](https://github.com/reaugusto/Dados_imobiliaria_Alura/assets/40721866/7fa71eb8-1755-458f-ba2b-e6e44b072898)

Após a analise foi mantido noa base para essa equipe apenas imoveis do tipo apartamente e dentro desses dados iniciado o tratamento, que consistiu em algumas etapas:

. Tratamento de **Nilos** (altando dados nulos para '0')
. Remoção de registros que não possuem informações de Aluguel ou Condominio
. Filtros para dados especificos
  *Apartamentos com 1 Quarto e aluguel menos que R$ 1200
  *Apartamentos com mais de 2 Quatos, aluguel menor que R$3000 e Area mair que 70m
. Criados as 3 bases para uso nos modelos, Base limpa dos apartamentos e as dos dois filtros

Para a demanda da equipe de desenvoldores, foi utilizado a Base original e criado algumas colunas númericas e colunas categoricas para uso no site:

. Coluna de **valor por mMês** criada com a soma dos valores de aluguel e condominio
. Coluna de **Valor por Ano** crirada com a multiplicação dos valores mensais pelos 12 meses + o valor do IPTU
. Coluna de **Discrição** criada com informações do proprio imóvel
. Coluna **Possui Suite** baseada na culuna de Suite que mostra quantidade preenchendo com sim ou não

Criado todos os arquivo para as duas equipes trabalharem seguindo o padrão da base de dados de origem.

[Projeto no Colab] (https://colab.research.google.com/drive/10--CP7l2JntDwdGkY3oqm2NOvjL78-k9?usp=sharing)
