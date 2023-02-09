# NodeJS03.js
Usando o Express, crie um código Node.JS, que deve receber requisições HTTP GET e POST. Depois, coloque o servidor para rodar na porta 8080.

const express = require('express');
const app = express();
const port = 8080;

app.get('/', (req, res) => {
  res.send('Recebendo uma requisição GET');
});

app.post('/', (req, res) => {
  res.send('Recebendo uma requisição POST');
});

app.listen(port, () => {
  console.log(`Servidor rodando na porta ${port}`);
});
