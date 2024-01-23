# Travel Tracker App

Esta é uma aplicação simples construída em Node.js para acompanhar os países já visitados. A aplicação utiliza o banco de dados PostgreSQL para armazenar informações sobre os usuários e os países visitados.

## Configuração

Certifique-se de ter o Node.js e o PostgreSQL instalados antes de iniciar a aplicação. Além disso, crie um banco de dados PostgreSQL chamado "traveltracker" e configure as variáveis de ambiente no arquivo .env com as seguintes informações:

```env

DB_USER=seu_usuario_do_banco
DB_PASSWORD=sua_senha_do_banco
```

Instale as dependências do projeto usando:

```bash
npm install
```
## Funcionalidades

- Visualizar países visitados por usuário.
- Adicionar países visitados.
- Adicionar novos usuários.

## Estrutura do Projeto

- index.ejs: Página principal que exibe os países visitados pelo usuário.
- new.ejs: Página para adicionar novos usuários.
- public: Pasta contendo arquivos estáticos como folhas de estilo.

## Executando a Aplicação

Execute o seguinte comando para iniciar o servidor:

```bash
node app.js
```

Acesse a aplicação em http://localhost:3000.

## Endpoints

- GET /: Exibe os países visitados pelo usuário.
- POST /add: Adiciona um país visitado pelo usuário.
- POST /user: Permite a troca do usuário atual ou adição de um novo usuário.
- POST /new: Adiciona um novo usuário ao banco de dados.

## Tecnologias Utilizadas

- Node.js
- Express.js
- PostgreSQL
- EJS (Embedded JavaScript) para templates