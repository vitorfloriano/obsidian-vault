---
tags: com100, semana6, univesp
alias: Teoria dos Grafos
---
# Grafo

Abstração utilizada para solucionar problemas de melhor rota entre pontos.

## Alguns tipos de grafos

- **Dirigido**: as arestas tem direção única, podendo ser:
	- **Cíclico**: as arestas voltam ao vértice inicial depois de terem visitado os vértices intermediários.
	- **Acíclico**: não volta ao vértice inicial. Não tem ciclo.
- **Não dirigido**: as arestas se conectam aos vértices em ambas as direções.
- **Ponderado**: cada aresta tem um valor, custo, associado, como tempo, dinheiro e energia, que deve ser pago ao passar por ela. 
- **Não ponderado**: todas as arestas tem o mesmo ou nenhum custo associado.
- **Denso**: muitas arestas, se comparado ao número de vértices.
- **Esparso**: poucas arestas, se comparado ao número de vértices.

### Grafo não dirigido

Não importa a sequência e direção em que os pontos se conectam. 

Exemplo: mapa rodoviário.

![[Pasted image 20220917201458.png]]

### Grafo dirigido

A direção em que os pontos se conectam é importante. 

Exemplo: vias de mão única em um mapa rodoviário.

![[Pasted image 20220917201525.png]]

### Grafo misto

Mistura de grafos dirigidos e não dirigidos. Podem ser subgrafos.

Exemplo: mapa rodoviário com vias de mão dupla e mão única.

### Grafo Ponderado

Mapa com valores atribuídos aos caminhos entre os pontos.

Exemplo: menor distância, melhor rota, em um mapa rodoviário.

![[Pasted image 20220917201606.png]]

### Grafos Acíclicos Dirigidos (DAGs)

Um dos mais importantes grafos, pois tem muitos usos práticos.

#### Princípios básicos dos DAGs:

- Seguem um ordem particular que impedem que você vá de um vértice para outro e volte por qualquer rota.
- Fornece caminhos específicos entre os vértices e permitem criar conjunto previsível de rotas.

São muito usados em estruturas organizacionais, como árvores genealógicas.

São mais fáceis de processar do que muitos outros tipos de grafos, pois permite criar rotas previsíveis, mesmo quando a rota não seguir uma ordem cronológica ou dominante.

# Buscas

## Busca em largura (BFS)

Breadth-First Search explora todas as arestas ligadas a um determinado vértice.

Sua maior vantagem é sempre retornar o menor caminho entre dois pontos quando buscar melhor rota.

Precisa de muita memória porque armazena todos os caminhos antes de encontrar uma solução.

## Busca em profundidade (DFS)

Explora todas as possibilidades de conexão entre as vértices e arestas existentes.

Mais usada quando encontrar todas as rotas é mais importante do que encontrar o caminho mais curto.

Muito utilizado em jogos e labirintos.

Precisa de menos memória , mas não garante solução mais curta e direta.

