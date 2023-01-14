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

`ex: public class MinhaClss {`

​    `//o código aqui`

`}` 

A classe deve possuir o mesmo nome do arquivo.java

* Todos os arquivos que forem gerados, sempre se iniciará com a letra maiúscula junto com cada palavra complementar (ao criar métodos e variáveis essas regras sofrerão alteração), por padrão todas as classes as primeiras palavras precisarão estar em maiúsculas. 

* grande parte das classes que serão criadas, serão iniciada com a expressão `public class`e o nome intuitivo da classe. 

* também é possível especificar o **modificador de acesso**. Por meio dele informamos a visibilidade da classe, que pode ser **public, private** ou **default.** 

## Declaração de variáveis e métodos

Uma variável corresponde a uma posição de memória. Uma posição de memória pode guardar um valor.

Estrutura:

`Tipo NomeBemDefinido = Atribuição (opcional em alguns casos)`

**int** correspondente a um subconjunto finito do conjunto dos inteiros 

**double** correspondente a um subconjunto finito do conjunto dos números reais

**boolean** corresponde a valores lógicos, true ou false, sim e não



```
int v1;
double v2;
v1=123;
v2=3.1415;
```

A linguagem Java tem oito *tipos primitivos*:

1. byte
2. short
3. int
4. long
5. char
6. float
7. double
8. boolean

Toda variável na linguagem Java terá a necessidade de dizermos o tipo.

ao manipular uma variável altera-se apenas o valor de atribuição

#### Métodos

`TipoRetorno NomeObjetivoNoinfinitivo Parametro (s)`

Ex: `int somar (int numeroUm, int numero2)` dois parâmetros.

* Os métodos na linguagem Java costumam ser aplicados no infinitivo.
* Todo método tem os seus parâmetros e um método pode receber parâmetros de tipos diferentes.

 String primeiroNome = "nome"

String segundoNome = "segundo nome"



`String nomeComplet = nomecompleto (primeiroNome, segundoNome)`

O valor desta variável é  a chamada de um método que também tem o mesmo nome.

#### Identação 

É o espaçamento aplicado no início das linhas de código que ajuda a manter uma hierarquia visual. Na maioria das linguagens esse não é um elemento que impede o código de ser compilado, mas manter o código **indentado** é fundamental para facilitar sua leitura, boas práticas de desenvolvimento.

## Mapa de atalhos

A classe precisa ter um método principal, denominamos esse método de Main que irá ter uma característica única na sua representação de inicialização, com isso, ele precisa seguir um padrão.

| Main, subentende que é o método main.         | main = public static void main(String[] args) { |
| :-------------------------------------------- | :---------------------------------------------: |
| Sout: comando de impressão na linguagem Java. |       System.out.println("hello  world");       |
|                                               |                                                 |
|                                               |                                                 |







