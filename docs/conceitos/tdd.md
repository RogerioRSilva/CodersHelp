# Test-Driven Development (TDD)

↩️ Retornar para guia

TDD, ou Desenvolvimento Guiado por Testes, é uma abordagem de desenvolvimento de software na qual os testes são escritos antes do código que os satisfará. O objetivo é garantir que cada parte do código seja testada desde o início. O ciclo TDD segue três etapas principais: Red, Green, Refactor.

## Etapas do Ciclo TDD

1. **Red (Vermelho):**

    * Escreva um teste para a próxima funcionalidade que deseja adicionar.

    * Execute o teste e observe que ele falha (porque o código que satisfaz o teste ainda não foi escrito).

2. **Green (Verde):**

    * Escreva o código mínimo necessário para passar no teste.

    * Execute todos os testes e observe que agora eles passam.

3. **Refactor (Refatorar):**

    * Refatore o código para melhorar sua estrutura e qualidade, sem alterar seu comportamento externo.

    * Execute todos os testes novamente para garantir que eles ainda passam após a refatoração.

## Benefícios do TDD

* **Qualidade do Código:** Produz código mais limpo e bem estruturado.

* **Confiança:** Permite que os desenvolvedores alterem e adicionem funcionalidades com mais segurança, pois sabem que os testes garantirão que nada foi quebrado.

* **Documentação:** Os testes servem como uma documentação executável das funcionalidades do sistema.

* **Design:** Força os desenvolvedores a pensarem no design e comportamento do software antes de escrever o código real.


## Exemplo de TDD em Python

Aqui está um exemplo simples de TDD em Python usando o módulo unittest:

~~~~python
    import unittest

    # Teste (Red)
    class TestSoma(unittest.TestCase):
        def test_soma(self):
            self.assertEqual(soma(1, 2), 3)

    # Código (Green)
    def soma(a, b):
        return a + b

    if __name__ == '__main__':
        unittest.main()

    # Refatoração (Refactor)
    # Nenhuma refatoração necessária neste exemplo simples
~~~~

## Conclusão

O TDD não apenas melhora a qualidade do software, mas também reduz o ciclo de desenvolvimento ao detectar erros precocemente e proporcionar uma base de código mais sólida. Adotar TDD pode parecer trabalhoso inicialmente, mas os benefícios a longo prazo valem o esforço.