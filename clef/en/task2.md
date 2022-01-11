# SimpleText@CLEF-2022 Tasks

[Home](./) | [Call for papers](./CFP) | [Important dates](./dates) | [Tasks](./tasks) | [Tools](./tools) 
[Program](./program) | [Publications](./publications) | [Organisers](./organisers) | [Contact](./contact) | [<img src="https://github.com/simpletext-madics/2021/blob/main/clef/FR.png?raw=true" width="30">](../fr/task2)


---

## SimpleText Task Guidelines

We invite you to submit both automatic and manual runs! Manual intervention should be reported.

---

<button>[Access](./tasks)</button> | <button>[Shared task 1](./task1)</button> | <button>[Shared task 2](./task2)</button> | <button>[Shared task 3](./task3)</button>| <button>[Unshared task 4](./task4)</button>

<br>

## Task 2: What is unclear? Given a passage and a query, rank terms/concepts that are required to be explained for understanding this passage (definitions, context, applications,..).

The goal of this task is to decide which terms (up to 10) require explanation and contextualization to help a reader to understand a complex scientific text – for example, with regard to a query, terms that need to be contextualized (with a definition, example and/or use-case). Term pooling and automatic metrics (NDCG,...) will be used to evaluate these results.

*Output format:*  

List of terms to be contextualized in a tabulated file TSV with the following fields:
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
