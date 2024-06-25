
# API RESTful com Java 22, Spring Boot 3 e Railway

Este projeto de API RESTful construído com Java 22 pela plataforma de ensino da DIO. Este repositório exemplifica o uso das tecnologias mais recentes para criar uma API robusta, escalável e fácil de manter.

# Diagrama De Classes
```mermaid

 classDiagram
    User "1" *-- "1" Account
    User "1" *-- "N" Feature
    User "1" *-- "1" Card
    User "1" *-- "N" News

    class User {
        +String name
        +Account account
        +List~Feature~ features
        +Card card
        +List~News~ news
    }

    class Account {
        +String Number
        +String Agency
        +Number Balance
        +Number Limit
    }

    class Feature {
        +String Icon
        +String description
    }

    class Card {
        +String Number
        +Number Limit
    }

    class News {
        +String Icon
        +String Description
    }

```

# Tecnologias Utilizadas
* Java 22: A versão LTS mais recente, com novos recursos e melhorias.

* Spring Boot 3: Framework que facilita a configuração e inicialização de aplicações.

* Spring Data JPA: Simplifica a interação com bancos de dados relacionais.

* OpenAPI (Swagger): Ferramenta para documentação de APIs RESTful.

* Railway: Plataforma de deploy simplificada na nuvem.
