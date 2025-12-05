# studybuddy
An interactive AI-driven platform that helps students learn smarter through personalized study plans, flashcards, quizzes, and progress tracking.
🚀 Overview

StudyBuddy AI is an adaptive learning platform designed to help students prepare for exams smarter—not harder.
It uses AI to analyze study material, identify weaknesses, generate learning content, and create a personalized study roadmap.

✨ Features

🎯 Personalized Study Planner

Automatically generates a dynamic study schedule based on:

Subjects & topics

Exam date

Daily available hours

Student strengths & weaknesses

🧠 AI Flashcard Generator

Paste your notes or upload a PDF, and StudyBuddy AI will generate:

Flashcards

Key highlights

Memory cues

Summary sheets

📝 Smart Quiz Generator

Creates quizzes from any text, uploaded notes, or URLs:

MCQs

Short answer

True/False

Coding questions (for CS subjects)

📊 Performance Dashboard

Tracks student improvement:

Mastery levels

Time spent

Topic difficulty

Predicted exam score

🏆 Gamification

XP points

Leaderboard

Weekly streaks

🏗 Tech Stack

Frontend

Next.js

React

Tailwind CSS

Framer Motion

Backend

Python FastAPI

PostgreSQL

Redis (for caching & background jobs)

AI Integration

OpenAI GPT-4.1 / GPT-4o

Embeddings for flashcards

Vector search (FAISS or pgvector)

Mobile (optional)

React Native

🛠 Project Structure
studybuddy-ai/
│
├── frontend/            # Next.js UI
├── backend/             # FastAPI backend
│   ├── routes/          # API endpoints
│   ├── models/          # Pydantic + DB models
│   ├── services/        # AI logic, flashcards, quizzes
│   ├── database/        # SQL scripts, ORM
│   └── main.py          # FastAPI entrypoint
│
├── mobile/              # React Native app (optional)
│
├── docs/                # Architecture diagrams & guides
├── README.md
└── LICENSE

📦 Installation
Clone the repository
git clone https://github.com/your-username/studybuddy-ai.git
cd studybuddy-ai

🧩 Frontend Setup
cd frontend
npm install
npm run dev


Visit:

http://localhost:3000

🧩 Backend Setup
1. Create a Python environment
cd backend
python -m venv venv
venv/Scripts/activate   # Windows
source venv/bin/activate # Mac/Linux

2. Install dependencies
pip install -r requirements.txt

3. Run the server
uvicorn main:app --reload


Backend runs at:

http://localhost:8000

🔐 Environment Variables

Create a .env file in the backend directory:

OPENAI_API_KEY=your_openai_key
DATABASE_URL=postgresql://user:pass@localhost:5432/studybuddy
REDIS_URL=redis://localhost:6379

🧪 API Endpoints
📘 Generate Study Plan
POST /generate-plan

📗 Create Flashcards
POST /flashcards

📝 Generate Quiz
POST /quiz

📊 Analyze Performance
POST /analyze

🧬 Example Flashcard Input
{
  "notes": "Photosynthesis is a process used by plants ..."
}

🧬 Example Flashcard Output
{
  "flashcards": [
    { "front": "What is photosynthesis?", "back": "A process used by plants..." },
    { "front": "Where does photosynthesis occur?", "back": "In the chloroplasts..." }
  ]
}

📸 Screenshots (Add your UI images here)
Home Page	Dashboard

	
🗺 Roadmap

 AI Study Plan Generator

 Flashcard Generation

 Mobile App

 Real-time Study Groups

 AI Voice Tutor

🤝 Contributing

Pull requests are welcome!
For major changes, open an issue to discuss what you'd like to improve.

📄 License

MIT License © 2025 StudyBuddy AI
