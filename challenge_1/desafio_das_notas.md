# Desafio das notas

João e Maria criaram um desafio de notas. Um sistema irá comparar e classificar cada nota obtida na disciplina de matemática.

A classificação de notas de Maria é m = (m[0], m[1], m[2], m[3]), e a classificação de notas de João é j = (j[0], j[1], j[2], j[3]).

O desafio é encontrar seus pontos de comparação comparando m[0] com j[0], m[1] com j[1], m[2] com j[2] e m[3] com j[3].


Se ***m[i] > j[i]*** , então Maria recebe 1 ponto.

Se ***m[i] < j[i]*** , João recebe 1 ponto.

Se ***m[i] = j[i]*** , nenhuma das pessoas recebe um ponto.


Os pontos de comparação são o total de pontos que uma pessoa ganhou.

Dados ***m*** e ***j*** , determine seus respectivos pontos de comparação.


Exemplo

m = [7, 6, 9, 8]

j = [10, 6, 7, 8]


Para os elementos *0*, João recebe um ponto porque m[0] < j[0].

Para os elementos iguais m[1] e j[1] , nenhum ponto é ganho.

Para os elementos *2* , m[2] > j[2] então Maria recebe um ponto.

Finalmente, para os elementos 3 , m[3] < j[3] então João recebe um ponto.

A matriz de retorno é [1, 1] com a pontuação de Maria primeiro e a de João em segundo.


***Descrição da função***

Complete a função compareNotes.
compareNotes tem os seguintes parâmetros:
 - int m[4] : Classificação de notas de Maria
 - int j[4] : Classificação de notas de João


***Retornar***

int[2] : A pontuação de Maria está na primeira posição e a pontuação de João está na segunda.


***Entrada de Amostra***
```
6 8 7 9
9 6 7 10
```
**Saída de Amostra**
```
1 2
```
A matriz de retorno é ***[1,2]*** .
