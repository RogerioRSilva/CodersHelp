# SOLID

↩️ Retornar para guia

SOLID é um acrônimo que descreve cinco princípios fundamentais para o design de software orientado a objetos. Esses princípios ajudam a criar sistemas mais robustos, flexíveis e fáceis de manter. Vamos aos conceitos:

1. **Single Responsibility Principle (SRP)**
Cada classe deve ter uma única responsabilidade ou motivo para mudar. Isso significa que uma classe deve fazer apenas uma coisa.

* **Exemplo:** Uma classe User que apenas gerencia dados de usuário, enquanto a classe UserService gerencia operações de serviço para o usuário.

2. **Open/Closed Principle (OCP)**
Os componentes de software devem ser abertos para extensão, mas fechados para modificação. Em outras palavras, devemos ser capazes de adicionar novas funcionalidades sem alterar o código existente.

* **Exemplo:** Usar interfaces e classes abstratas que permitem a criação de novas implementações sem alterar as já existentes.

3. **Liskov Substitution Principle (LSP)**
Objetos de uma classe base devem poder ser substituídos por objetos de uma classe derivada sem alterar o correto funcionamento do programa.

* **Exemplo:** Se temos uma classe base Bird com um método fly, todas as subclasses (como Sparrow ou Eagle) devem implementar fly de tal forma que se comportem como um pássaro.

4. **Interface Segregation Principle (ISP)**
Os clientes não devem ser forçados a depender de interfaces que eles não utilizam. Em vez de uma interface grande, várias interfaces pequenas e específicas são preferíveis.

* **Exemplo:** Em vez de uma interface genérica Machine com métodos print, scan, fax, usar interfaces específicas como Printable, Scannable, Faxable.

5. **Dependency Inversion Principle (DIP)**
Depender de abstrações, e não de implementações. Módulos de alto nível não devem depender de módulos de baixo nível, mas sim de abstrações.

* **Exemplo:** Em vez de uma classe EmailService depender diretamente de uma classe SmtpClient, ela deve depender de uma interface IEmailClient, permitindo o uso de diferentes implementações de clientes de e-mail.

Esses princípios ajudam a criar um código mais modular, flexível e escalável. Em suma, aplicar SOLID torna o desenvolvimento de software mais eficiente e o sistema mais fácil de manter e evoluir. 