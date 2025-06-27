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

Це сервер Express/GraphQL/Apollo з [Job Board server](https://github.com/labattaria/job-board-server) репозиторію, але перенесений на TypeScript
Серверний застосунок був трохи відрефакторений із використанням TypeScript, що додало типобезпечність коду
Він використовує генератор коду GraphQL TypeScript, який дозволяє нам генерувати TypeScript-типи з нашої GraphQL-схеми
Генератор коду також створює TypeScript-типи для наших резолверів, роблячи їх більш типобезпечними

Цей сервер — лише частина додатку, друга частина (клієнтська) знаходиться в цьому репо: [Job Board typescript client](https://github.com/labattaria/job-board-client-ts)

Застосунок у цьому репозиторії розгорнуто за адресою: [https://render.com](https://render.com), за цією URL-адресою: [job-board-server-ts.onrender.com/graphql](job-board-server-ts.onrender.com/graphql)

## Залежностi, якi використовуються:

- **TypeScript** - Мова, що базується на JavaScript, додаючи статичні типи, допомагає розробникам раніше знаходити помилки та писати більш надійний код
- **GraphQL Code Generator** - Інструмент, який автоматично генерує TypeScript-типи (або типи інших мов) і шаблонний код на основі вашої GraphQL-схеми та операцій
- **GraphQL** - Основна бібліотека GraphQL
- **Apollo-server** - GraphQL-сервер, який працює з будь-якою схемою GraphQL
- **SQLite** - Легка, автономна SQL-база даних. Весь вміст зберігається в одному файлі
- **JWT (JSON Web Token)** - Компактний, безпечний для URL формат токена, який використовується для безпечної передачі інформації між сторонами. Зазвичай застосовується для автентифікації та авторизації у вебзастосунках
- **Nodemon** - Утиліта для розробки, яка автоматично перезапускає ваш сервер Node.js при виявленні змін у файлах
- **Concurrently** - Інструмент Node.js, який дозволяє запускати кілька команд (скриптів) одночасно в одному терміналі

Повний список залежностей можна знайти у файлі **package.json**

---

## Вміст

- [Встановлення](#Встановлення)
- [Використання](#Використання)

### Встановлення

1. Склонуйте репозиторій:

```shell
git clone https://github.com/labattaria/job-board-server-ts.git
```

2. Встановіть залежності проекту:

```shell
cd job-board-server-ts
npm install
```

### Usage

Запустіть сервер за допомогою наступної команди:

```shell
npm start
```

Це запустить сервер, а також буде відслідковувати зміни в режимі watch, генеруючи вихідні дані у папку за шляхом src/generated/
Сервер буде доступний за адресою **http://localhost:9000/graphql**
