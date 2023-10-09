---
alias: Numeric Systems, Sistema Numérico Decimal, Sistema Numérico Binário, Notação Posicional, Positional Notation, Base-10 (decimal), Base-2 (Binary), Base 2 (Binário)
tags: math, com100, semana3, univesp
---
# Sistemas Numéricos

No mundo atual, a maioria das coisas utilizam um sistema de representação numérica de base 10, ou seja, utilizando 10 dígitos, 0 até 9.  Com estes números é possível representar qualquer outro número real.

Com computadores, utiliza-se o sistema numérico de base 2, ou[[Circuitos Lógicos| binário]], para representar qualquer combinação numérica.

## Base-10 (decimal)

Se observarmos o número 263, este possui 2 centenas, 6 centenas e 3 unidades.

Em um sistema de notação base 10, a casa à esquerda é 10 vezes a casa à direita, por isso temos 1s (unidades), 10s (dezenas) e 100s (centenas).

|100s | 10s | 1s |
|:---: | :---: | :---: |
|2 | 6 | 3 |

A coluna à esquerda sempre é dez vezes a coluna anterior porque há 10 combinações possíveis (0-9) para aquela coluna antes de passar para a próxima.

Se o número for maior que 9, é necessário [[Carry Operation|levar um]], e assim será nas próximas casas (10s, 100s, 1000s, etc).

## Base-2 (binary)

Em um sistema binário, temos apenas duas possibilidades dentro de cada coluna, 0 e 1, a coluna à esquerda sempre será o dobro (x2) da coluna anterior, 1s, 2s, 4s, 8s, 16s, e assim por diante.

### 101 na base-2

Por exemplo, o binário 101 possui um 1, zero 2, e um 4, que se somados, 4+0+1, é igual à 5.

| casa | 4s | 2s | 1s|
| :---:|:---:|:---:|:---:| :---:|
|binário| 1 | 0 | 1 |
| decimal | 4 | 0 | 1 |
| resultado em decimal | 4  | + 0  | + 1  | = 5 |

Logo, 101 representa 5 decimal.

Podemos representar números maiores com binários, precisando apenas de uma sequencia maior.

### 10110111 na base-2

| casa | 128s | 64s | 32s | 16s | 8s | 4s | 2s | 1s |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:| :---:|
| binário |1|0|1|1|0|1|1|1|
| decimal |128 |0 | 32 |16| 0| 4|2|1|
| resultado em decimal |128 | +  0 | + 32 | + 16 | + 0 | + 4 | + 2 | + 1 | = 183 |

![[10110111-binary.gif]]

### Soma de binários

A lógica é semelhante à base-10, com operações de [[Carry Operation|vai-um]], sempre que o limite da casa é excedido.

Compare 183+19 em decimal e binário.

![[202-decimal.gif]]

![[202-binary.gif]]

## bits

Em binário, cada dígito é um [[bit]], e em um número de [[8-bit |8 bits]], os números vão de 0, sendo 00000000, à 255, sendo 11111111.

Computadores mais antigos utilizavam pedaços de 8 bits para executar operações, o que era limitado.

![[24-bit vs 8-bit image.png]]

Jogos 8-bit só podiam utilizar 256 cores. Músicas 8-bit só podem utilizar 256 notas.

1 [[Byte]] são 8 [[bit|bits]].

A maioria dos computadores utiliza o primeiro bit para representar se o número é positivo ou negativo, sendo 0 positivo e 1, negativo.

Em um computador de 32-bit, sobrariam 31 bits para representar um número, o que daria um alcance de aproximadamente 2 bilhões de combinações possíveis, positivo e negativo.

Já com 64-bits, temos 63 bits podemos chegar à 9.2 quintilhões de combinações, positivo e negativo.

Parece muito, mas se colocarmos na conta os números "picados" e as letras ,maiúsculas e minúsculas, e sinais de todos os alfabetos possíveis, não parece tanto.
 
