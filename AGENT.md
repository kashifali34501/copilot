# 🚀 Copilot Project Reference

## 🛠 Stack
- **Frontend:** Next.js 16, React 19, Node 24, TS 7, shadcn/ui (`frontend/`, port 3000)
- **Backend:** FastAPI, Python 3.13, uv, Ruff, pytest (`backend/`, port 8000)
- **AI:** Ollama (`gemma3:1b`), OpenAI, Anthropic, Grok, Meta, Gemini

## ⌨️ Commands
### Frontend
`cd frontend && npm install && npm run dev`
- Install package: `npm install <package>`

### Backend
`cd backend && uv sync && uv run fastapi dev`
- Add package: `uv add <package>`
- Test: `uv run pytest`
- Lint/Format: `uv run ruff check .` | `uv run ruff format .`

## 📜 Guidelines
- **Structure:** Keep `frontend/` and `backend/` strictly separated.
- **Tools:** Use `uv` (Python) and `npm` (JS/TS). Format with **Ruff**.
- **Workflow:** Run tests after changes; keep updates minimal and consistent.
- **Security:** **Never commit secrets.** Use environment variables for all API keys.
- **Dependencies:** Avoid unnecessary new libraries.
