# SimpleText@CLEF-2022 Shared tasks

[Home](./) | [Call for papers](./CFP) | [Important dates](./dates) | [Tasks](./tasks) | [Tools](./tools) 
[Program](./program) | [Publications](./publications) | [Organisers](./organisers) | [Contact](./contact) | [<img src="https://github.com/simpletext-madics/2021/blob/main/clef/FR.png?raw=true" width="30">](../fr/tasks)

---

## SimpleText Shared Task Guidelines

We invite you to submit both automatic and manual runs! Manual intervention should be reported.

---

<button>[Access](./tasks)</button> | <button>[Shared task 1](./task1)</button> | <button>[Shared task 2](./task2)</button> | <button>[Shared task 3](./task3)</button>| <button>[Unshared task 4](./task4)</button>

<br>

## Access
Please register at the SimpleText@CLEF workshop in order to access the data: [https://clef2022.clef-initiative.eu/index.php](https://clef2022.clef-initiative.eu/index.php)  
After registration, you will receive an email with information on how to get access to the data.

### Result submission:
Participants should put their run results into the folder Documents created for their user.

### 2022 DataSet
For this edition we use the Citation Network Dataset: DBLP+Citation, ACM Citation network ([https://www.aminer.org/citation](https://www.aminer.org/citation)). É fornecido aos participantes um índice de pesquisa elástico acessível através de uma GUI API. Este índice é adequado para:
* aplicar métodos básicos de recuperação de passagens baseados em modelos de IR vectoriais ou linguísticos
* gerar modelos de alocação de Dirichlet Latente,
* formar Redes Neuronais Gráficas para recomendação de citação como realizado em [https://stellargraph.readthedocs.io/](https://stellargraph.readthedocs.io/) por exemplo,
* aplicar transformadores bi-direccionais profundos para expansão de consulta.
* e muito mais...

### 2022 Consultas
Para esta edição, as consultas são uma selecção de títulos de imprensa recentes de *The Guardian* enriquecidos com palavras-chave extraídas manualmente do conteúdo do artigo. Foi verificado que cada palavra-chave permite extrair pelo menos 5 resumos relevantes. A utilização destas palavras-chave é opcional.

*Formato de entrada para todas as tarefas:*
*Os tópicos estão no formato MD

<img src="https://github.com/simpletext-madics/2021/blob/main/clef/Query1.png?raw=true">

* Artigos de texto completo de *The Guardian* (link, pasta query_related_content com textos completos no formato MD)
* Índice ElasticSearch no seguinte servidor de dados (por exemplo): [https://guacamole.univ-avignon.fr/nextcloud/index.php/apps/files/?dir=/simpleText/queries&fileid=570352](https://guacamole.univ-avignon.fr/nextcloud/index.php/apps/files/?dir=/simpleText/queries&fileid=570352)
* DBLP full dump no formato JSON.GZ
* Resumos DBLP extraídos para cada tópico no seguinte formato MD (doc_id, ano, resumo):

<img src="https://github.com/simpletext-madics/2021/blob/main/clef/MDformat.png?raw=true"> 
