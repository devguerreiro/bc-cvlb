# 📡 To Do Backend

Este é o backend da aplicação de tarefas, construído com **FastAPI** e utilizando **SQLite** para persistência.

## ✅ Requisitos

- [Docker](https://www.docker.com/)
- Docker Compose
- Rede Docker compartilhada (`cvlb`)

## 🔌 Criar rede Docker (se ainda não existir)

```bash
docker network create cvlb
```

## 🚀 Subir o backend com Docker Compose

```bash
docker compose up -d
```

> Isso irá iniciar a API na porta **8000** ([http://localhost:8000](http://localhost:8000)).

## 🔁 Endpoints disponíveis

- `GET    /tasks` — Lista todas as tarefas
- `POST   /tasks` — Cria uma nova tarefa (title, description)
- `DELETE /tasks/{id}` — Deleta uma tarefa por ID
- `PATCH  /tasks/{id}` — Marca uma tarefa como concluída

## 🧪 Testar com cURL (exemplo)

```bash
curl http://localhost:8000/tasks
```
