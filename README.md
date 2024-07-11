# plann.er
<!-- [![Portuguese](https://cdn.countryflags.com/thumbs/brazil/flag-round-250.png)](README.md#português) [![English](https://cdn.countryflags.com/thumbs/united-states-of-america/flag-round-250.png)](README.md#english) -->

## Índice

- [Português](#português)
  - [Tecnologias Utilizadas](#tecnologias-utilizadas)
  - [Funcionalidades](#funcionalidades)
  - [Pré-requisitos](#pré-requisitos)
  - [Instalação](#instalação)
  - [Uso](#uso)
  <!-- - [Licença](#licença)
  - [Contato](#contato) -->
- [English](#english)
  - [Technologies Used](#technologies-used)
  - [Features](#features)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
  <!-- - [License](#license)
  - [Contact](#contact) -->

---

# Português

**plann.er** é uma aplicação backend desenvolvida com Node.js, Fastify e Prisma, destinada a facilitar a criação de viagens e a adição de grupos de amigos.

## Tecnologias Utilizadas

- **Node.js (v20.15)**: Ambiente de execução JavaScript server-side.
- **Fastify**: Framework web rápido e leve para Node.js.
- **Prisma**: ORM para Node.js e TypeScript, utilizando SQLite como banco de dados.

## Funcionalidades

- **Confirmar participação** ***(Método GET)***: 
    - params: participantId
- **Confirmar viagem** ***(Método GET)***: 
    - params: tripId
- **Criar atividade** ***(Método POST)***: 
    - params: tripId
    - body: title e occurs_at
- **Criar convite** ***(Método POST)***: 
    - params: tripId
    - body: email
- **Criar link** ***(Método POST)***: 
    - params: tripId
  - body: title e url
- **Criar viagem** ***(Método POST)***: 
    - params: tripId
    - body: destination, starts_at, ends_at, owner_name, owner_email e emails_to_invite
- **Obter atividades** ***(Método GET)***: 
    - params: tripId
- **Obter links** ***(Método GET)***: 
    - params: tripId
- **Obter participante** ***(Método GET)***: 
    - params: participantId
- **Obter participantes** ***(Método GET)***: 
    - params: tripId
- **Obter detalhes da viagem** ***(Método GET)***: 
    - params: tripId
- **Atualizar viagem** ***(Método PUT)***: 
    - params: tripId
    - body: destination, starts_at e ends_at

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
    cd plann.er
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
```
#
# English

**plann.er** is a backend application developed with Node.js, Fastify, and Prisma, aimed at facilitating the creation of trips and the addition of friend groups.

## Technologies Used

- **Node.js (v20.15)**:  Server-side JavaScript runtime environment.
- **Fastify**: Fast and lightweight web framework for Node.js.
- **Prisma**: ORM for Node.js and TypeScript, using SQLite as the database.

## Features

- **Confirm participant** ***(Method GET)***: 
    - params: participantId
- **Confirm trip** ***(Method GET)***: 
    - params: tripId
- **Create activity** ***(Method POST)***: 
    - params: tripId
    - body: title e occurs_at
- **Create invite** ***(Method POST)***: 
    - params: tripId
    - body: email
- **Create link** ***(Method POST)***: 
    - params: tripId
  - body: title e url
- **Create trip** ***(Method POST)***: 
    - params: tripId
    - body: destination, starts_at, ends_at, owner_name, owner_email e emails_to_invite
- **Get activities** ***(Method GET)***: 
    - params: tripId
- **Get links** ***(Method GET)***: 
    - params: tripId
- **Get participant** ***(Method GET)***: 
    - params: participantId
- **Get participants** ***(Method GET)***: 
    - params: tripId
- **Get trip details** ***(Method GET)***: 
    - params: tripId
- **Update trip** ***(Method PUT)***: 
    - params: tripId
    - body: destination, starts_at e ends_at

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed the version 20.15 of `Node.js` and `npm`.

## Installation

Follow the steps below to set up the project locally:

1. Clone the repository:

    ```bash
    git clone https://github.com/wallacewolv/backend.git
    ```

2. Navigate to the project directory:

    ```bash
    cd plann.er
    ```

3. Install the dependencies:

    ```bash
    npm install
    ```

4. Configure the environment variables:

    Create a `.env` file in the root of the project and add the necessary configurations for your database and other API keys.

    ```plaintext
    DATABASE_URL="file:./dev.db"
    ```

5. Run the database migrations:

    ```bash
    npx prisma migrate dev --name init
    ```

## Usage

To start the development server, run:

```bash
npm run dev
