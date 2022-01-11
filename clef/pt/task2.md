# SimpleText@CLEF-2022 Tarefas


[Início](./) | [Chamada para papéis](./CFP) | [Datas importantes](./dates) | [Tarefas](./tasks) | [Ferramentas](./tools) 
[Programa](./program) | [Publicações](./publications) | [Organisadores](./organisers) | [Contactos](./contact) | [<img src="https://github.com/simpletext-madics/2021/blob/main/clef/FR.png?raw=true" width="30">](../fr/task1)


---

## Linhas de Guia da Tareda SimpleText 

Convidamo-lo a submeter tanto as execuções automáticas como manuais! A intervenção manual deve ser comunicada.

---

<button>[Aceder](./tasks)</button> | <button>[Tarefa partilhada 1](./task1)</button> | <button>[Tarefa partilhada 2](./task2)</button> | <button>[Tarefa partilhada 3](./task3)</button>| <button>[Tarefa não partilhada 4](./task4)</button>

<br>

## Tarefa 2: O que é que não está claro? Dada uma passagem e uma pergunta, os termos/conceitos de classificação que é necessário explicar para compreender esta passagem (definições, contexto, aplicações,...).

O objectivo desta tarefa é decidir que termos (até 10) requerem explicação e contextualização para ajudar o leitor a compreender um texto científico complexo - por exemplo, em relação a uma consulta, termos que precisam de ser contextualizados (com uma definição, exemplo e/ou caso de uso). O agrupamento de termos e a métrica automática (NDCG,...) serão utilizados para avaliar estes resultados.

*Formato de saída:*  

Lista de termos a serem contextualizados num ficheiro tabelado TSV com os seguintes campos:
*run_id*: Run ID começando com team_id_id_
*manual*: Se a execução é manual {0,1}
*topic_id*: ID do Tópico
*passage_text*: Texto da passagem
*term*: Termo ou outra frase a ser explicada
*Marcação*: Importância da explicação de um determinado termo

Run_id &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; manual &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; topic_id &nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; passage_text &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; termo &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; classificação

### Avaliação
Os termos "pooling" e métricas automáticas (NDCG,...) serão utilizados para avaliar estes resultados.

Exemplo de SAÍDA:

| run_id | manual | topic_id | passage_text | termo | rank |
|:-------|:-------|:---------|:-------------|:-----|:-----|
| ST_1 | 1 | 1 | A tomada de decisão automatizada baseada em grandes dados e algoritmos de aprendizagem de máquinas (ML) pode resultar em decisões discriminatórias contra certos grupos protegidos definidos sobre dados pessoais como género, raça, orientação sexual, etc. Tais algoritmos concebidos para descobrir padrões em grandes dados podem não só detectar quaisquer preconceitos sociais codificados nos dados de formação, mas, pior ainda, podem reforçar tais preconceitos resultando numa discriminação mais severa. A maioria das abordagens de aprendizagem de máquinas com consciência de justiça propostas até agora concentram-se exclusivamente nas etapas de pré, em ou pós-processamento do processo de aprendizagem de máquinas, ou seja, dados de entrada, algoritmos de aprendizagem ou modelos derivados, respectivamente. No entanto, o problema da equidade não pode ser isolado a uma única etapa do processo ML. Pelo contrário, a discriminação é frequentemente o resultado de interacções complexas entre grandes dados e algoritmos e, por conseguinte, é necessária uma abordagem mais holística. O quadro proposto FAE (Fairness-Aware Ensemble) combina intervenções relacionadas com a equidade tanto nas fases de pré como de pós-processamento do processo de análise de dados. Na etapa de pré-processamento, abordamos os problemas de sub-representação do grupo protegido (desequilíbrio de grupo) e de equilíbrio de classe através da geração de amostras de formação equilibradas. Na etapa de pós-processamento, abordamos o problema da sobreposição de classes, deslocando o limite de decisão no sentido da equidade.| aprendizagem de máquinas | 1 |
| ST_1 | 1 | 1 | A tomada de decisão automatizada baseada em grandes dados e algoritmos de aprendizagem de máquinas (ML) pode resultar em decisões discriminatórias contra certos grupos protegidos definidos sobre dados pessoais como género, raça, orientação sexual, etc. Tais algoritmos concebidos para descobrir padrões em grandes dados podem não só detectar quaisquer preconceitos sociais codificados nos dados de formação, mas, pior ainda, podem reforçar tais preconceitos resultando numa discriminação mais severa. A maioria das abordagens de aprendizagem de máquinas com consciência de justiça propostas até agora concentram-se exclusivamente nas etapas de pré, em ou pós-processamento do processo de aprendizagem de máquinas, ou seja, dados de entrada, algoritmos de aprendizagem ou modelos derivados, respectivamente. No entanto, o problema da equidade não pode ser isolado a uma única etapa do processo ML. Pelo contrário, a discriminação é frequentemente o resultado de interacções complexas entre grandes dados e algoritmos e, por conseguinte, é necessária uma abordagem mais holística. O quadro proposto FAE (Fairness-Aware Ensemble) combina intervenções relacionadas com a equidade tanto nas fases de pré como de pós-processamento do processo de análise de dados. Na etapa de pré-processamento, abordamos os problemas de sub-representação do grupo protegido (desequilíbrio de grupo) e de equilíbrio de classe através da geração de amostras de formação equilibradas. Na etapa de pós-processamento, abordamos o problema da sobreposição de classes, deslocando o limite de decisão no sentido da equidade.| enviesamentos societais | 2 | 
| ST_1 | 1 | 1 | A tomada de decisão automatizada baseada em grandes dados e algoritmos de aprendizagem de máquinas (ML) pode resultar em decisões discriminatórias contra certos grupos protegidos definidos sobre dados pessoais como género, raça, orientação sexual, etc. Tais algoritmos concebidos para descobrir padrões em grandes dados podem não só detectar quaisquer preconceitos sociais codificados nos dados de formação, mas, pior ainda, podem reforçar tais preconceitos resultando numa discriminação mais severa. A maioria das abordagens de aprendizagem de máquinas com consciência de justiça propostas até agora concentram-se exclusivamente nas etapas de pré, em ou pós-processamento do processo de aprendizagem de máquinas, ou seja, dados de entrada, algoritmos de aprendizagem ou modelos derivados, respectivamente. No entanto, o problema da equidade não pode ser isolado a uma única etapa do processo ML. Pelo contrário, a discriminação é frequentemente o resultado de interacções complexas entre grandes dados e algoritmos e, por conseguinte, é necessária uma abordagem mais holística. O quadro proposto FAE (Fairness-Aware Ensemble) combina intervenções relacionadas com a equidade tanto nas fases de pré como de pós-processamento do processo de análise de dados. Na etapa de pré-processamento, abordamos os problemas de sub-representação do grupo protegido (desequilíbrio de grupo) e de equilíbrio de classe através da geração de amostras de formação equilibradas. Na etapa de pós-processamento, abordamos o problema da sobreposição de classes, deslocando o limite de decisão no sentido da equidade. | ML | 3 |  
