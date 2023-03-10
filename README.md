<h1 align="center">
  💸 Transactions API
</h1>

<p align="center">
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/amanda-santos/transactions-api">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/amanda-santos/transactions-api">

  <a href="https://github.com/amanda-santos/transactions-api/commits/master">
    <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/amanda-santos/transactions-api">
  </a>

  <a href="https://github.com/amanda-santos/transactions-api/issues">
    <img alt="Repository issues" src="https://img.shields.io/github/issues/amanda-santos/transactions-api">
  </a>
</p>

<p align="center">
  <a href="#-about-the-project">About the project</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-layout">Layout</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-technologies">Technologies</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-preview">Preview</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-getting-started">Getting started</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-how-to-contribute">How to contribute</a>&nbsp;&nbsp;&nbsp;
</p>

## 📝 About the project

<p>This is a Node.js project built for study purposes. Here a HTTP Rest API is implemented with Typescript, Fastify, Knex, PostgreSQL and more.</p>

<p>With this API it's possible to create and list transactions. Each transaction has a title, an amount of money and a type (credit or debit).</p>

<p>The app is fully tested with E2E tests done with Vitest and Supertest.</p>

<p>Access the API through <a href="https://transactions-api-ukop.onrender.com/" target="_blank">this</a> link.</p>

<p>Developed as part of Ignite Node.js by <a href="https://www.rocketseat.com.br/" target="_blank">Rocketseat</a> 🚀</p>

## ✔️ Functional and non-functional requirements

### Functional requirements

- [x] The user must be able to create a new transaction;
- [x] The user must be able to obtain a summary of his account;
- [x] The user must be able to list all transactions that have already occurred;
- [x] The user must be able to view a single transaction;

### Non-functional requirements

- [x] The transaction can be of the credit type that will add to the total amount, or debit will subtract;
- [x] It must be possible to identify the user among the requests;
- [x] User can only view transactions which he created;

## 👩🏻‍💻 Technologies

Technologies used to develop this project:

- Node.js
- Typescript
- Fastify
- Knex
- PostgreSQL
- SQLite
- Zod
- TSup
- Vitest
- Supertest

## 🚃 Routes

<table>
  <tr>
    <th>HTTP Method</th>
    <th>Route</th>
    <th>Description</th>
    <th>Request body</th>
  </tr>

  <tr>
    <td>GET</td>
    <td>/transactions</td>
    <td>Returns a list of the transactions</td>
    <td>N/A</td>
  </tr>

  <tr>
    <td>POST</td>
    <td>/transactions</td>
    <td>Creates a new transaction</td>
    <td>
      title
      <br />
      amount
      <br />
      type (credit or debit)
    </td>
  </tr>

  <tr>
    <td>GET</td>
    <td>/transactions/:id</td>
    <td>Returns a transaction with the given id</td>
    <td>N/A</td>
  </tr>

  <tr>
    <td>GET</td>
    <td>/summary</td>
    <td>Returns a summary of the transactions</td>
    <td>N/A</td>
  </tr>
</table>

## 🖥 Preview

https://user-images.githubusercontent.com/49074930/224413220-4600101d-39c5-44d2-811a-f00aa97802a6.mp4

## ⌨ Getting started

### Running the server

- Create `.env` file based on `.env.example`
- Run `npm i` to install the dependencies
- Run `npm run knex -- migrate:latest` to run the migrations
- Run the development server with `npm run dev`
- Optionally, import the file `insomnia` on Insomnia to test the routes

### Running E2E tests

- Create `.env.test` file based on `.env.test.example`
- Run `npm test`

## 🤔 How to contribute

**Make a fork of this repository**

```bash
# Fork using GitHub official command line
# If you don't have the GitHub CLI, use the web site to do that.

$ gh repo fork amanda-santos/transactions-api
```

**Follow the steps below**

```bash
# Clone your fork
$ git clone your-fork-url && cd transactions-api

# Create a branch with your feature
$ git checkout -b my-feature

# Make the commit with your changes
$ git commit -m 'feat: My new feature'

# Send the code to your remote branch
$ git push origin my-feature
```

After your pull request is merged, you can delete your branch

---

Made with 💚 by Amanda Santos
