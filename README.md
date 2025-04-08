# 📋 Projeto CRUD com Autenticação - Node.js + Sequelize

Este é um projeto de API RESTful para gerenciamento de **usuários**, **projetos** e **tarefas** com autenticação via JWT. Desenvolvido com Node.js, Express e Sequelize (MySQL).

---

## 🔧 Linguagem e Tecnologias Utilizadas

- Node.js
- Express
- Sequelize
- MySQL
- JWT (jsonwebtoken)
- Bcrypt
- Javascript

---

## 📁 Estrutura do Projeto

```
tasksystemapi_/ 
│-- src/ 
│ ├── config/ 
│ │ └── database.js 
│ ├── controllers/ 
│ │ ├── userController.js 
│ │ ├── projectController.js 
│ │ └── taskController.js 
│ ├── models/ 
│ │ ├── user.js 
│ │ ├── project.js 
│ │ └── task.js 
│ ├── routes/ 
│ │ ├── userRoutes.js 
│ │ ├── projectRoutes.js 
│ │ └── taskRoutes.js 
│ └── server.js
| └── package.json
```
---

## ⚙️ Configuração do Projeto

1. **Clone o repositório**  
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```

2. **Instalar dependências**  
   ```bash
   npm install
   ```

3. **Iniciar servidor**  
   ```bash
   npm start
   ```
Servidor rodando em: http://localhost:3000

> ⚠️ Rodar o XAMPP com o MYSQL ativo e com o banco de dados informado criado. 

> ❗O servidor rodará na porta **3001** por padrão.

---

## 📌 Endpoints

### 🔑 Autenticação
- `POST /register` – Cadastro de novo usuário
- `POST /login` – Login e retorno do token JWT

### 👤 Usuários (`/api/users`)
- `GET /api/users` – Listar todos os usuários
- `GET /api/users/:id` – Buscar usuário por ID
- `PUT /api/users/:id` – Atualizar usuário
- `DELETE /api/users/:id` – Remover usuário

### 📁 Projetos (`/api/projects`)
- `GET /api/projects`
- `GET /api/projects/:id`
- `POST /api/projects`
- `PUT /api/projects/:id`
- `DELETE /api/projects/:id`

### ✅ Tarefas (`/api/tasks`)
- `GET /api/tasks`
- `GET /api/tasks/:id`
- `POST /api/tasks`
- `PUT /api/tasks/:id`
- `DELETE /api/tasks/:id`

> Todos os endpoints (exceto `/register` e `/login`) exigem token JWT válido.

---

## 🧪 Testes com Postman

Recomenda-se o uso do **Postman** para testar os endpoints. Crie uma nova requisição, adicione o token JWT no campo de headers:

```
Authorization: Bearer <seu_token>
```

---

## 📝 Licença

Projeto desenvolvido para fins educacionais e pode ser utilizado livremente para estudos.

