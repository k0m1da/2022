# SimpleText@CLEF-2022 Tasks

[Home](./) | [Call for papers](./CFP) | [Important dates](./dates) | [Tasks](./tasks) | [Tools](./tools) 
[Program](./program) | [Publications](./publications) | [Organisers](./organisers) | [Contact](./contact) | [<img src="https://github.com/simpletext-madics/2021/blob/main/clef/FR.png?raw=true" width="30">](../fr/task3)


---

## SimpleText Task Guidelines

We invite you to submit both automatic and manual runs! Manual intervention should be reported.

---

<button>[Access](./tasks)</button> | <button>[Shared task 1](./task1)</button> | <button>[Shared task 2](./task2)</button> | <button>[Shared task 3](./task3)</button>| <button>[Unshared task 4](./task4)</button>

<br>

## Task 3: Rewrite this! Given a query, simplify passages from scientific abstracts. 

The goal of this task is to provide a simplified version of text passages. Participants will be provided with queries and abstracts of scientific papers. The abstracts can be split into sentences as in the exemple [https://guacamole.univ-avignon.fr/nextcloud/index.php/s/SQTdS2Yowf9dxNa](https://guacamole.univ-avignon.fr/nextcloud/index.php/s/SQTdS2Yowf9dxNa). The simplified passages will be evaluated manually with eventual use of aggregating metrics.

*Output format:*  

Passagens simplificadas num ficheiro tabelado TSV com os seguintes campos:
*run_id*: Run ID começando com team_id_
*manual*: Se a execução é manual {0,1}
*topic_id*: ID do Tópico 
*texto_tópico*: Texto do tópico
*passagem_de_fonte*: Texto da passagem de origem 
*passage_simplified_passage*: Texto da passagem simplificada 

run_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; manual &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; topic_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; topic_text &nbsp; &nbsp;&nbsp;&nbsp;&nbsp; doc_id &nbsp;&nbsp;&nbsp;&nbsp; passagem_fonte &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; passagem_ simplificada

### Avaliação
As passagens simplificadas serão avaliadas manualmente com eventual utilização de métricas de agregação.

Exemplo de SAÍDA:

| run_id | manual | topic_id | topic_text | doc_id | source_passage | simplified_passage |
|:-------|:-------|:---------|:-----------|:-------|:---------------|:-------------------|
| BTU | 1 | 1 | Assistentes digitais como o Siri e Alexa entrincheiram preconceitos de género, diz ONU | 3003409254 | A tomada de decisão automatizada baseada em grandes dados e algoritmos de aprendizagem de máquinas (ML) pode resultar em decisões discriminatórias contra certos grupos protegidos definidos sobre dados pessoais como género, raça, orientação sexual, etc. Tais algoritmos concebidos para descobrir padrões em grandes dados podem não só detectar quaisquer preconceitos sociais codificados nos dados de formação, mas, pior ainda, podem reforçar tais preconceitos resultando numa discriminação mais severa. | A tomada de decisão automatizada pode incluir preconceitos sexistas e racistas e até reforçá-los porque os seus algoritmos se baseiam na representação social mais proeminente no conjunto de dados que utilizam. | 
