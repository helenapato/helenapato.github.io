# Videogames - Qualidade versus Popularidade

|-------------|-------------------------------------------------------------------------------|
| Data        | 06/2019                                                                       |
| Colaboração | Dupla                                                                         |
| Disciplina  | Introdução a Ciência de Dados, UFMG                                           |
| Professor   | [Flávio Vinícius Diniz de Figueiredo](http://lattes.cnpq.br/9481210393304645) |
| Tecnologias | Python, Jupyter Notebook, Matplotlib, Numpy, Scikit Learn, Pandas             |

- [Notebook](https://github.com/helenapato/ProjetoFinal_ICD_201901/blob/master/NotebookProjetoFinalVideoGames.ipynb)
- [Video](https://www.youtube.com/watch?v=8a3kgH6a2Ms&feature=youtu.be)

O embate entre a popularidade e a qualidade de um produto midiático interessa aqueles que o consomem. É sempre bom ouvir que seu filme favorito é bom, enquanto uma nota baixa da crítica deixa os fãs contrariados. Porém, muitos trabalhos independem da opinião de um especialista para ganharem o coração do público. Os Video Games não são uma exceção. Enquanto jogos avaliados como obras primas por críticos costumam fazer sucesso, existem também os que são considerados medíocres e mesmo assim vendem milhões pelo mundo.

Outro aspecto que influencia no êxito comercial de um Video Game é seu gênero. Os jogos violentos normalmente são o centro das atenções, mas existem vários outros que fazem sucesso no mercado. O que nos leva a uma reflexão em relação ao público consumidor de um determinado gênero de entretenimento, já que tudo isso influencia na formação do jogador.

Para analisar essas relações, utilizamos uma base de dados sobre Video Games que venderam pelo menos 10.000 cópias, entre 1980 e 2016, gerada a partir do site VGChartz. A caracterização inicial dos dados evidenciou que o número de avaliações de críticos é menos da metade do número de jogos, ou seja, a maioria dos jogos não tinham avaliação no site Metacritic. Além disso, observamos que os jogos de ação são os mais contemplados pelo conjunto de dados.

Para relacionar a avaliação dos críticos às vendas globais, usamos um modelo de regressão linear simples. O teste de hipótese por permutação indicou que a pontuação de um jogo tem, sim, uma relação direta com seu sucesso comercial, mas ela não é absoluta. Ao olharmos para os jogos que tem uma classificação ruim, constatamos que eles vendem pouco. Porém, também existem vários jogos bem classificados que não foram muito consumidos. Assim, nossa função de regressão ficou com uma inclinação um pouco diferente da realmente representada pelos pontos, e as métricas usadas para avaliá-la não foram muito boas.

Já para medir como o gênero influencia nas vendas ao redor do mundo, utilizamos um classificador kNN, que tenta prever a qual gênero (classe) pertence o jogo, de acordo com suas vendas em cada região geográfica. A primeira tentativa gerou métricas bem ruins e, ao desenhar uma matriz de confusão, percebemos que muitos jogos de outros gêneros estavam sendo classificados como de ação. 

Para contornarmos esse problema, fizemos uma amostragem menor dos jogos e retreinamos o modelo, gerando resultados bem melhores. Como exemplo, contrastamos a popularidade de jogos de ação na América do Norte, com a de jogos de RPG no Japão. Usando outro teste de hipótese, concluímos que esses dois aspectos são sim, bastante correlacionados e serviram bem para a classificação realizada.
