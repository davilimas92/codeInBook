# 🎬 Microserviço: Admin do Catálogo de Vídeos

Este repositório contém o código-fonte de um microserviço responsável por gerenciar o **Catálogo de Vídeos**, permitindo operações como adicionar, editar, remover e listar vídeos, além de gerenciar **categorias** e **gêneros**.

O microserviço foi desenvolvido com foco em escalabilidade, manutenção e boas práticas de engenharia de software, utilizando **Clean Architecture**, **DDD**, **TDD** e ferramentas modernas de desenvolvimento.

---

## 🏗️ Arquitetura

Este projeto segue os princípios da **Clean Architecture**, promovendo o desacoplamento entre camadas e garantindo que a lógica de negócio permaneça independente de frameworks, bancos de dados e interfaces externas.

### Camadas da Arquitetura:

- **Entidades**: Representam os objetos de domínio (ex.: `Vídeo`, `Categoria`, `Gênero`).
- **Use Cases**: Contêm a lógica de negócio principal (ex.: `AdicionarVídeoUseCase`, `EditarVídeoUseCase`).
- **Interfaces (Gateways)**: Definem contratos com repositórios, serviços externos e adaptadores.
- **Frameworks e Drivers**: Implementações específicas com bibliotecas/frameworks (ex.: Spring Boot, RabbitMQ, JPA).

---

## 🚀 Tecnologias Utilizadas

- **Java 17**: Linguagem principal da aplicação.
- **Spring Boot**: Framework para construção de APIs RESTful.
- **RabbitMQ**: Comunicação assíncrona com serviço de encoding de vídeos.
- **JPA (Hibernate)**: Mapeamento objeto-relacional e persistência de dados.
- **JUnit 5 / Mockito**: Testes unitários baseados em TDD.
- **Maven**: Gerenciador de dependências e build.

---

## 📦 Funcionalidades

- ✅ **Gerenciamento de Vídeos**  
  - Adicionar, editar, listar e excluir vídeos do catálogo.

- ✅ **Gerenciamento de Categorias e Gêneros**  
  - Criar, editar e associar categorias e gêneros a vídeos.

- ✅ **Integração com Encoder de Vídeos**  
  - Envio de vídeos para encoding via fila de mensagens (RabbitMQ).

- ✅ **API RESTful**  
  - Endpoints expostos para interação com o catálogo.

---

## 📁 Organização do Projeto

