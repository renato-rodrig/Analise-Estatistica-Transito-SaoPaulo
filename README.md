MOBIT - Teste de nível Ciência de Dados para Estágio
========================================

Visão do projeto
----------------
O teste consiste em desafios para avaliar o nível de conhecimento do candidato em logica de programação, Linguagem Python e Análise de dados.

Tecnologias:
*	Python 3;
*   Jupyter Notebook;
*	Controle de versão GIT;


Iniciando
---------
Projeto disponibilizado em: 
    
    http://pdi.mobitbrasil.com.br:8601/projects/ANP/repos/estagiario-ciencia-dados

Para realizar o teste, faça o clone do repositório em sua máquina local.  
 
    http://pdi.mobitbrasil.com.br:8601/scm/anp/estagiario-ciencia-dados.git

Também disponível para download em:

    http://pdi.mobitbrasil.com.br:8601/rest/api/latest/projects/ANP/repos/estagiario-ciencia-dados/archive?format=zip

Utilize o e-mail jobs@mobitbrasil.com.br para dúvidas e esclarecimentos.


Dicionário dos dados
-------
Descrição das colunas:
```
- passage (str) - Nome da passagem.
- direction (str) - direção da passagem.
- type (str) - Indica se a passagem é em uma via expressa.
- region (str) - A região de São Paulo.\n",
- timestamp (datetime) - Quando ocorreu o engarrafamento (UTC-4).
- jam_size (int) - Comprimento do engarrafamento em metros.
- segment (str) - Onde a passagem foi localizada.
```

Tarefas
-------
Os seguintes testes buscam avaliar o nível de conhecimento do candidato em recursos de análise de dados e linguagem Python. Caso o candidato deseje, pode-se utilizar de bibliotecas de terceiros para auxílio, desde que presentes em repositório no pypi. Adicione ao projeto o `requirements.txt` com as informações das bibliotecas utilizadas.

É de escolha do candidato a IDE ou editor de textos preferido para codificação, sugere-se utilizar o jupyter notebook.



1- Carregue o conjunto de dados em memória para realizar as análises.
```
- Carregue os dados em data/traffic_data.feather
```

2- Dados Nulos
```
- Plote o gráfico dos dados nulos referente a cada coluna.
- Em cada caso o que você faria para resolver o problema dos dados nulos?
```
4- Dados Categóricos
```
- Realize um processamento sobre os dados categóricos de forma a transformá-los em numéricos. Justifique sua resposta.
```
5- Correlação
```
- Gere um gráfico de correlação das variáveis em uso, utilize somente as variáveis que você acha interessante para o problema proposto.

```
6- Engarrafamentos
```
- Plote um gráfico da distribuição dos engarrafamentos sendo agregado por ano.
- Plote um gráfico da distribuição dos engarrafamentos sendo agregado por mês.
- Plote um gráfico da distribuição dos engarrafamentos sendo agregado por dia da semana.
- Plote um gráfico da distribuição dos engarrafamentos sendo agregado por horário do dia.
- Comente sobre os resultados obtidos, há alguma tendência?
```
7- Geolocalização
```
- A partir dos endereços propostos, utilize alguma api do python que converta o endereço e geolocalização.
- Plote círculos de engarrafamentos em um mapa de São Paulo baseado no comprimento do mesmo e a geolocalização obtida anteriormente. 
```
[EXTRA] 
```
- Configure e treine algum classificador(árvores, bayesiano, rede neural) que receba informações de entrada, seja as disponibilizadas no dataset ou geradas por outro dataset, com o intuito de informar se no determinado horário e local se haverá ou não engarrafamento.
- Gere um gráfico de correlação das variáveis em uso e crie um ranque das variáveis mais relevantes para a solução do problema proposto no item EXTRA.
```

Não se limite às análises sugeridas. Fique a vontade a realizar outros tipos de análises que não foram sugeridas.

Submetendo o código para avaliação
----------------------------------


Quando finalizado e pronto para envio, gere o(s) arquivo(s) de patch com os códigos desenvolvidos.

	git format-patch origin/master

Envie os arquivos de patch gerados por e-mail ao responsável pela aplicação do teste (jobs@mobitbrasil.com.br). Com o git configurado para envio de e-mail, pode ser feito com:

    git send-email  

Caso prefira, o candidato pode clonar este repositório e subir as soluções em sua própria conta do Bitbucket. Nesse caso, enviar o endereço do repositório com as soluções para o email (jobs@mobitbrasil.com.br). 
