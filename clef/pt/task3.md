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

## Tarefa 3: Reescrever isto! Dada uma consulta, simplificar passagens de resumos científicos. 

O objectivo desta tarefa é fornecer uma versão simplificada de passagens de texto. Serão fornecidas aos participantes consultas e resumos de artigos científicos. Os resumos podem ser divididos em frases, como no exemplo [https://guacamole.univ-avignon.fr/nextcloud/index.php/s/SQTdS2Yowf9dxNa](https://guacamole.univ-avignon.fr/nextcloud/index.php/s/SQTdS2Yowf9dxNa). As passagens simplificadas serão avaliadas manualmente com eventual utilização de métricas de agregação.

*Formato de saída:* 

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
