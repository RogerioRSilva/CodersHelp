# Lógica de programação em JAVA


## Tipos de Dados

- **byte:** Um inteiro de 8 bits. Intervalo: -128 a 127.

- **short:** Um inteiro de 16 bits. Intervalo: -32.768 a 32.767.

- **int:** Um inteiro de 32 bits. Intervalo: -2.147.483.648 a 2.147.483.647.

- **long:** Um inteiro de 64 bits. Intervalo: -9.223.372.036.854.775.808 a 9.223.372.036.854.775.807.

- **float:** Um ponto flutuante de 32 bits.

- **double:** Um ponto flutuante de 64 bits.

- **boolean:** Representa valores lógicos: true ou false.

- **char:** Um caractere Unicode de 16 bits. Intervalo: '\u0000' a '\uffff'.

### Exemplo de código

~~~java
        // Tipos Numéricos INTEIROS
		byte anosDeEmpresa = 23;
		short numeroDeVoos = 542;
		int id = 567;
		long pontosAcumulados = 3_234_845_223L; //com L na frente demonstra que ele é literal ou seja acima do valor de capacidade.
		
		// Tipos numéricos FLOAT
		float salario = 11_445.44F; // tem que ser colocado a letra F no final demonstra que ele é litral.
		double vendasAcumuladas = 2_991_797_103.01;
		
		// Tipos boleanos
		boolean estaDeFerias = false; //true
		
		// Tipos Caracter
		char status = 'A'; // Ativo  somente um caracter porem em listagem unicode pode ser feito assim '\u0010'

~~~

- **Tipo String:**
    - **Características:**
        - Imutável: Uma vez criada, a string não pode ser alterada. Qualquer operação que pareça modificar uma string, na verdade, cria uma nova string.

        - Classe Final: String é uma classe final, o que significa que não pode ser estendida (herdada).

        - Conveniente: A classe String oferece muitos métodos convenientes para manipular cadeias de caracteres, como substring(), toUpperCase(), toLowerCase(), trim(), entre outros.

        ### Exemplo de código

        ~~~java
            String s1 = "Olá Mundo";
            String s2 = new String("Olá Mundo");
        ~~~

        - **Pool de Strings:**
        O Java mantém um pool de strings para otimizar o uso de memória. Quando você cria uma string literal, ela é armazenada no pool e reutilizada se uma string com o mesmo valor for criada novamente.
    
    - **Principais Métodos:**
        - **charAt(int index):** Retorna o caractere no índice especificado.

        - **length():** Retorna o comprimento da string.

        - **substring(int beginIndex, int endIndex):** Retorna uma substring da string original.

        - **equals(Object anObject):** Compara duas strings para igualdade.

        - **compareTo(String anotherString):** Compara duas strings lexicograficamente.

        - **concat(String str):** Concatena duas strings

        ### Exemplo de código

        ~~~java    
            String texto = "Olá Mundo";

            // Imprimir comprimento
            System.out.println("Comprimento: " + texto.length());

            // Imprimir caractere no índice 1
            System.out.println("Caractere no índice 1: " + texto.charAt(1));

            // Imprimir substring
            System.out.println("Substring (0, 4): " + texto.substring(0, 4));

            // Converter para maiúsculas
            System.out.println("Maiúsculas: " + texto.toUpperCase());

            // Comparar strings
            System.out.println("Comparação: " + texto.equals("Olá Mundo"));
        ~~~

<br>

## Operadores Aritméticos:

- **Adição ( + ):** Soma dois valores.
~~~java
    int a = 5 + 3;  // a = 8
~~~

- **Subtração ( - ):** Subtrai um valor de outro.
~~~java
    int b = 5 - 3;  // b = 2
~~~

- **Multiplicação ( * ):** Multiplica dois valores.
~~~java
    int c = 5 * 3;  // c = 15
~~~

- **Divisão (/):** Divide um valor por outro.
~~~java
    int d = 9 / 3;  // d = 3
~~~

- **Módulo (%):** Retorna o resto da divisão entre dois valores.
~~~java
int e = 9 % 4;  // e = 1
int f = 10 % 2; // f = 0
~~~

<br>

## Operadores Lógicos

- **E lógico ( && ):** Retorna true se ambas as expressões forem verdadeiras.
~~~java
    boolean a = true && false;  // a = false
~~~

