# Análise dos pós-graduandos regressos da UFRN com base nos dados abertos da UFRN

Trabalho da disciplina de Probabilidade 2018.1 (IMD/UFRN)

## Link do vídeo

https://www.youtube.com/watch?v=9Tf0Q94IiBU

## Autores

- [Alison Hedigliranes da Silva](https://github.com/lalodbzkin) (alison.hedigliranes@gmail.com)
- [Felipe Morais da Silva](https://github.com/jeowf) (moraisfelipe97@gmail.com)

## Contextualização

A UFRN (Universidade Federal do Rio Grande do Norte) possui um órgão responsável pelo gerenciamento dos programas de pós-graduação, que é a [Pró-reitoria de Pós-graduação](http://www.ppg.ufrn.br/index.php) (PPG) cujo desempenha um papel fundamental na expansão e consolidação do Sistema de Pós-graduação no âmbito da Universidade, na pespectiva de contribuir com as demandas da Sociedade Norte-rio-grandense e brasileira, como um importante instrumento de qualificação acadêmica e técnica.

O ensino de pós-graduação da UFRN abrange tanto os programas *Stricto sensu* (Mestrado e Doutorado) quanto *Lato sensu* (Especialização e Residências em Saúde e outras áreas do conhecimento).

## Problemática

Os programas de *Stricto sensu* possuem pós-graduandos advindos de diversas instituições de ensino, dentre elas, a própria UFRN. Desta forma, cabem-se os seguintes questionamentos:

1. Quantos alunos de pós-graduação vieram de uma graduação anterior na UFRN?
2. Agrupando os programas de pós-graduação em áreas do saber, quais cursos mais possuem alunos ingressando em uma pós-graduação?
3. É possível traçar um perfil sobre os pós-graduandos (isto é, saber se é possível identificar um aluno que, potencialmente, irá reingressar em um curso de pós-graduação)? Se sim, qual é o perfil?

## Materiais

Para tentar responder as perguntas levantas anteriormente, nós utilizamos os [dados abertos da UFRN](http://dados.ufrn.br/group/ensino).

Dentre todos os dados que dispomos, escolhemos os necessários:

- Tabela de alunos ingressantes entre 2009 e 2016;
- Tabela com alunos em bolsas de iniciação científica;
- Tabela referente às estruturas curriculares.

Ainda, para desenvolver a análise proposta com base em todos esses dados, utilizamos o [Jupyter](http://jupyter.org/install) em conjunto com as bibliotecas:

- Pandas;
- Matplotlib;
- Seaborn;
- Numpy.

## Metodologia

Utilizando os dados citados, foram realizados os seguintes processos:

- Carregar os dados em um DataFrame (estrutura de dados do pandas para armazenar tabelas);
- Separar os discentes por nível de ensino (graduação, mestrado e doutorado);
- Descobrir a quantidade média de semestres necessárias que um graduando precisa para se formar e, em seguida, filtrar os alunos de pós-graduação com base nesse dado;
- Descobrir os pós-graduandos que fizeram alguma graduação na UFRN com base na interseção das tabelas graduando X pós-graduando (levando em consideração o nome);
- Descobrir os cursos de graduação que mais possuem regressos em uma pós-graduação verificando nas tabelas de pós-graduação (dos pós-graduandos na UFRN) de quais cursos de graduação vieram aqueles alunos;
- Descobrir alguma correlação entre a tabela de bolsistas de iniciação científica e pós-graduandos;
- Gerar gráficos pertinentes à discussão;
- Discutir resultados.

## Considerações finais

Neste trabalho buscamos responder a algumas perguntas levantas relativas aos cursos de mestrado e doutorado oferecidos pela UFRN. Assim, como conclusões gerais, temos que:

1. A grande maioria dos pós-graduandos vieram de instituições distintas da UFRN;
2. Os cursos da área de Ciências Humanas, Letras e Artes possuem um caráter mais acadêmico dentre os demais (tendo em vista que possuem alunos com maior ingresso no mestrado e doutorado) e, Ciências Exatas e da Terra possui a maior quantidade de alunos que ingressam no doutorado;
3. Dentre os cursos de tecnologia, temos que Ciência e Tecnologia é o que possui maior quantidade de alunos que ingressam tanto no mestrado quanto no doutorado, tendo em vista que se trata do curso com maior ingresso de alunos;
4. Não foi possível traçar um perfil de um possível regresso com os dados disponíveis.
Em conclusão, o trabalho trouxe resultados alguns resultados inesperados por nós, porém interessantes (como o fato da UFRN possuir poucos regressos). Isso mostra a importância do método científico e que os dados abertos são úteis para responder diversas outras perguntas como as levantadas na discussão.

## Trabalhos futuros

Como adições à análise feita, novas perguntas surgem:

E quanto aos alunos da UFRN que ingressaram em uma pós-graduação em outras universidades?
A quantidade de pós-graduandos (oriundos de uma graduação na UFRN) que ingressaram em cursos de pós-graduação na UFRN é maior que a quantidade de ingressantes em programas de outras universidades? Se sim, porque isso ocorre?