# Java básico



#### IDE

ambiente de desenvolvimento integrado, da a opção de ficar acompanhando a execução.

oferece:

* aceleração de nossa escrita com auto-completo ou inteliSense
* formatação de palavras e blocos de códigos
* análise de erro de sintaxe
* compilação de programa
* Depuração (acompanhamento) de execução do programa

cada IDE possui suas qualidades

* **Eclipse**: é a IDE mais utilizada no ambiente corporativo, com interface bem interativa
* **NetBeans**: utilizada mais em ambiente acadêmico e com versão de menu e assistentes em português
* **IntelliJ**:  oferece muitos recursos de inteligência para agilidade de nosso desenvolvimento com sugestões de ações bem assertivas.  
* **VS Code**: muito utilizados por desenvolvedores que já atuam com NodeJs ou plataformas de front-end. 

## configuração do ambiente

JDK para desenvolvimento É um **pacote de software** que você pode usar para desenvolver aplicativos baseados em **Java** (Java development kit) pra começar a desenvolver em Java é necessário ter instalado o JDK

JRE (Java Runtime Environment) é uma camada de software que é executado sobre um software de sistema operacional de um computador e fornece as bibliotecas de classe e outros recursos que um programa específico do Java precisa executar.

#### Intellij

Em uma única ferramenta, consegue-se gerenciar toda a parte do projeto do desenvolvimento, etc.

 Após configurar a IDe;

* criar um novo projeto
* criar um arquivo na pasta src (é onde contem o código fonte)
* diretório do projeto definido

uma das vantagens do intellij é que ele salva automaticamente a cada alteração

## Anatomia das classes

Uma **classe** é um elemento do código Java que utilizamos para representar objetos do mundo real. Dentro dela é comum declararmos atributos e métodos, que representam, respectivamente, as características e comportamentos desse objeto.

O ponto inicial do arquivo, das interações com a linguagem, é comum iniciar o projeto criando um **arquivo.java** e esse arquivo tem um padrão que é o nome do arquivo **e esse nome do arquivo tem que está coerente com a expressão que se irá escrever** com o conteúdo que se vai representar, e todo o conteúdo fica entre chaves, definimos os elementos a ela relacionados: atributos, construtores e métodos. 

```java
ex: public class MinhaClss {

​    //o código aqui

} 
```

A classe deve possuir o mesmo nome do arquivo.java

* Todos os arquivos que forem gerados, sempre se iniciará com a letra maiúscula junto com cada palavra complementar (ao criar métodos e variáveis essas regras sofrerão alteração), por padrão todas as classes as primeiras palavras precisarão estar em maiúsculas. 

* grande parte das classes que serão criadas, serão iniciada com a expressão `public class`e o nome intuitivo da classe. 

* também é possível especificar o **modificador de acesso**. Por meio dele informamos a visibilidade da classe, que pode ser **public, private** ou **default.** 

## Declaração de variáveis e métodos

Uma variável corresponde a uma posição de memória. Uma posição de memória pode guardar um valor.

Estrutura:

```java
Tipo NomeBemDefinido = Atribuição (opcional em alguns casos)
```

**int** correspondente a um subconjunto finito do conjunto dos inteiros 

**double** correspondente a um subconjunto finito do conjunto dos números reais

**boolean** corresponde a valores lógicos, true ou false, sim e não



```java
int v1;
double v2;
v1=123;
v2=3.1415;
```

Toda variável na linguagem Java terá a necessidade de dizermos o tipo.

ao manipular uma variável altera-se apenas o valor de atribuição

#### Métodos

```java
TipoRetorno NomeObjetivoNoinfinitivo Parametro (s)

Ex: int somar (int numeroUm, int numero2) dois parâmetros.
```

* Os métodos na linguagem Java costumam ser aplicados no infinitivo.
* Todo método tem os seus parâmetros e um método pode receber parâmetros de tipos diferentes.

 String primeiroNome = "nome"

String segundoNome = "segundo nome"



