
# Avaliando modelos de _Machine Learning_ (ONGOING)

Nesta seção vamos estudar como avaliar um dado modelo de _machine learning (ML)_. Depois das definições das métricas passaremos

## Definições


|      Sigla      | Significado      |
|:--------------:|:-----------------:|
| VP  | verdadeiros positivos       |
| FN | Falsos negativos| 
|FP  | falsos positivos| 
|VN |verdadeiros negativos|
|P  | Precisão |
|S| Sensibilidade|
|N| Total de elementos|

## Matriz de confusão

É um diagrama no qual se colocam os resultados obtidos com a previsão versus os resultados reais. O interessante da matriz de confusão é que ela tem a ver com os erros tipo I e tipo II da estatística da seguinte forma (exemplo com uma matriz 2 x 2):

|            |          | Previsto                       |                                    |
|------------|:--------:|--------------------------------|------------------------------------|
|            |          |            Positivo            |              Negativo              |
| **Verdadeiro** | Positivo | VP  (acerto)                   | FN (perda de alarme, erro tipo II) |
|            | Negativo | FP (alarme falso, erro tipo I) | VN (rejeição  correta)             |

A matriz de confusão reflete de forma pictórica a qualidadeda previsão. Via de regra se deseja que os números na diagonal principal sejam significativamente maiores que os fora da diagonal. 


## Métricas de ML

As seguintes métricas são comumente usadas em ML ([link para referência](https://diegomariano.com/metricas-de-avaliacao-em-machine-learning/))

|      Nome      | Nome  (em inglês) |    Descrição    |
|:--------------:|:-----------------:|:---------------:|
| Sensibilidade  | Sensitivity       | VP / (VP+FN)    |
| Especificidade |                   | VN / (FP+VN)    |
| Acurácia       | Accuracy          | (VP+VN) / N     |
| Precisão       | Precision         | VP / (VP+FP)    |
| Placar F              | F-Score           | 2.(P.S) / (P+S) |




Vamos discutir em um pouco mais de detalhe o que significa cada uma dessas métricas. 

### Sensibilidade

### Especificidade

### Acurácia

A acurácia é definida como a razão entre os acertos e a quantidade de elementos disponíveis. Embora seja uma métrica de suma importância deve-se lembrar que ela lava a conclusões erradas sobre a qualidade da previsão quando os dados estão desbalanceados.  Para este caso é melhor usar a _acurácia balanceada (bACC)_ dada por:


$bACC = \frac{TPR+TNR}{2}$




### Precisão

Esta métrica mede o quão preciso o modelo é com respeito às quantidades que foram previstas como positivas. Ou seja é _a razão entre os verdadeiros positivos e as quantidades previstas como positivas._


### _F-Score_

## Referências

1. https://mabittar.github.io/Metricas/
2. https://diegomariano.com/metricas-de-avaliacao-em-machine-learning/
2. https://en.wikipedia.org/wiki/Precision_and_recall#Definition_(classification_context)
3. https://towardsdatascience.com/accuracy-precision-recall-or-f1-331fb37c5cb9


