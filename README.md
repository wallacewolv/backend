# plann.er

**plann.er** é uma aplicação backend desenvolvida com Node.js, Fastify e Prisma, destinada a facilitar a criação de viagens e a adição de grupos de amigos.

## Tecnologias Utilizadas

- **Node.js (v20.15)**: Ambiente de execução JavaScript server-side.
- **Fastify**: Framework web rápido e leve para Node.js.
- **Prisma**: ORM para Node.js e TypeScript, utilizando SQLite como banco de dados.

## Funcionalidades

- **Criação de Viagens**: Permite aos usuários criar e gerenciar viagens.
- **Grupos de Amigos**: Permite aos usuários adicionar amigos e organizar viagens em grupos.

## Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:

- Você instalou a versão 20.15 do `Node.js` e `npm`.

## Instalação

Siga os passos abaixo para configurar o projeto localmente:

1. Clone o repositório:

    ```bash
    git clone https://github.com/wallacewolv/backend.git
    ```

2. Navegue até o diretório do projeto:

    ```bash
    cd backend
    ```

3. Instale as dependências:

    ```bash
    npm install
    ```

4. Configure as variáveis de ambiente:

    Crie um arquivo `.env` na raiz do projeto e adicione as configurações necessárias para o seu banco de dados e outras chaves de API.

    ```plaintext
    DATABASE_URL="file:./dev.db"
    ```

5. Execute as migrações do banco de dados:

    ```bash
    npx prisma migrate dev --name init
    ```

## Uso

Para iniciar o servidor de desenvolvimento, execute:

```bash
npm run dev
