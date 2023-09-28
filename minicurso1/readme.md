# Lógica aplicada à Matemática

## Conceitos iniciais

> **Proposições**: são afirmações as quais podemos atribuir um valor verdadeiro ou falso. 

_Exemplos_
- A lua é um planeta
- O céu é azul
- Matemática é a melhor disciplina

_Contraexemplos_
- Você vai no cinema amanhã?
- Que horas passa o próximo ônibus? 


> **Conectivos**: são operadores lógicos que usamos para aglutinar proposições.

_Exemplos_
- e
- ou
- não
- se ... então ...
- se e somente se

_Exemplos_
- A lua é cinza e a lua é cheia de crateras
- O número 2 é primo ou o número 17 é par
- Se um número é primo então esse número é ímpar

> **Proposições atômicas**: são proposições que não podem ser divididas em proposições menores.

# Cálculos das proposições

Para simplificar, utilizamos letras para representar proposições atômicas, geralmente $p$, $q$, $r$ e $s$.

## Operações com proposições

Quando aglutinamos proposições usando conectivos, podemos calcular o valor-verdade da nova proposição formada usando os valores das proposições atômicas. 

### Negação: Operador `não`

A negação, também chamada de operador `não`, é denotada pelo símbolo $\sim$ ou $\neg$. 

_Exemplo_
- $p=$ "o número 2 é ímpar"
- $\sim p =$ "o número 2 não é ímpar"

#### Tabela-verdade da negação

| $p$ | $\sim p$ |
| --- | :---: | 
|  V  |  F  |
|  F  |  V  | 


### Conjunção: Operador `e`

A conjunção, também chamada de operador `e`, é denotada pelo símbolo $\wedge$. 

_Exemplo_

- $p=$ "A lua é cinza"
- $q=$ "A lua é cheia de crateras" 
- $p\wedge q$ = "A lua é cinza e a lua é cheia de crateras". 

Dadas duas proposições $p$ e $q$, o valor-verdade de $p\wedge q$ será verdadeiro somente quando $p$ e $q$ forem ambas verdadeiras. Caso contrário, o valor da conjunção será falso. 

#### Tabela-verdade da conjunção

| $p$ | $q$ | $p\wedge q$|
| --- | --- | :----------: |
|  V  |  V  |  V |
|  V  |  F  |  F |
|  F  |  V  |  F |
|  F  |  F  |  F |


### Disjunção: Operador `ou`

A disjunção, também chamada de operador `ou`, é denotada pelo símbolo $\vee$.

_Exemplo_

- $p=$ "o número 2 é primo" 
- $q=$ "número 17 é par"
- $p\vee q=$"o número 2 é primo ou o número 17 é par"

Dadas duas proposições $p$ e $q$, o valor-verdade de $p\vee q$ será verdadeiro caso pelo menos uma das afirmações $p$ ou $q$ seja verdadeira. Caso contrário, o valor-verdade da disjução é falso.

#### Tabela-verdade da disjunção

| $p$ | $q$ | $p\vee q$|
| --- | --- | :----------: |
|  V  |  V  |  V |
|  V  |  F  |  V |
|  F  |  V  |  V |
|  F  |  F  |  F |


### Condicional: `se então`

O operador condicional, é denotado por $\rightarrow$, e em linguagem coloquial é construído com a frase "se [...] então [...]". 

_Exemplo_

- $p=$ "ela dança" 
- $q=$ "eu danço"
- $p\rightarrow q =$ "se ela dança então eu danço"

Dadas duas proposições $p$ e $q$, o valor-verdade da condicional $p\rightarrow q$ só será falso caso $p$ seja verdadeira e $q$ seja falsa. Caso contrário, a condicional é verdadeira.

> Na construção $p\rightarrow q$, $p$ é chamada _condição necessária_ e $q$ é chamada _condição suficiente_.


#### Tabela-verdade da condicional

