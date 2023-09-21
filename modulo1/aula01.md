# Funções: definição, domínio, contradomínio e imagem.

## Introdução 

Antes de mais nada, precisamos nos situar. Eu assumo que vocês já tenham algum conhecimento de teoria dos conjuntos: noção intuitiva do que é um conjunto, o que significa dizer que um elemento pertence a um conjunto. 

Dado que sabemos o que é um conjunto, podemos falar de funções. Funções nada mais são do que associações feitas entre elementos de diferentes conjuntos. Você associa um elemento de um conjunto A com um elemento de um conjunto B e tudo certo. 

Sem adentrar no mundo matemático, podemos pensar em uma função associando cada elemento de um conjunto de chaves a um elemento de um conjunto de fechaduras. Ou também associando cada elemento de um conjunto de placas de veículos a um elemento de um conjunto de veículos. 

Podemos pensar então em algo como

```mermaid
flowchart LR
    chaves --> fechaduras
    placas --> veículos
```

Em notação matemática, usamos a notação $$f:A\to B$$ para representar uma função de nome $f$ que associa elementos do conjunto $A$ a elementos do conjunto $B$.

Na notação acima, chamamos o conjunto $A$ de **domínio** da função $f$ e o conjunto $B$ de **contradomínio**.


## Formalizando

Uma função é uma relação de um conjunto $A$ num conjunto $B$ tal que cada elemento de $A$ está associado a um único elemento de $B$.

## Imagem

A imagem de uma função é o conjunto de todos os elementos do contradomínio que estão associados a algum elemento do domínio.