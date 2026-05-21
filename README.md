[![NPM](https://img.shields.io/npm/l/react)](https://github.com/RMFurlan/furshop/blob/main/LICENSE) 

# Sobre o projeto

Este é um projeto de back-end web desenvolvido como parte do curso **Java Completo**, sob orientação do Prof. Nelio Alves da DevSuperior.

A aplicação consiste em um sistema de Web Services robusto construído com Spring Boot e persistência de dados utilizando JPA e Hibernate. O objetivo principal do projeto foi consolidar as boas práticas de desenvolvimento backend, o que inclui a implementação de um modelo de domínio, estruturação de camadas lógicas, povoamento automatizado de banco de dados e tratamento detalhado de exceções HTTP.

## Modelo Conceitual
![Modelo Conceitual](https://github-production-user-asset-6210df.s3.amazonaws.com/13802711/594815518-2ee9fffd-cad5-418e-b906-86fbd61c9b8c.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20260519%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20260519T150240Z&X-Amz-Expires=300&X-Amz-Signature=0297d69764df02d45519215419cacffd0d0b519d356fa5bc02d8f98382568185&X-Amz-SignedHeaders=host&response-content-type=image%2Fpng)

### Entidades do Sistema:
* **User**: Cadastro de usuários/clientes do sistema.
* **Order**: Registro dos pedidos realizados pelos usuários.
* **OrderItem**: Tabela associativa que gerencia a relação de muitos para muitos entre produtos e pedidos, contendo atributos extras como quantidade e preço histórico do item.
* **Product**: Catálogo de produtos cadastrados.
* **Category**: Categorias para agrupamento dos produtos.
* **Payment**: Gerenciamento do estado e momento do pagamento dos pedidos.

## Arquitetura em Camadas Lógicas

![Camadas Lógicas](https://github-production-user-asset-6210df.s3.amazonaws.com/13802711/596039413-87b85be2-45cb-4e78-b5a2-b22cd025e79e.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20260521%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20260521T104627Z&X-Amz-Expires=300&X-Amz-Signature=05dc88d5d28f7d542233cda0c773b628b852616f6fffb3ba353e22aa0608922e&X-Amz-SignedHeaders=host&response-content-type=image%2Fpng)

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
