# 🚀 FSC Task Manager API

API simples de gerenciamento de tarefas construída com **JSON Server**, desenvolvida durante a formação em React do Full Stack Club.

## 📌 Sobre o projeto

Esta API simula um backend REST para um sistema de gerenciamento de tarefas (Task Manager), permitindo operações básicas como listar, criar, editar e remover tarefas.

Ela utiliza um arquivo `db.json` como banco de dados local e é ideal para desenvolvimento e testes de aplicações frontend.

---

## 🔗 Links

- 💻 **Projeto frontend (consome essa API):**  
  https://github.com/pedrofaleirosss/fsc-task-manager.git

- 🚀 **API em produção (Vercel):**  
  https://fsc-task-manager-api-kappa.vercel.app/

---

## 🛠️ Tecnologias utilizadas

- ✅ Node.js
- ✅ JSON Server
- ✅ JavaScript

---

## 📂 Estrutura do projeto

```
.
├── api/
│   └── server.js
├── .gitignore
├── db.json
├── package-lock.json
├── package.json
├── vercel.json
└── README.md
```

---

## ⚙️ Como funciona

A API é baseada no **JSON Server**, que transforma o arquivo `db.json` em uma API REST completa automaticamente.

Além disso, foi configurado um **rewriter** para que todas as rotas com `/api` funcionem corretamente.

Exemplo:

```
/api/tasks → /tasks
```

---

## ▶️ Como rodar o projeto

### 1. Clone o repositório

```bash
git clone https://github.com/pedrofaleirosss/fsc-task-manager-api.git
```

### 2. Acesse a pasta

```bash
cd fsc-task-manager-api
```

### 3. Instale as dependências

```bash
npm install
```

### 4. Inicie o servidor

```bash
npm run start
```

Servidor rodando em:

```
http://localhost:3000
```

---

## 📡 Endpoints da API

### 🔹 Listar tarefas

```http
GET /api/tasks
```

---

### 🔹 Buscar tarefa por ID

```http
GET /api/tasks/:id
```

---

### 🔹 Criar nova tarefa

```http
POST /api/tasks
```

Body:

```json
{
  "title": "Nova tarefa",
  "description": "Descrição da tarefa",
  "time": "morning",
  "status": "not_started"
}
```

---

### 🔹 Atualizar tarefa

```http
PUT /api/tasks/:id
```

---

### 🔹 Atualização parcial

```http
PATCH /api/tasks/:id
```

---

### 🔹 Deletar tarefa

```http
DELETE /api/tasks/:id
```

---

## 🧱 Estrutura dos dados

Exemplo de tarefa:

```json
{
  "id": "1",
  "title": "Estudar",
  "description": "Estudar para a prova de matemática",
  "time": "morning",
  "status": "done"
}
```

### 📌 Campos

| Campo       | Tipo   | Descrição                                 |
| ----------- | ------ | ----------------------------------------- |
| id          | string | Identificador único                       |
| title       | string | Título da tarefa                          |
| description | string | Descrição                                 |
| time        | string | Período (morning, afternoon, evening)     |
| status      | string | Status (not\_started, in\_progress, done) |

---

## 🌐 Deploy

A API está hospedada na Vercel e pode ser acessada diretamente:

👉 [https://fsc-task-manager-api-kappa.vercel.app/api/tasks](https://fsc-task-manager-api-kappa.vercel.app/api/tasks)

---

## 💡 Observações

- Este projeto não utiliza banco de dados real (como PostgreSQL ou MongoDB)
- Os dados são armazenados em memória (arquivo JSON)
- Ideal para prototipação e estudos

---

## 📚 Aprendizados

Durante o desenvolvimento desta API, foram praticados:

- Criação de APIs REST com JSON Server
- Manipulação de rotas
- Estruturação de dados
- Integração com frontend React

---

## 👨‍💻 Autor

Desenvolvido por [**Pedro Faleiros**](https://github.com/pedrofaleirosss) 🚀
