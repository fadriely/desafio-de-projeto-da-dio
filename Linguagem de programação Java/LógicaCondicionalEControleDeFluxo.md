# Operadores relacionais

"são símbolos especiais quais são capazes de realizar comparação entre **determinados** (nem todo operador relacional pode ser utilizado em qualquer tipo de dado) operandos e, em seguida, retornar um resultado "

Tipos:

* **Similaridade**: igual, diferente
* **Tamanho:** maior, maior igual, menor, menor igual 

em comparação relacionais, sempre existirão dois operandos mesmo que esses operandos sejam iguais 

### **Similaridade**  

* Igualdade: determina se um operando é igual ao outro
* Diferença: determina se um operando não é igual ao outro

**Simbologia**

* igualdade: == 

  ```java
  //tem que se ter um cuidado ao utilizar o operador de igualdade ou de diferença com classes de objetos
  ```
* Diferença: !=

### **Tamanho**

* maior: determina se um operador é maior do que outro
* maior igual: determina se um operador é maior ou igual a outro
* menor igual: determina se um operador é menor ou igual a outro

**simbologia**

* Maior: >

* Maior igual: >=

* Menor igual: <=

  

  # Operadores lógicos

  "São símbolos especiais quais são capazes de realizar comparações lógicas entre operadores lógicas ou expressões e, em seguida, retornar um resultado"

  

  Tipos:

  * Conjunção 
  * Disjunção exclusiva
  * Negação

  ```java
  //não posso aplicar comparações lógicas em cima de números, apenas em relacionais, lógicos não. A não ser que esses números estejam dentro de expressões
  ```

  

Tipos:

* **Conjunção:** operação lógica que só é verdadeira quando ambos os operandos ou expressões envolvidas são verdade

  Simbologia:  

  * && 

  Terminologia:

  - and(e)

* **Disjunção:** operação que só é falsa quando ambos os operandos ou expressões envolvidas são falsos

Simbologia:

* I I

Terminologia:

* or (ou)

* **Disjunção exclusiva:** operação que só é verdade quando ambos os operandos ou expressões são opostos

Simbologia:

* ^

Terminologia:

* xor

* **Negação:** operação que inverte o valor lógico de um operando ou expressão

Simbologia:

* !

Terminologia:

* invenção

| O-E  | O-E  |  R   |
| :--: | :--: | :--: |
|  V   |  V   |  V   |
|  V   |  F   |  F   |
|  F   |  V   |  F   |
|  F   |  F   |  F   |



​				O - Operando E - Expressão R - Resultado



boolean b1 = true; boolean b2 = false;
boolean b3 = true; boolean b4 = false;

a) b1 && b2 = false

b) b1 && b3 = true

c) b2 || b3 = true

d) b2 || b4 = false

e) b1^b3 = false

f) b4 ^ b1 = true

g) !b1 = false (inversões)

h) !b2 = true 

// (i1 > i2) || (f2 < f1) ((i1 + i2) < (f2 - f1)) && true



## Controle de fluxo

"São estruturas que tem a capacidade de direcionar o fluxo do código"

* Tipos:
  Decisão: if, if-else, if-else-if, switch e operador ternário
  Repetição: for, while, do while
  Interrupção: break, continue e return

* Tipos:
  Decisão: estrutura que avalia uma condição booleana ou variável para direcionar o fluxo de execução

   ![S](C:\Users\ferre\OneDrive\Imagens\Pictures\Screenshots\Captura de tela 2023-03-30 152400.png)

Tipos:
• Decisão
if (idade > 18) {
}
if (aprovado) {
} else {
}
if (casado && temFilhos) {
} else if (casado && sem Filhos) {
} else {
}

//se o código começar a crescer muito é sinal de que ele precisa ser melhorado

* Decisão: operador ternário

![](C:\Users\ferre\OneDrive\Imagens\Pictures\Screenshots\Captura de tela 2023-03-30 152836.png)

* Decisão: escolha

![](C:\Users\ferre\OneDrive\Imagens\Pictures\Screenshots\Captura de tela 2023-03-30 153253.png)

* Decisão: switch
  Variável:
  byte
  short
  char
  int
  Enum
  String

   switch (variável) {
  case 1:
  break;
  case... :
  break;
  default:
  break;
  }

switch (olhos) { case "AZUIS": break;
case "VERDES":
break;
case "CASTANHOS": break; default: }
break;

### Boas práticas

* Switch é para valores exatos e if para expressões booleanas
* Evitar usar o default do switch para "cases genéricos" //o default é para indicar que o valor passado está errado
* Evitar o efeito "flecha" dos if's
* Evitar muitos if's aninhados
* Usar a boa prática da aula 2 para diminuir o tamanho if
