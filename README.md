### 🚀 PostgreSQL com Docker Compose e Rede Externa Proxy

Este repositório contém a configuração para rodar o **PostgreSQL** em um contêiner Docker utilizando o **Docker Compose**. O projeto foi configurado para usar uma **rede externa chamada `proxy`**, permitindo que o contêiner PostgreSQL se conecte com outros serviços em uma rede isolada.

### 📦 Como Usar

- **Crie a rede externa `proxy`**:
   Antes de rodar o projeto, é necessário criar a rede externa que será usada pelos contêineres

   ```bash
   docker network create proxy
  ```


- Configure as credenciais do seu banco de dados PostgreSQL no arquivo `.env`

   ```bash
   POSTGRES_USER=myuser
   POSTGRES_PASSWORD=mypassword
   POSTGRES_DB=mydatabase

  ```

- Rode o comando para iniciar o contêiner PostgreSQL:

   ```bash
  docker-compose up -d
  ```
