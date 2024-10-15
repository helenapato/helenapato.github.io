## Banco de Dados de Licitações

|  |  |
|------|------|
| Data | 10/2020 |
| Colaboração | Grupo |
| Disciplina | Introdução a Bancos de Dados |
| Professor | [Rodrygo Luis Teodoro Santos](http://lattes.cnpq.br/1162362624079364) |
| Tecnologias | Python, Jupyter Notebook, SQLite, Numpy, Pandas |

- [Notebook](https://github.com/helenapato/helenapato.github.io/blob/main/projetos/licitacoes/TP2_IBD_Notebook.ipynb)
- [Video](https://www.youtube.com/watch?v=Kt4Wm4tGM44&feature=youtu.be)

O objetivo deste trabalho foi projetar e implementar um banco de dados relacional para análise de dados abertos governamentais. Seguimos um processo bottom-up, iniciado a partir da análise de um conjunto de dados de Licitações, referentes ao mês de janeiro de 2020, extraídos do Data Warehouse do Sistema Integrado de Administração de Serviços Gerais (DW-SIASG) e publicados no Portal da Transparência do Governo Federal.

Originalmente, os dados estavam distribuídos em três tabelas, cujo esquema relacional não estava normalizado, portanto foi necessário fazê-lo a fim de mapeá-lo para o esquema Entidade-Relacionamento correspondente. O resultado possui sete tabelas. Usando a biblioteca SQLite, criamos o banco de dados em seu formato original, além das tabelas vazias correspondentes ao nosso esquema, e então as preenchemos usando consultas de seleção a partir do banco original. 

Por fim, realizamos diversas consultas SQL, envolvendo operações de seleção, projeção, junção de duas ou mais relações e funções de agregação. Por exemplo, identificamos que o órgão superior encarregado do maior número de unidades gestoras é o Ministério da Educação, cujas licitações têm um custo médio de R$ 414.592,09 .