```java
String nomeComplet = nomecompleto (primeiroNome, segundoNome)
```

O valor desta variável é  a chamada de um método que também tem o mesmo nome.

#### Identação 

É o espaçamento aplicado no início das linhas de código que ajuda a manter uma hierarquia visual. Na maioria das linguagens esse não é um elemento que impede o código de ser compilado, mas manter o código **indentado** é fundamental para facilitar sua leitura, boas práticas de desenvolvimento.

#### Java Beans

Escrever algoritmos legíveis para a compreensão. Para isso a linguagem Java sugere formas de escrita universal para as classes atributos e métodos.

**Variáveis** 

* Uma variável precisa ser clara, sem abreviações ou definições sem sentido;
* Uma variável é sempre no singular, **exceto quando se refere a um array [] ou coleção.**
* Definir sempre as variáveis em um único idioma.

**Métodos** 

Os métodos deverão ser nomeados como verbos, através de uma mistura de letras maiúsculas e minúsculas. 

## Java sintaxe

#### Tipos e variáveis

Há oito tipos primitivos em Java:

int, byte, short, long, float, double, boolean e char

| Tipo  | Memória | Valor mínimo               | valor máximo                 |
| ----- | ------- | -------------------------- | ---------------------------- |
| Byte  | 1 byte  | -128                       | 127                          |
| short | 2 byte  | -32.768                    | 32.767 ex: anos              |
| int   | 4 byte  | -2.147.483.648             | 2.147.483.647 é a mais comum |
| long  | 8 byte  | -9.223.372.036.854.775.808 | 9.223.372.036.854.755.807    |

Tipos que podem conter partes **fracionárias**

| tipo   | Memória | Mínimo         | Máximo                     |
| ------ | ------- | -------------- | -------------------------- |
| float  | 4 bytes | -3,4028E + 38  | 3,4028E + 38               |
| double | 8 bytes | -1,7976E + 308 | 1,7976E + 309 o mais comum |

Toda variável é composta por: tipo + identificação + valor atribuído (opcional

#### Variáveis e constantes

Uma variável é uma área de memória, associada a um nome, que pode armazenar valores de um determinado tipo. Java é uma linguagem com rigidez de tipos, diferente de linguagens como Java Script, onde declarar o tipo de variável não é obrigatório. Uma referencia em Java pode ser redirecionada a outro valor, portanto o valor pode variar.

Já as constantes são valores armazenados em memória que não podem ser modificados depois de declarados. Para declarar uma variável como uma constante, utiliza-se a palavra `final`. Constantes são sempre escritas em CAIXA ALTA

## Operadores

São símbolos especiais que tem um significado próprio para a linguagem e estão associados a determinadas operações.

= é uma atribuição e o valor atribuído pode ser alterado(recebe) 

Ex: 

```java
String nome = "Adriely"; 
int idade = 22;
double peso = 68.5;
char sexo = 'F';
boolean doadorOrgao = false;
date dataNascimento = new date();
```

#### Aritméticos 

```java
double soma = 10.5 + 15.7;
int subtração = 113 - 25;
int multiplicação = 20 * 7;
int divisâo = 15 / 3;
int modulo = 18 % 3;
double resultado = (10 * 7) + (20/4);
```

O operador de adição quando utilizado em variáveis do tipo texto, realizará a concatenação de textos. Ele faz a junção quando se tem palavras que precisam ser acopladas em um único resultado.

Exemplo: 

```java
String nomeCompleto = "LINGUAGEM" + "JAVA";
```

## Mapa de atalhos

A classe precisa ter um método principal, denominamos esse método de Main que irá ter uma característica única na sua representação de inicialização, com isso, ele precisa seguir um padrão.

| Main, subentende que é o método main.         | main = public static void main(String[] args) { |
| :-------------------------------------------- | :---------------------------------------------: |
| Sout: comando de impressão na linguagem Java. |       System.out.println("hello  world");       |
| ctrl+shift+P                                  |                criar um projeto                 |
| ctrl+k                                        |              abre a tela de commit              |







