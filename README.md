🧠 RAG Chatbot – AI-powered Legal Assistant (Flask + React)
📌 Overview

This project is an AI-powered legal assistant chatbot built using Flask (Python) for the backend and React.js for the frontend.
It answers user queries related to consumer rights and legal guidance using a Retrieval-Augmented Generation (RAG) architecture.

The project demonstrates how to:

Integrate LLMs (OpenAI-compatible models) in real-world applications

Combine a React frontend with a Flask backend

Handle CORS and REST API communication

Manage local inference and troubleshooting with multiple model versions
__________________________________________________________________________________________________________________________________________________________________________________________

⚙️ Tech Stack
Layer	Technology	Purpose
Frontend	React.js, TailwindCSS	User interface and chat system
Backend	Flask (Python)	API endpoints and LLM integration
AI/LLM	OpenAI-compatible model (gpt-4 / gpt-3.5-turbo, or local)	Language understanding and generation
Utilities	Flask-CORS, Threading	Cross-origin communication and background server run

____________________________________________________________________________________________________________________________________________________________________________________________

🚀 Features

🧩 Chatbot Interface: Ask questions about consumer rights, legal procedures, etc.

🔗 Flask API Integration: Communication between React and backend AI model.

⚡ Asynchronous Operation: Flask runs parallel to Jupyter using threads.

🔒 CORS Configured: Secure communication between localhost:3000 and localhost:5000.

🧠 RAG Ready: Supports expansion with document-based retrieval (deprecation-ready).

_____________________________________________________________________________________________________________________________________________________________________________________________

🧰 Project Structure
rag-chatbot/
│
├── backend/
│   ├── app.py              # Flask backend (API + LLM integration)
│   ├── requirements.txt    # Backend dependencies
│
├── frontend/
│   ├── src/
│   │   ├── App.js          # React UI
│   │   ├── components/     # Reusable chat components
│   │   └── styles/         # Tailwind styles
│   ├── package.json        # Frontend dependencies
│
├── README.md               # Project documentation
└── .gitignore

________________________________________________________________________________________________________________________________________________________________________________________________

🧩 Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/<your-username>/rag-chatbot.git
cd rag-chatbot

2️⃣ Backend Setup (Flask)
cd backend
pip install -r requirements.txt


requirements.txt example:

flask
flask-cors
openai


Run Flask (inside Jupyter or terminal):

from app import app
app.run(port=5000)


If using Jupyter:

!pip install flask flask-cors openai
# then run the cell containing app.run() or the threaded version

3️⃣ Frontend Setup (React)

Open another terminal:

cd frontend
npm install
npm start


Frontend runs on http://localhost:3000

Backend runs on http://127.0.0.1:5000

_______________________________________________________________________________________________________________________________________________________________________________________________

🔄 How It Works

User enters a legal query in the chat window.

React frontend sends a POST request to Flask API (/api/chat).

Flask processes the query, forwards it to the AI model, and returns a JSON response.

The frontend displays the model’s answer in real time.

_______________________________________________________________________________________________________________________________________________________________________________________________


🧠 What Problems It Solves

❌ Many people don’t understand consumer rights or basic legal steps.

✅ This chatbot simplifies complex laws into plain-language answers using AI.

⚙️ It also showcases full-stack AI application integration — bridging backend AI logic with frontend interactivity.

_______________________________________________________________________________________________________________________________________________________________________________________________


💡 Skills Learned
Area	Skill/Concept
Backend Dev	REST API creation, Flask threading, error handling
Frontend Dev	React components, state management, API integration
AI Integration	Using OpenAI-like APIs with Python
DevOps	Localhost coordination, dependency isolation
Debugging	CORS setup, version conflicts, model deprecation fixes

_______________________________________________________________________________________________________________________________________________________________________________________________

🧩 Challenges & Solutions
Challenge	Solution
Flask not connecting to frontend	Implemented flask-cors with proper headers
Model version mismatch	Deployed compatible LLMs and handled deprecation gracefully
Jupyter + Flask concurrency	Used background threading to run Flask within Jupyter
Frontend API errors	Added OPTIONS method and manual CORS response for preflight requests

_______________________________________________________________________________________________________________________________________________________________________________________________

🪄 Future Enhancements

Add vector database (FAISS/Chroma) for RAG document retrieval

Include user chat history and session persistence

Integrate speech-to-text for hands-free queries

Deploy using Render / Vercel / Hugging Face Spaces

_______________________________________________________________________________________________________________________________________________________________________________________________


🧾 Example Query

Input:
“What should I do if an online store refuses to refund a defective item?”

Output:
“You can file a complaint under the Consumer Protection Act, 2019. Start by contacting the seller with proof of defect. If unresolved, approach the consumer forum online through the National Consumer Helpline (NCH).”

_______________________________________________________________________________________________________________________________________________________________________________________________

✨ Author

Nisarga / Sanmati Pol
📍 India | 💻 Computer Science & Data Science Graduate
🧠 Interests: AI, Machine Learning, Full-Stack Projects, Legal-Tech Innovation

