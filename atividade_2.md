# Sintaxe e programação em C#

Nessa atividade, será abordado conceitos básicos de programação em C#. Esses pontos são importantes para que possamos programar APIs em .NET Core.

A sintaxe de C# é semelhante a C, C++ e Java. No entanto, existem algumas diferenças.

## 1. Hello World em C#

O trecho do vídeo a seguir (a partir de 13:00) fala sobre as estruturas básicas utilizadas em um código C# e como fazer um "Hello World":

https://www.youtube.com/watch?v=dVzJ3bx68FA&t=780s

Obs: Será necessário usar o compilador de C#. Ele é acessível no Windows como `csc.exe`. No Ubuntu/Debian, é possível instalá-lo usando o comando `sudo apt install mono-csc`.

## 2. Tipos de dados

Os tipos são int, float, char, string e byte (inteiros positivos pequenos de 0 a 255). A declaração dessas variáveis ocorre do mesmo jeito que é feito em C:

```cs
int numero = -2345939;
char letra = 'q';
float valor = 222.4f;
string nome = "eccjr";
byte state = 42;
```

Obs: aspas simples `'` indicam valores do tipo char e aspas duplas `"` indicam valores do tipo string. Inverter os tipos causará um erro.

Vetores são declarados usando o operador `[]` após o tipo da sua declaração e os vetores são definidos entre chaves `{}`:

```cs
int[] numeros = {2, 4, 6, 8};
char[] vogais = {'a', 'e', 'i', 'o', 'u'};
```

## 2. Estruturas de controle

As estruturas de controle (if, else, switch) e de repetição (for, while, do while) são exatamente as mesmas de C, com a mesma sintaxe.

O foreach é uma estrutra semelhante ao for comum, porém com uma diferença na sintaxe que o torna mais prático. O vídeo a seguir explica a sintaxe da estrutura foreach:

https://www.youtube.com/watch?v=n3Ns1_F7yUo&list=PLx4x_zx8csUglgKTmgfVFEhWWBQCasNGi&index=24

## 3. Métodos e classes

Os métodos são definidos da mesma forma que em C, com a diferença de que pode-se usar a palavras reservada static antes do tipo do método, que significa que esse método pertence a classe principal do programa e não a uma outra classe.

Esse vídeo exemplifica conceitos de orientação à objetos em C#:

https://www.youtube.com/watch?v=dARHRw1d0qI

## 4. Interfaces

Interfaces representam tipos de dados utilizados na programação orientada à objetos. São como classes abstratas que só podem conter propriedades e métodos vazios.

Esse vídeo explica o que são interfaces e como implementá-las em C#:

https://www.youtube.com/watch?v=NSjz4HS7bPU

## Links úteis

Documentação do C# (repleta de tutoriais): https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/

W3 Schools sobre C# (muito didático e fácil de encontrar o que procura): https://www.w3schools.com/cs
