# Lógica Proposicional 

É a forma mais básica de lógica. A ideia central dela é trabalhar com proposições, que são sentenças declarativas que podem ser classificadas, sem ambiguidade, como verdadeiras (V) ou falsas (F).
<br>

É um conjunto infinito e contável de átomos (SImbolos Proposicionais, Variáveis Proposicionais)<br>
P = {P₁, P₂, P₃, ...}

***

### Operadores Lógicos, conectivos e outros simbolos: 

#### Unários:
- Negação (NÃO): ¬
    
#### Binários
- Conjunção (E): ∧

- Disjunção (OU): ∨

- Implicação (SE ... ENTÃO): →


#### Simbolos Auxiliares
- Parenteses "(" , ")"

<br>

***
### Na Lógica Proposicional não é possível expressar:

- Quantificações ("Todos", "Existe").
- Relações (Comparações).
- Propriedades.

<br>

*** 

### Linguagem Proposicional Llp (Conjunto de Fórmulas)

- ### Caso Base:
Átomos (Simbolos Proposicionais) ∈ Llp

- ### Caso Indutivo 01:
Se A ∈ Llp, então (¬A) ∈ Llp

- ### Caso Indutivo 02:
Se A, B ∈ Llp, então (A∧B), (A∨B), (A→B) ∈ Llp


### O conjunto Llp é o menor obtido das regras anteriores!

***

### Simplificar a notação (Metalinguagem)

- Simbolos Proposicionais <br>
(p, q, r, s, ...)

- Fórmulas Quaisquer <br>
(A, B, C, ...)

- Dispensar parenteses <br>
    - (P∧Q) ➔ p∧q 
    - Em uso repetido de V ou ∧
    - Quando p→q→r→s 
    - Por precedencia: ¬, ∧, V, →

<br>

***

### Subfórmulas
Definimos SUB(A) (subfórmulas) indutivamente:

- Caso Base: A = P <br>
SUB(P) = {P} 

- Caso Indutivo A = ¬B <br>
SUB(¬B) = {¬B} ∪ SUB(B)

- Caso Indutivo A = B □ C | □ ∈ {∧, V, →} <br>
SUB(B □ C) = {B □ C} ∪ SUB(B) ∪ SUB(C)