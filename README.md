# Sistema de Reservas de Hotel

Este é um projeto simples em Java que simula um sistema de gerenciamento de reservas de hotel via console. O objetivo principal do projeto é demonstrar o uso de **Tratamento de Exceções** (Exception Handling), com foco na criação e implementação de **Exceções Personalizadas** (Custom Exceptions) para validar regras de negócio.

## 📋 Funcionalidades

* **Criação de Reserva:** Permite inserir número do quarto, data de check-in e data de check-out.
* **Atualização de Reserva:** Permite atualizar as datas de uma reserva existente.
* **Cálculo de Duração:** Calcula automaticamente a quantidade de noites entre o check-in e check-out.
* **Validação de Regras de Negócio (Domain Rules):**
    * A data de check-out não pode ser anterior à data de check-in.
    * Para atualizações, as datas devem ser futuras (não é permitido reservar datas passadas).

## 🛠️ Tecnologias e Conceitos

* **Java** (JDK)
* **POO** (Programação Orientada a Objetos)
* **Tratamento de Exceções:** Blocos `try-catch`.
* **Custom Exceptions:** Uso da classe `DomainException` (estendendo `RuntimeException`) para erros específicos do domínio.
* **Manipulação de Datas:** Uso de `Date`, `SimpleDateFormat` e `TimeUnit`.

## 📂 Estrutura do Projeto

O projeto está organizado em pacotes seguindo o padrão MVC (Model-View-Controller) simplificado:

* `application`
    * `Program.java`: Classe principal com o método `main`, responsável pela interação com o usuário.
* `model`
    * `entities`
        * `Reservation.java`: Classe de entidade contendo os dados da reserva e a lógica de validação de datas.
    * `exceptions`
        * `DomainException.java`: Exceção personalizada para capturar erros de regra de negócio.

## 👤 Autor

**Gustavo Canzi**

* **LinkedIn:** [https://www.linkedin.com/in/gustavo-canzi](https://www.linkedin.com/in/gustavo-canzi)
* **Email:** [gustavo.canzi@gmail.com](mailto:gustavo.canzi@gmail.com)