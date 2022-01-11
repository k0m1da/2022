# SimpleText@CLEF-2022 Tasks


[Home](./) | [Call for papers](./CFP) | [Important dates](./dates) | [Tasks](./tasks) | [Tools](./tools) 
[Program](./program) | [Publications](./publications) | [Organisers](./organisers) | [Contact](./contact) | [<img src="https://github.com/simpletext-madics/2021/blob/main/clef/FR.png?raw=true" width="30">](../fr/task1)


---

## SimpleText Task Guidelines

We invite you to submit both automatic and manual runs! Manual intervention should be reported.

---

<button>[Access](./tasks)</button> | <button>[Shared task 1](./task1)</button> | <button>[Shared task 2](./task2)</button> | <button>[Shared task 3](./task3)</button>| <button>[Unshared task 4](./task4)</button>

<br>

## Task 1:  What is in (or out)? Select passages to include in a simplified summary, given a query.

Given an article from a major international newspaper general audience, this task aims at retrieving from a large scientific bibliographic database with abstracts, all passages that would be relevant to illustrate this article. Extracted passages should be adequate to be inserted as plain citations in the original paper. Sentence pooling and automatic metrics will be used to evaluate these results. The relevance of the source document will be evaluated as well as potential unresolved anaphora issues.

*Formato de saída:*  
 
Um máximo de 1000 passagens a serem incluídas num resumo simplificado num ficheiro TSV (Tab-Separated Values) com os seguintes campos:
*run_id*: Run ID começando com team_id_id_
*manual*: Se a execução é manual {0,1}
*topic_id*: ID do Tópico
*doc_id*: ID do documento de origem
*passage*: Texto da passagem seleccionada
*Marcação*: Rank de passagem

*run_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; manual &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; topic_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; doc_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; passagem &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; classificação*

### Avaliação  
O agrupamento de sentenças e a métrica automática serão utilizados para avaliar estes resultados. A relevância do documento de origem será avaliada, bem como as potenciais questões de anáfora não resolvidas.

Exemplo de SAÍDA:

| run_id | manual | topic_id | doc_id | passage | rank |
|:-------|:-------|:---------|:-------|:--------|:-----|
| ST1_1 | 1 | 1 | 3000234933 | As pessoas estão a ficar cada vez mais confortáveis a usar Assistentes Digitais (DAs) para interagir com serviços ou objectos ligados. | 1 |
| ST1_1 | 1 | 1 | 3003409254 | grandes algoritmos de aprendizagem de dados e máquinas (ML) podem resultar em decisões discriminatórias contra certos grupos protegidos definidos sobre dados pessoais como género, raça, orientação sexual, etc. | 2 |
| ST1_1 | 1 | 1 | 3003409254 | Tais algoritmos concebidos para descobrir padrões em grandes dados podem não só detectar quaisquer vieses sociais codificados nos dados de formação, mas ainda pior, podem reforçar tais vieses resultando numa discriminação mais severa. | 3 |  
