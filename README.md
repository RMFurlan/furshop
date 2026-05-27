[![MIT](https://img.shields.io/npm/l/react)](https://github.com/RMFurlan/furshop/blob/main/LICENSE) 

# Sobre o projeto

Este é um projeto de back-end web desenvolvido como parte do curso **Java Completo**, sob orientação do Prof. Nelio Alves da DevSuperior.

A aplicação consiste em um sistema de Web Services robusto construído com Spring Boot e persistência de dados utilizando JPA e Hibernate. O objetivo principal do projeto foi consolidar as boas práticas de desenvolvimento backend, o que inclui a implementação de um modelo de domínio, estruturação de camadas lógicas, povoamento automatizado de banco de dados e tratamento detalhado de exceções HTTP.

## Modelo Conceitual
![Modelo Conceitual](https://github.com/RMFurlan/furshop/blob/main/assets/modelo_conceitual.png)

### Entidades do Sistema:
* **User**: Cadastro de usuários/clientes do sistema.
* **Order**: Registro dos pedidos realizados pelos usuários.
* **OrderItem**: Tabela associativa que gerencia a relação de muitos para muitos entre produtos e pedidos, contendo atributos extras como quantidade e preço histórico do item.
* **Product**: Catálogo de produtos cadastrados.
* **Category**: Categorias para agrupamento dos produtos.
* **Payment**: Gerenciamento do estado e momento do pagamento dos pedidos.

## Arquitetura em Camadas Lógicas

![Camadas Lógicas](https://github.com/RMFurlan/furshop/blob/main/assets/camadas_logicas.png)

* **Resource Layer**: Controladores REST que expõem os endpoints da API.
* **Service Layer**: Onde residem as regras de negócio e orquestração do sistema.
* **Data Access Layer**: Repositórios JPA responsáveis pelas consultas e persistência no banco de dados.

# Tecnologias utilizadas
- Java
- Spring Boot
- JPA / Hibernate
- Maven
- Banco de dados: H2 Database (Ambiente de Testes) e PostgreSQL (Ambiente de Produção/Desenvolvimento)
- Postman (Para testes e validação das rotas e payloads HTTP)

# Autor

Rafael Medeiros Furlan

https://www.linkedin.com/in/rafael-medeiros-furlan-743954257/
