# digital-twin-local
This repo is based on the guideline by `Ed Donner's` [production repo](https://github.com/ed-donner/production/tree/main/week2) which is used at his [Udemy AI Engineering Production Track](https://www.udemy.com/course/generative-and-agentic-ai-in-production) course. 

## Getting Started

This repos is based on Ed Donner's repo except it has used `Gemini API` rather than `openAI API`

### Start Backend

- Add Environment varialbes at your `backend/.env` file:

```
GEMINI_API_KEY=YOUR_API_KEY
CORS_ORIGINS=http://localhost:3000
```

- Run Backend

```bash
cd backend
uv init --bare
uv python pin 3.12
uv add -r requirements.txt
uv run uvicorn server:app --reload
```

- Run Frontend

```bash
cd frontend
npm run dev
```

That's it, Now you should see a chat box at `http://localhost:3000`
