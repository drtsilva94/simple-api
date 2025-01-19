# Simple API

Este projeto é uma API REST desenvolvida utilizando **Spring Boot 3** e **Java 17** com persistência de dados em um banco de dados H2 em memória. A aplicação foi implantada no Railway para facilitar o acesso e o uso.

## Funcionalidades

- CRUD de produtos:
  - Adicionar produtos.
  - Listar todos os produtos.
  - Atualizar informações de um produto.
  - Excluir produtos.
- Persistência de dados utilizando **Spring Data JPA**.
- Banco de dados em memória H2 acessível via console.
- API documentada seguindo boas práticas REST.

## Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **Banco de Dados H2**
- **Railway** (deploy)

## Como Executar o Projeto Localmente

1. Clone este repositório:

   ```bash
   git clone https://github.com/drtsilva94/simple-api.git
   ```

2. Acesse o diretório do projeto:

   ```bash
   cd simple-api
   ```

3. Execute o projeto utilizando Maven:

   ```bash
   ./mvnw spring-boot:run
   ```

4. Acesse o console do banco de dados H2 em:

   ```plaintext
   http://localhost:8080/h2-console
   ```
   - **JDBC URL:** `jdbc:h2:mem:taskdb`
   - **Username:** `sa`
   - **Password:** *(deixe vazio)*

5. Use ferramentas como **Postman** ou **cURL** para testar os endpoints da API.

## Endpoints Disponíveis

| Método | Endpoint        | Descrição                     |
|--------|-----------------|-------------------------------|
| GET    | `/produtos`     | Lista todos os produtos.      |
| GET    | `/produtos/{id}`| Retorna um produto pelo ID.   |
| POST   | `/produtos`     | Adiciona um novo produto.     |
| PUT    | `/produtos/{id}`| Atualiza um produto existente.|
| DELETE | `/produtos/{id}`| Remove um produto pelo ID.    |

## Como Acessar a Aplicação Implantada

A aplicação foi implantada no **Railway** e está acessível através do seguinte domínio público:

[**Simple API no Railway**](https://simple-api-production-61ac.up.railway.app)

## Estrutura do Projeto

O projeto segue a arquitetura MVC:
- **Model**: Representa as entidades de dados.
- **Repository**: Responsável por interações com o banco de dados.
- **Controller**: Define os endpoints da API.
- **Service**: Contém a lógica de negócio.

## Como Contribuir

1. Faça um fork do repositório.
2. Crie uma nova branch para sua feature:

   ```bash
   git checkout -b minha-feature
   ```

3. Realize as alterações e faça um commit:

   ```bash
   git commit -m "Adicionando minha feature"
   ```

4. Envie para o seu repositório forkado:

   ```bash
   git push origin minha-feature
   ```

5. Abra um Pull Request neste repositório.

## Contato

Desenvolvido por **Anna Duarte**. Você pode me encontrar no [LinkedIn](https://www.linkedin.com/in/anna-duarte).

---

**Nota:** Este projeto foi desenvolvido como parte do aprendizado no bootcamp **Santander Fullstack Developer** pela [Digital Innovation One](https://www.dio.me/).
