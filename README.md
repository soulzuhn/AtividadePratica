# DevBlog API

API básica para gerenciamento de posts técnicos de um blog de desenvolvedores.

## Tecnologias

- Node.js
- Express
- MongoDB + Mongoose
- Dotenv

## Instalação

1. Clone o repositório:
   git clone https://github.com/seu-usuario/devblog-api.git
   cd devblog-api
   

2. Instale as dependências:
   npm install express moongose dotenv
   

3. Crie um arquivo `.env` com:
   
   PORT=3000
   MONGO_URI=mongodb+srv://soulzuhn:VtdaZTsbpduPEqlz@cluster0.izbfhx4.mongodb.net/gestao_conteudo?retryWrites=true&w=majority&appName=Cluster0
   

4. Inicie o servidor:
    node app.js

## Testando com Insomnia ou Postman

### Listar posts:
`GET http://localhost:3000/api/posts`

### Buscar por ID:
`GET http://localhost:3000/api/posts/id`

### Criar post:
`POST http://localhost:3000/api/posts`
```json
   {
   "title": "Primeiro Post",
   "content": "Conteúdo aqui...",
   "author": "Dev"
   }
```

### Atualizar post:
`PUT http://localhost:3000/api/posts/id`

### Deletar post:
`DELETE http://localhost:3000/api/posts/id`