| $p$ | $q$ | $p\rightarrow q$|
| --- | --- | :----------: |
|  V  |  V  |  V |
|  V  |  F  |  F |
|  F  |  V  |  V |
|  F  |  F  |  V |

### Bicondicional: `se e somente se`

O operador bicondicional, denotado por $\leftrightarrow$, e em linguagem coloquial é construído com a frase "[...] se o somente se [...]"

_Exemplo_

- $p=$ "eu vou ao parque" 
- $q=$ "está fazendo sol"
- $p\leftrightarrow q=$ "eu vou ao parque se e somente se está fazendo sol"

Dadas duas proposições $p$ e $q$, o valor-verdade da bicondicional $p\leftrightarrow q$ é verdadeiro quando ambos os valores-verdade de $p$ e $q$ são iguais. Caso contrário, o valor da bicondicional é falso.

#### Tabela-verdade da condicional

| $p$ | $q$ | $p\leftrightarrow q$|
| --- | --- | :----------: |
|  V  |  V  |  V |
|  V  |  F  |  F |
|  F  |  V  |  F |
|  F  |  F  |  V |

# Contradição e Tautologia

> Uma contradição é uma proposição composta que possui o valor-verdade sempre falso, independente do valor-verdade das proposições atômicas que o constituem.

_Exemplo_
$$p \wedge \sim p$$

> Uma tautologia é uma proposição composta que possui o valor-verdade sempre verdadeiro, independente do valor-verdade das proposições atômicas que o constituem.

_Exemplo_
$$ p \vee \sim p$$

# Validade de argumentos

Um _argumento_ é composto de uma lista de proposiçoes $p_1, p_2, \ldots, p_n$ que serão chamadas de _premissas_, e uma proposiçao _q_ chamada de _conclusão_. 
> Dizemos que o argumento é _válido_ se, toda vez que as premissas forem todas verdadeiras, a conclusão também é verdadeira. 

Quando o argumento é válido, denotamos por 
$$ p_1, p_2, \ldots, p_n \models q$$

_Exemplo 1_

- $p_1=$ "se choveu hoje então a rua está molhada"
- $p_2=$ "a rua não está molhada"
- $q_1=$ "não choveu hoje"

O argumento acima é válido (construir a tabela-verdade).


_Exemplo 2_

- $p_1=$ "se choveu hoje então a rua está molhada"
- $p_3=$ "não choveu hoje"
- $q_2=$ "a rua não está molhada"

O argumento acima é inválido (construir a tabela-verdade).



# Lógica de predicados

Nem toda lógica pode ser descrita usando proposições. As vezes, queremos fazer afirmações sobre elementos de conjuntos. Um _predicado_ denota uma relação entre objetos de um determinado contexto de discurso. Esse contexto de discurso é um conjunto no qual os objetos existem. 

_Exemplos_
- Sócrates é mortal
- O número 2 é primo
- Um pássaro voa

Nesse caso, simbolizamos os predicados com letras maiúsculas, e deixamos uma _variável livre_, abaixo denotada por $x$.

- M(x) = x é mortal
- P(x) = x é primo
- V(x) = x voa

As frases acima se traduzem como

- M(Sócrates)
- P(2)
- V(pássaro)



## Quantificadores

Quando estamos falando de predicados, geralmente queremos fazer afirmações do tipo 
- Existe um elemento com tal propriedade
- Todo elemento satisfaz essa propriedade

Para isso, usamos os quantificadores

### Existe

Considerando o predicado $P$ anterior, a seguinte construção
$$\exists x, P(x)$$
 é lida como "existe um x tal que P(x)". Como P(x) significa "x é primo", a construção se traduz como 

> Existe um x que é primo

### Para todo

Considerando o predicado M acima, a construção
$$\forall x, M(x)$$
é lida como "para todo x, M(x)". Como M(x) significa "x é mortal", a construção se traduz como
> Todo x é mortal 


