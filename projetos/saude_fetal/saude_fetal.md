# Classificação de Saúde Fetal

|  |  |
|------|------|
| Data | 11/2022 |
| Tipo | Individual |
| Disciplina | Mineração de Dados |
| Professor | [Wagner Meira Jr.](http://lattes.cnpq.br/9092587237114334) |
| Tecnologias | Python, Numpy, Pandas, Matplotlib, Scikit Learn, Google Colaboratory |

- [Relatório](TP3_Relatorio_Helena_Pato.pdf)
- [Notebook](https://github.com/helenapato/helenapato.github.io/blob/main/projetos/saude_fetal/tp3-classificacao.ipynb)

A mortalidade infantil é um importante indicador de saúde e qualidade de vida. Definida como a taxa de óbitos de crianças menores de cinco anos de idade a cada mil nascidas vivas, um  valor  elevado  evidencia  condições  de  vida  precárias  e  baixo  nível  de  desenvolvimento. Nesse contexto, a ONU espera que, em 2030, os países acabem com as mortes preveníveis de recém-nascidos e crianças menores de cinco anos de idade.  

Dado  que  grande  parte  dos  óbitos  ocorrem  em  situações  de  poucos  recursos,  a cardiotocografia (CTG) é um exame simples e acessível para avaliar a saúde fetal. A análise de seus resultados permite que profissionais da saúde ajam para prevenir a mortalidade infantil e materna. 

A partir de dados de 2126 exames CTG,  em  que  a  saúde  fetal  foi  categorizada  em  três  classes:  normal, suspeita e patológica, visamos criar um classificador que preveja o estado de saúde da criança. Dessa forma, contribuímos para a atuação dos profissionais de saúde e para a prevenção da mortalidade infantil.

Inicialmente, fizemos uma exploração da distribuição dos dados e outras características que nos permitiram definir procedimentos para adequá-los a um algoritmo de classificação. O desbalanceamento constatado nessa etapa gerou uma oportunidade de fazer experimentos com diferentes tipos de métodos de balanceamento e levou à conclusão de que o método mais adequado neste caso é o oversampling. 

O modelo final, apesar de ser uma simples árvore de decisão, foi capaz de atingir bons valores  de  acurácia  e  gerar  uma  matriz  de  confusão  com  poucas  classificações  errôneas.  Ele 
também foi capaz de generalizar bem para dados não vistos antes, mantendo bons resultados nos dados de teste. 

Dessa  forma,  o  modelo  está  apto  atuar  em  seu  propósito  inicial,  de  ajudar  a  prever  a condição  de  saúde  fetal.  Principalmente  devido ao  baixo  número  de  casos  de  saúde patológica sendo classificados como normal ou suspeita, dado que os falsos negativos são mais perigosos nesse cenário.


*[CTG]: Cardiotocografia