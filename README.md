# Personal AI Knowledge Hub

A personal, AI-supported knowledge hub that indexes your own documents (e.g. PDFs and notes) and allows them to be searched intelligently via a chat interface.  
The project combines modern technologies such as **LLM-based queries** (RAG), **FastAPI**, **React/Next.js** and a **vector database** (Chroma). 

---

## Features

- **Document upload:** PDFs, text or Markdown files can be uploaded and analyzed.
- **Semantic search:** Queries in natural language (e.g. “What is in chapter 3?”).
- **AI-supported chat:** LLM answers questions based on uploaded documents and names sources.
- **Modern full-stack setup:** FastAPI (backend), React/Next.js (frontend), PostgreSQL and ChromaDB.
- **Containerized:** Easy installation and start via Docker-Compose.

---

## Technology stack

- **Backend:** [FastAPI](https://fastapi.tiangolo.com/) (Python)
- **Frontend:** [Next.js](https://nextjs.org/) + [React](https://react.dev/) + [TailwindCSS](https://tailwindcss.com/)
- **Databases:** PostgreSQL + [ChromaDB](https://www.trychroma.com/)
- **AI:** OpenAI API (Embeddings & ChatGPT)
- **Containerization:** Docker & Docker-Compose

---

## Local development

### Clone repository

```bash
git clone git@github.com:tflm91/ai-knowledge-hub.git
cd ai-knowledge-hub
```

### Start backend

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload
```

The backend can then be accessed at: [http://localhost:8000]

### Start frontend

```bash
cd frontend
npm install
npm run dev
```

The frontend can then be reached at: [http://localhost:3000]

### Docker (optional)

The project can be started easily with Docker-Compose: 

```bash
docker-compose up --build
```

---

## License

This project is licensed under the [MIT license](LICENSE).