- **OU lógico ( || ):** Retorna true se pelo menos uma das expressões for verdadeira.
~~~java
    boolean b = true || false;  // b = true
~~~

- **NÃO lógico ( ! ) : **Inverte o valor lógico de uma expressão.
~~~~java
    boolean c = !true;  // c = false
~~~~

- **E lógico bit a bit ( & ):** Retorna true se ambas as expressões forem verdadeiras, mas verifica ambas as condições, mesmo que a primeira seja false.
~~~~java
    boolean d = true & false;  // d = false
~~~~

- **OU lógico bit a bit ( | ):** Retorna true se pelo menos uma das expressões for verdadeira, mas verifica ambas as condições.
~~~~java
    boolean e = true | false;  // e = true
~~~~

- **OU exclusivo lógico bit a bit ( ^ ):** Retorna true se uma e apenas uma das expressões for verdadeira.
~~~~java
    boolean f = true ^ false;  // f = true
~~~~

<br>

## Estruturas Condicionais

- **if-else:** Permite executar diferentes blocos de código com base em uma condição.
~~~~java
    if (condition) {
        // código se condição for verdadeira
    } else {
        // código se condição for falsa
    }

~~~~

- **else if:** Permite verificar múltiplas condições.
~~~~java
    if (condition1) {
        // código se condition1 for verdadeira
    } else if (condition2) {
        // código se condition2 for verdadeira
    } else {
        // código se todas as condições forem falsas
    }
~~~~

- **Operador Ternário:** O operador ternário em Java é uma forma compacta de escrever uma expressão condicional, e tem a seguinte sintaxe:
~~~~java
    variavel = (condição) ? valorSeVerdadeiro : valorSeFalso;
~~~~

- **switch:** Escolhe entre múltiplas opções.
~~~~java
    switch (variable) {
        case 1:
            // código para caso 1
            break;
        case 2:
            // código para caso 2
            break;
        default:
            // código para caso padrão
    }
~~~~

<br>

## Estuturas de Repetição (Loops)

- **for:** Repete um bloco de código um número específico de vezes.
~~~~java
    for (int i = 0; i < 10; i++) {
        // código a ser executado
    }
~~~~

- **while:** Repete um bloco de código enquanto uma condição é verdadeira.
~~~~java
    while (condition) {
        // código a ser executado
    }
~~~~

- **do-while:** Semelhante ao while, mas garante que o bloco de código seja executado pelo menos uma vez.
~~~~java
    do {
        // código a ser executado
    } while (condition);
~~~~

<br>

## Estruturas de Controle de Fluxo

- **break:** Interrompe um loop ou switch.
~~~~java
    for (int i = 0; i < 10; i++) {
        if (i == 5) {
            break;
        }
    }   
~~~~

- **continue:** Passa para a próxima iteração do loop.
~~~~java
    for (int i = 0; i < 10; i++) {
        if (i % 2 == 0) {
            continue;
        }
        // código para números ímpares
    }
~~~~

- **return:** Sai de um método e retorna um valor, se especificado.
~~~~java
    public int sum(int a, int b) {
        return a + b;
    }
~~~~

<br>

## Vetores

- **Array Unidimensional:** Um vetor simples que contém elementos de um único tipo.
~~~~java
    int[] numeros = {1, 2, 3, 4, 5};
~~~~

- **Array Bidimensional:** Uma matriz que contém elementos em linhas e colunas.
~~~~java
    int[][] matriz = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9}
    };
~~~~

- **ArrayList:** Além de arrays, Java oferece a classe ArrayList que faz parte do framework Collections e fornece uma maneira dinâmica de trabalhar com listas de elementos.
~~~~java
    import java.util.ArrayList;

    ArrayList<String> lista = new ArrayList<>();
    lista.add("Elemento 1");
    lista.add("Elemento 2");

~~~~

- **LinkedList:** Outra alternativa é a classe LinkedList, que também faz parte do framework Collections e é útil para listas onde a inserção e remoção de elementos são frequentes.
~~~~java
    import java.util.LinkedList;

    LinkedList<String> listaEncadeada = new LinkedList<>();
    listaEncadeada.add("Elemento 1");
    listaEncadeada.add("Elemento 2");

~~~~

Cada tipo tem suas vantagens dependendo do caso de uso. Arrays são fixos em tamanho, enquanto ArrayList e LinkedList podem crescer dinamicamente.

