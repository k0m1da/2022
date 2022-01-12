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

## Tarefa 1: O que está dentro (ou fora)? Seleccione passagens a incluir num resumo simplificado, dada uma consulta.

Dado um artigo de um grande público internacional, esta tarefa visa recuperar de uma grande base de dados bibliográficos científicos com resumos, todas as passagens que seriam relevantes para ilustrar este artigo. As passagens extraídas devem ser adequadas para serem inseridas como citações simples no artigo original. O agrupamento de frases e as métricas automáticas serão utilizados para avaliar estes resultados. A relevância do documento de origem será avaliada, bem como as potenciais questões de anáfora não resolvidas.

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
