# pos-ufrn
Trabalho da disciplina de Probabilidade 2018.1 (IMD/UFRN)
# Análise de dados abertos
## Autores
- [Alison Hedigliranes da Silva](https://github.com/lalodbzkin) (alison.hedigliranes@gmail.com)
- [Felipe Morais da Silva](https://github.com/jeowf) (moraisfelipe97@gmail.com)

## Contextualização

 A UFRN (Universidade Federal do Rio Grande do Norte) possui um órgão responsável pelo gerenciamento dos programas de pós-graduação, que é a [Pró-reitoria de Pós-graduação](http://www.ppg.ufrn.br/index.php) (PPG) cujo desempenha um papel fundamental na expansão e consolidação do Sistema de Pós-graduação no âmbito da Universidade, na pespectiva de contribuir com as demandas da Sociedade Norte-rio-grandense e brasileira, como um importante instrumento de qualificação acadêmica e técnica.
O ensino de pós-graduação da UFRN abrange tanto os programas *Stricto sensu* (Mestrado e Doutorado) quanto *Lato sensu* (Especialização e Residências em Saúde e outras áreas do conhecimento).

## Problemática
Os programas de *Stricto sensu* possuem pós-graduandos advindos de diversas instituições de ensino, dentre elas, a própria UFRN. Desta forma, cabem-se os seguintes questionamentos:
1. Quantos alunos de pós-graduação vieram de uma graduação anterior na UFRN?
2. Agrupando os programas de pós-graduação em áreas do saber, quais cursos mais possuem alunos ingressando em uma pós-graduação?3. É possível traçar um perfil sobre os pós-graduandos (isto é, saber se é possível identificar um aluno que, potencialmente, irá reingressar em um curso de pós-graduação)? Se sim, qual é o perfil?

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
