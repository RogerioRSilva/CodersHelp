# 🖥️ Lógica de programação em Python

↩️ [Retornar para guia](/README.md)


## 🎲 Tipos de Dados

### Tipos Primitivos:

1. **int:** Números inteiros.
    ~~~~python
        x = 10
    ~~~~
2. **float:** Números de ponto flutuante (decimais).
    ~~~~python
        y = 10.5
    ~~~~
3. **str:** Cadeias de caracteres (strings).
    ~~~~python
        texto = "Olá, Mundo!"
    ~~~~
4. **bool:** Valores booleanos, True ou False.
    ~~~~python
        verdadeiro = True
    ~~~~    

<br>

### Tipos Compostos:

1. **list:** Lista mutável de itens.
    ~~~~python
        lista = [1, 2, 3, "texto"]
    ~~~~   
2. **tuple:** Tupla imutável de itens.
    ~~~~python
        tupla = (1, 2, 3, "texto"
    ~~~~  
3. **dict:** Dicionário, uma coleção de pares chave-valor.
    ~~~~python
        dicionario = {"chave1": "valor1", "chave2": "valor2"}
    ~~~~  
4. **set:** Conjunto, uma coleção não ordenada de itens únicos.
    ~~~~python
        conjunto = {1, 2, 3}
    ~~~~   
5. **frozenset:** Conjunto imutável.
    ~~~~python
        conjunto_imutavel = frozenset([1, 2, 3])
    ~~~~   

<br>

### Outros Tipos:

1. **bytes:** Sequência de bytes.
    * Imutável: Uma sequência de bytes que não pode ser alterada após a criação.
    * Uso: Ideal para armazenar dados binários que não precisam ser modificados.
    ~~~~python
        dados_bytes = b"exemplo"
    ~~~~  
2. **bytearray:** Sequência mutável de bytes.
    * Mutável: Semelhante a bytes, mas os dados podem ser modificados após a criação.

    * Uso: Útil quando você precisa alterar os dados binários.
    ~~~~python
        dados_bytearray = bytearray(5)
    ~~~~  
3. **None:** Representa a ausência de valor ou tipo nulo.
    ~~~~python
        nenhum_valor = None
    ~~~~  

<br>

## 🧮 Operadores Aritméticos:

1. **Adição ( + ):** Soma dois valores.
    ~~~~python
        x = 5 + 3  # x = 8
    ~~~~

2. **Subtração ( - ):** Subtrai um valor de outro.
    ~~~~python
        y = 5 - 3  # y = 2
    ~~~~

3. **Multiplicação ( * ):** Multiplica dois valores.
    ~~~~python
        z = 5 * 3  # z = 15
    ~~~~

4. **Divisão ( / ):** Divide um valor por outro, sempre retornando um número de ponto flutuante.
    ~~~~python
        w = 9 / 3  # w = 3.0
    ~~~~

5. **Divisão Inteira ( // ):** Divide dois valores, retornando um inteiro.
    ~~~~python
        a = 9 // 2  # a = 4
    ~~~~

6. **Módulo ( % ):** Retorna o resto da divisão entre dois valores.
    ~~~~python
        b = 9 % 2  # b = 1
    ~~~~

7. **Exponenciação ( ** ):** Eleva um valor à potência de outro.
    ~~~~python
        c = 2 ** 3  # c = 8
    ~~~~

<br>

## ✅ Operadores Lógicos

1. **and:** Retorna True se ambas as expressões forem verdadeiras.
    ~~~~python
        a = True and False  # a = False
    ~~~~

2. **or:** Retorna True se pelo menos uma das expressões for verdadeira.
    ~~~~python
        b = True or False  # b = True
    ~~~~

3. **not:** Inverte o valor lógico de uma expressão.
    ~~~~python
        c = not True  # c = False
    ~~~~

### Operadores de comparação

1. Igualdade **( == )**.
    ~~~~python
        a = (5 == 5)  # a = True
    ~~~~

2. Diferença **( != )**.
    ~~~~python
        b = (5 != 3)  # b = True
    ~~~~

3. Maior que **( \> )**.
    ~~~~python
        c = (5 > 3)  # c = True
    ~~~~

4. Menor que **( \< )**.
    ~~~~python
        d = (5 < 3)  # d = False
    ~~~~

5. Maior ou igual a **( >= )**.
    ~~~~python
      e = (5 >= 3)  # e = True  
    ~~~~

6. Menor ou igual a **( <= )**.
    ~~~~python
        f = (5 <= 5)  # f = True
    ~~~~

<br>

## 🔎 Estruturas Condicionais

1. **if :** Permite executar um bloco de código se uma condição for verdadeira.
    ~~~~python
        if condição:
            # Código a ser executado se a condição for verdadeira
    ~~~~

2. **if - else:** Permite executar um bloco de código se a condição for verdadeira e outro bloco se a condição for falsa.
    ~~~~python
        if condição:
            # Código a ser executado se a condição for verdadeira
        else:
            # Código a ser executado se a condição for falsa
    ~~~~

3. **if - elif - else :** Permite testar múltiplas condições.
    ~~~~python
        if condição1:
            # Código a ser executado se condição1 for verdadeira
        elif condição2:
            # Código a ser executado se condição2 for verdadeira
        else:
            # Código a ser executado se todas as condições forem falsas
    ~~~~

### Exemplo de código: 

~~~~python
    idade = 20

    if idade < 18:
        print("Menor de idade")
    elif idade >= 18 and idade < 65:
        print("Adulto")
    else:
        print("Idoso")  
~~~~

4. **Operador Ternário:**
    ~~~~python
        resultado = "Menor de idade" if idade < 18 else "Maior de idade"
    ~~~~

    * **Exemplo de Código:**
    ~~~~python
        idade = 20
        mensagem = "Menor de idade" if idade < 18 else "Maior de idade"
        print(mensagem)  # Saída: Maior de idade
    ~~~~

<br>

## 🎡 Estuturas de Repetição (Loops)

1. **for:** Usado para iterar sobre uma sequência (como lista, tupla, string) ou qualquer outro objeto iterável.
    ~~~~python
        # Iterar sobre uma lista
        for item in [1, 2, 3, 4, 5]:
            print(item)

        # Iterar sobre uma string
        for char in "Python":
            print(char)
    ~~~~

2. **while:** Repete um bloco de código enquanto uma condição for verdadeira.
    ~~~~python
        contador = 0
        while contador < 5:
            print(contador)
            contador += 1
    ~~~~

3. **break e continue:** 
    * **break:** Interrompe a iteração do loop.
        ~~~~python
            for item in [1, 2, 3, 4, 5]:
            if item == 3:
                break
            print(item)  # Saída: 1, 2
        ~~~~
    * **continue:** Passa para a próxima iteração do loop, pulando o código restante no corpo do loop.
        ~~~~python
            for item in [1, 2, 3, 4, 5]:
            if item == 3:
                continue
            print(item)  # Saída: 1, 2, 4, 5
        ~~~~

4. **Loop com else:** Um bloco else pode ser associado a loops for ou while. O bloco else é executado quando o loop é concluído normalmente, ou seja, não é interrompido por um break.
    ~~~~python
        for item in [1, 2, 3]:
            print(item)
        else:
            print("Loop concluído.")
    ~~~~


