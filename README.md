# List Comprehension X Filter

## Sintaxe:
` [ expression | generators, conditions ]`
- generators: Fornecem a lista de origem;
- conditions: São filtros a serem aplicados as listas de origem fornecidas pelos generators;
- expression: Expressão que será aplicada a cada valor da lista de origem;
## Exemplo:
![exemplo](img/exemplo.png)

## Exemplos de List Comprehension como Filter:
- O código acima usando List comprehension: `[x+1 | x <- [1..100], mod x 10 == 0]`
Usando Filter: `map (\x -> x+1) (filter (\x -> mod x 10 == 0) [1..100])`