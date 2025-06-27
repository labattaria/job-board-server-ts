**Read in another language: [Українська](README.ukr.md), [English](README.md).**

# Job Board typescript server

---

[![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)](#)
[![GraphQL](https://img.shields.io/badge/GraphQl-E10098?style=for-the-badge&logo=graphql&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)](#)
[![ApolloGraphQL](https://img.shields.io/badge/-ApolloGraphQL-311C87?style=for-the-badge&logo=apollo-graphql)](#)
[![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white)](#)
[![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)](#)
[![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)](#)

This is the Express/GraphQL/Apollo server from the [Job Board server](https://github.com/labattaria/job-board-server) repo, but migrated and converted to TypeScript

The server-side application was slightly refactored using TypeScript, which added type safety to the code

It uses the GraphQL TypeScript code generator, which allows us to generate TypeScript definitions from our GraphQL schema

The code generator also creates TypeScript types for our resolvers, making them more type-safe

This server is only part of the application, the second part (the client) is located at this repo: [Job Board typescript client](https://github.com/labattaria/job-board-client-ts)

The app in this repo is deployed at [https://render.com](https://render.com), hosting public URL: [https://job-board-server-ts.onrender.com/graphql](https://job-board-server-ts.onrender.com/graphql)

## Used dependencies:

- **TypeScript** - Language that builds on JavaScript by adding static types, helping developers catch errors early and write more reliable code
- **GraphQL Code Generator** - Tool that automatically generates TypeScript types (or other language types) and boilerplate code based on your GraphQL schema and operations
- **GraphQL** - Core GraphQL library
- **Apollo-server** - GraphQL server that works with any GraphQL schema
- **SQLite** - A lightweight, self-contained SQL database engine. It stores the entire database in a single file
- **JWT (JSON Web Token)** - A compact, URL-safe token format used for securely transmitting information between parties. Commonly used for authentication and authorization in web applications
- **Nodemon** - A development utility that automatically restarts your Node.js server when it detects file changes
- **Concurrently** - Node.js tool that lets you run multiple commands (scripts) at the same time in a single terminal

The full list of dependencies can be found in the **package.json** file.

---

## Contents

- [Installation](#installation)
- [Usage](#usage)

### Installation

1. Clone the repository:

```shell
git clone https://github.com/labattaria/job-board-server-ts.git
```

2. Install project dependencies:

```shell
cd job-board-server-ts
npm install
```

### Usage

Start the server using the following command:

```shell
npm start
```

This will start the server and also watch for changes in watch mode, generating outputs into the folder at the path src/generated/
Server will be located at **http://localhost:9000/graphql**
