# KISS - "Keep It Simple, Stupid"

↩️ Retornar para guia

KISS é um acrônimo para "Keep It Simple, Stupid" (ou "Mantenha Simples, Estúpido" em português). É um princípio de design que enfatiza a simplicidade como um objetivo principal, ou seja, os sistemas funcionam melhor quando são mantidos simples ao invés de complicados. Aqui estão os pontos principais desse conceito no desenvolvimento de software:

* **Facilidade de Manutenção:** Código simples é mais fácil de manter, depurar e modificar.

* **Leitura e Compreensão:** Programadores, especialmente os novatos, conseguem ler e entender o código mais rapidamente.

* **Redução de Erros:** Sistemas complexos tendem a ter mais bugs e problemas.

* **Eficiência:** Simplicidade pode melhorar a eficiência do código, tornando-o mais rápido e menos propenso a falhas.

A ideia é evitar desnecessárias complexidades e complicações, focando sempre em soluções diretas e claras. É uma filosofia que valoriza a clareza e eficiência no desenvolvimento de software.

## Complexo (Não KISS):
Aqui está uma versão mais complicada que envolve loops e funções desnecessárias:

~~~~python
    def add_numbers():
        numbers = []
        for i in range(1, 11):
            numbers.append(i)
        
        sum = 0
        for number in numbers:
            sum += number
        
        return sum

    result = add_numbers()
    print("A soma é:", result)
~~~~


## Simples (KISS):
Agora, uma versão muito mais simples e direta:
~~~~python
    soma = sum(range(1, 11))
    print("A soma é:", soma)
~~~~

### Explicação:
* **Complexo:** A primeira abordagem cria uma lista de números, faz dois loops e usa uma função extra. Isso torna o código mais longo e difícil de entender.

* **Simples:** A segunda abordagem usa a função sum() diretamente sobre um range(). É mais conciso, fácil de ler e entender.

Menos é mais. Manter as coisas simples facilita a manutenção e compreensão do código.

> Está com dúvidas sobre python confira [Logica de Programação Python](../Python/logica_programacao_python.md)