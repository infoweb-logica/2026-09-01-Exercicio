# 2026.2 - Python - Atividade pré avaliação

## Informações gerais

- **Público alvo**: alunos da disciplina de **Introdução a lógica e programação** do curso de [Infoweb](https://diatinf.ifrn.edu.br/cursos/tecnico-em-informatica-para-internet/) na [DIATINF](https://diatinf.ifrn.edu.br/) no [CNAT-IFRN](https://portal.ifrn.edu.br/campus/natalcentral/)
- **Professor**: [L A Minora](https://github.com/leonardo-minora/)
- **Objetivo**:
  1. Mostrar como será a próxima atividade avalitiva

---
## Questões

### 1. Execute mentamelmente ("faça o chinês") do programa python abaixo e para cada conjunto de entrada, escreva a saída correspondente.

```python
numeros = [int(numero) for numero in input().split()]
# numeros = [23, -32, 1, -2, 3, 4, -5, 6, 7, 8, 9, 10]
resultado = 0
outro_resultado = 1
for numero in numeros:
   resultado += numero
   outro_resultado *= numero

print(f"resultado 1: {resultado}")
print(f"resultado 2: {outro_resultado}")
```

| Entradas  | Saídas |
| --------- | ------ |
| 2 3 5 8   |  |
| 1 -2 3 -4 |  |
| -1 -2 3 4 |  |
| 5 -1 2 1  |  |

### 2. Execute mentamelmente ("faça o chinês") do programa python abaixo e para cada conjunto de entrada, escreva a saída correspondente.

```python
repeticoes = int(input())
numeros = [int(numero) for numero in input().split()]
positivo = 0
negativo = 0
for indice in range(repeticoes):
  if numeros[indice] > 0:
    positivo += 1
  elif numeros[indice] < 0:
    negativo += 1
print(f'zero: {repeticoes-negativo-positivo}')
print(f'negativo: {negativo}')
print(f'positivo: {positivo}')

```

| Entradas                | Saídas |
| ----------------------- | ------ |
| 2<br />1 -2 3 -4 5 0 -6 |  |
| 4<br />1 -2 3 -4 5 0 -6 |  |
| 6<br />1 -2 3 -4 5 0 -6 |  |


### 3. Soma da fila
Você recebeu uma fila com `N` números inteiros. Seu programa deve somar todos os valores da lista e mostrar o resultado final.
Para resolver, percorra a lista inteira e acumule a soma em uma variável.

**Entrada**
- A primeira linha contém um inteiro `N`, quantidade de elementos da lista.
- A segunda linha contém `N` inteiros separados por espaço.

**Saída**
- Imprima a soma de todos os elementos.

**Exemplo**
```text
Entrada
5
3 1 4 1 5

Saída
14
```

### 4. Dobrar pares
Crie uma nova lista em que apenas os números pares sejam multiplicados por 2.
Os números ímpares devem permanecer iguais.

**Entrada**
- A primeira linha contém `N`.
- A segunda linha contém `N` inteiros.

**Saída**
- Imprima a lista resultante.

**Exemplo**
```text
Entrada
5
2 3 4 5 6

Saída
4 3 8 5 12
```

### 5. Compressão por frequência
Dado um inteiro `K`, cada valor pode aparecer no máximo `K` vezes na lista de saída.
Se um número aparecer mais vezes, mantenha apenas as primeiras `K` ocorrências.

**Entrada**
- A primeira linha contém `N` e `K`.
- A segunda linha contém `N` inteiros.

**Saída**
- Imprima a lista comprimida.

**Exemplo**
```text
Entrada
10 2
3 1 3 3 2 1 1 2 2 2

Saída
3 1 3 2 1 2
```
