# SimpleText@CLEF-2022 Tarefas


[Início](./) | [Chamada para papéis](./CFP) | [Datas importantes](./dates) | [Tarefas](./tasks) | [Ferramentas](./tools)

[Programa](./program) | [Publicações](./publications) | [Organizadores](./organisers) | [Portefólio](./portefolio) 
[<img src="https://github.com/simpletext-madics/2021/blob/main/clef/FR.png?raw=true" width="30">](../fr/CFP) [<img src="https://upload.wikimedia.org/wikipedia/commons/f/f2/Flag_of_Great_Britain_%281707–1800%29.svg?raw=true" width="30">](../en/CFP)  [<img src="https://icons.iconarchive.com/icons/wikipedia/flags/128/PT-Portugal-Flag-icon.png?raw=true" width="30">](../pt/CFP)


---

## Linhas de Guia da Tareda SimpleText 

Convidamo-lo a submeter tanto as execuções automáticas como manuais! A intervenção manual deve ser comunicada.

---

<button>[Aceder](./tasks)</button> | <button>[Tarefa partilhada 1](./task1)</button> | <button>[Tarefa partilhada 2](./task2)</button> | <button>[Tarefa partilhada 3](./task3)</button>| <button>[Tarefa não partilhada 4](./task4)</button>

<br>

## Acesso
Por favor, registar-se no workshop SimpleText@CLEF a fim de aceder aos dados: [https://clef2022.clef-initiative.eu/index.php](https://clef2022.clef-initiative.eu/index.php)  
Após o registo, receberá um e-mail com informações sobre como obter acesso aos dados.

### Apresentação de resultados:
Os participantes devem colocar os seus resultados de execução na pasta Documentos criados para o seu utilizador.

### 2022 DataSet
Para esta edição utilizamos o Citation Network Dataset: DBLP+Citation, ACM Citation network ([https://www.aminer.org/citation](https://www.aminer.org/citation)). É fornecido aos participantes um índice de pesquisa elástico acessível através de uma GUI API. Este índice é adequado para:
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
