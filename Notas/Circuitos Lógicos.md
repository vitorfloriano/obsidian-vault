---
alias: Logic Gates, Logic Circuits, Truth Tables, Binaries, Binários
tags: cs, com100, semana3
---
# Circuitos Lógicos

Circuitos lógicos são representações de [[Álgebra Booleana]] utilizadas em computadores.

Quando falamos de binários, estamos tratando de conceitos para representar ligado e desligado, verdadeiro ou falso. Por isso utiliza-se 0 e 1, sendo 0 desligado, ou falso, e 1 ligado ou verdadeiro.

| binary | state | truth | voltage |
| :---: | :---: | :---: | :---: |
| 0 | off | F | 0 volt |
| 1 | on | T | 0< voltz |

#### Operações

AND = product
OR = sum
0' = 1
1' = 0

#### Propriedades da Lógica Booleana
|Property | OR (sum) | AND (product)|
| :---: | :---: | :---:|
|Commutative Property|a+b = b+a|a.b = b.a|
|Associative Property|a+(b+c) = (a+b)+c |a.(b.c) = (a.b).c|
| Identity Property | a+0 = a | a.1 = a |
| Null Property | a+1 = 1 | a.0 = 0 |
| Complement Property | a+a' = 1 | a.a' = 0 |

1 + 1 = 1 em circuitos lógicos.

## Buffer Gate

| input | output |
| :---: | :---: |
| a | a |
| 1 | 1 |
| 0 | 0 | 

## NOT Gate

| input | output |
| :---: | :---:|
| a | a'|
| 0 | 1 |
| 1 | 0 |

Sempre é o contrário.

### NOT Gate Logic Circuit

![[NOT-gate.gif]]

## AND Gate

| input | input | output |
| :---: | :---: | :---: |
| a | b | a.b |
| 0 | 0 | 0 |
| 1 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 1 | 1 |

### AND Gate Logic Circuit

![[AND-gate.gif]]

## OR Gate

| input | input | output |
| :---: | :---: | :---: |
| a | b | a+b |
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 1 |

### OR Gate Logic Circuit

![[OR-gate.gif]]

## NAND Gate

| input | input | output |
| :---: | :---: | :---: |
| a | b | (a.b)'|
| 0 | 0 | 1 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 1 | 1 | 0 |

É o contrário do [[#And Gate]].

### NAND Gate alternativo

| input | input | output |
| :---: | :---: | :---: |
| a | a | (a.a)'|
| 1 | 1 | 0 |
| 0 | 0 | 1 |

É o mesmo que um [[#Not Gate]].

## NOR Gate

| input | input | output |
| :---: | :---: | :---: |
| a | b | (a+b)'|
| 0 | 0 | 1 |
| 1 | 0 | 0|
| 0 | 1 | 0 |
| 1 | 1 | 0 | 

NOR Gate é o contrário (complemento) do [[#Or Gate]].

# XOR Gate

| input | input | output |
| :---: | :---: | :---: |
| a | b | |
| 0 | 0 | 0 |
| 1 | 0 | 1 |
| 0 | 1 | 1 |
| 0 | 0 | 0 | 

### XOR Gate Logic Circuit

![[XOR-gate.gif]]