# Atividade Avaliativa 1 — Recursividade em C
 
## Soluções
 
**Exercício 1 — Fibonacci ingênuo**
Caso base: `fib(0) = 0`, `fib(1) = 1`. A cada chamada o problema é reduzido em dois subproblemas menores (`fib(n-1)` e `fib(n-2)`). O contador de chamadas é passado por ponteiro para evidenciar a ineficiência — complexidade O(2ⁿ).
 
**Exercício 2 — Fibonacci memoizado**
Mesmos casos base. Antes de calcular, a função verifica um cache (`long long*`) alocado dinamicamente com `malloc` e inicializado com `-1`. Se o valor já existe, retorna sem novas chamadas. O programa exibe as duas versões lado a lado para comparação — complexidade O(n).
 
**Exercício 3 — Torres de Hanoi**
Caso base: `n == 0`, nada a fazer. A cada chamada o problema de `n` discos é reduzido a dois subproblemas de `n-1` discos com o pino auxiliar alternado. A solução sempre executa exatamente `2ⁿ − 1` movimentos.
