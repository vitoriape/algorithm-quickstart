Conteúdos
=================
<!--ts-->
   * [Operadores](#operadores)
      * [Operadores Aritméticos](#operadores-aritméticos)
   * [Tipos Primitivos](#tipos-primitivos)
      * [Casting de Tipos Primitivos](#casting-de-tipos-primitivos)
   * [Classes](#classes)
      * [Objetos](#objetos)
      * [Atributos](#atributos)
      * [Métodos](#métodos)
   

---

#### Operadores

|    Tipo    	| Sinal 	| Exemplo 	  |
|:----------:	|:-----:	|:-------:	  |
| Atribuição 	|   `=`   	| `A = 100` 	  |
|    Igual   	|   `==`  	|  `A == B` 	  |
|  Diferente 	|   `!=`  	|  `A != B`	  |
|      Maior    |   `>`  	| `A > B` 	  |
| Maior ou Igual|  `>=`  	| `A >= B`	  |
|      Menor    |   `<`  	| `A < B`	  |
| Menor ou Igual|  `<=`  	| `A <= B`	  |
|        E      |  `&&`  	| `A > B && A < C`|
|       OU      | `\|\|` 	| `A = B \|\| A = C`|

>**Normalmente, os operadores `==` e `!=` só são usados para comparar variáveis de [tipos primitivos]((#tipos-primitivos)), mas é possível usá-los para saber se duas declarações (instâncias) estão apontando para o mesmo [objeto]()**

#### Operadores Aritméticos

|               	| Simples 	| Unitária - Mesmo Valor 	| Unitária - Valor Diferente 	|
|:-------------:	|:-------:	|:----------------------:	|:--------------------------:	|
|     Adição    	|    `+`    	|           `++`           	|             `+=`             	|
|   Subtração   	|    `-`    	|           `--`           	|             `-=`             	|
| Multiplicação 	|    `*`    	|                        	|             `*=`             	|
|    Divisão    	|    `/`    	|                        	|             `/=`             	|
|     Resto     	|    `%`    	|                        	|             `%=`             	|

---

💡 Os dados em Java são divididos em "dados por valor", que são os **tipos primitivos**, e em "dados por referência", chamados de **classes**.

### Tipos Primitivos
Variáveis de tipo primitivo armazenam somente um valor de seu tipo de cada vez, ou seja, assim que outro valor for atribuído a essa variáel, seu valor original é substituído. **Sempre são inicializadas com o valor `0` ou `false` no caso do tipo `boolean`**.

| Declaração 	|        Função       	               |      
|:----:	      |:-------------------:	               |
| char 	      | Armazena caracteres 	               | 
| int         | Armazena números inteiros            |
| short       | Armazena números inteiros de 16 bits |
| long        | Armazena números inteiros de 64 bits |
| float       | Armazena números decimais reais, ou seja, **números de ponto flutuante de maior extensão** com mais precisão. Caso o valor da variável seja do tipo `float` mas o programa interpretá-la como double, basta acrescentar `f` ao final do valor |
| double | Armazena números decimais reais, ou seja, **números de ponto flutuante de menor extensão** com mais precisão |
| byte | |
| boolean | Armazena valores booleanos/lógicos, ou seja, `true` e `false` |



- Exemplos
```java
char dadoChar = 'D';

int dadoInt = 5;

short dadoShort = 32767;

long dadoLong = 9223372036854775807L;

float dadoFloat = 6.5f;

double dadoDouble = 3.59;

byte dadoByte = 127;

boolean dadoBoolean = true;
```

---

#### Casting de Tipos Primitivos
Ato de apontar ao compilador uma **mudança** no tipo de variável de um valor, sempre tomando cuidado com a possível perda de dados. 

>**Valores do tipo `boolean` não aceitam casting**

- Declaração
```java
tipo variável = (tipo) valor;
```

- Exemplo
```java
// Casting double -> float
float Y = (float) 7.0;

// Conversão automática sem casting (int -> float)
float W = 100;

// Casting double -> int
int H = (int) 7.1987;

// Conversão automática sem casting (char -> int)
int A = 'A';
```

>**A _conversão_ ocorre sem a necessidade de _casting_ em alguns casos, como quando se adiciona uma variável de um tipo **menor** que o tipo que receberá esse valor**

---

### Classes
Armazenam as localizações de objetos na memória do computador, sendo que esses objetos podem conter várias variáveis.
**Sempre são inicializadas com o valor `null`**. Elas são "receitas" de um objeto, contendo características e comportamentos, permitindo assim armazenar propriedades e **métodos** dentro dela. 

>**Toda classe possui nome e status de visibilidade (`public`, `private`, `protected`)**

- Exemplo
```java
<modificador de acesso> class nomeClasse {

  // Local onde os objetos são criados e manipulados
  
  variável;
  método;

}
```

---

#### Objetos

Os objetos computacionais em Java são características definidas pelas classes, através dos quais é possível inicializar atributos e invocar métodos.

---

#### Atributos

Características de um objeto, conhecidas como variáveis.

---

#### Métodos

Ações que os objetos podem exercer quando solicitados.

---




