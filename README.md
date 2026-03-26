🌿 EmoLearn
EmoLearn is an emotion-aware chat application that understands how users feel, learns from feedback, and responds with empathy.
Instead of just chatting, EmoLearn detects emotional context, adapts over time, and creates a more human, supportive experience.

✨ Features

🧠 Emotion Detection

Analyze user messages to identify emotions like sadness, anger, joy, and more.

🔁 Learning Feedback Loop

Users can confirm or correct detected emotions → the system improves over time.

💬 Context-Aware Conversations

Maintains recent message history for more natural responses.

🌱 Check-in System

Periodically reflects emotional patterns and asks meaningful questions.

🤖 AI-Powered Replies (Groq / LLM)

Generates empathetic, human-like responses based on emotional context.

📊 User Stats Dashboard

Tracks accuracy, corrections, and emotional trends.


🏗️ Tech Stack

* Frontend
* React (Vite)
* Custom hooks (useChat)
* Component-based UI
* Backend
* Python (API routes)
* Emotion analysis system
* Feedback + correction handling
* AI Integration
* Groq API (LLM for responses)



⚙️ Setup

1\. Ensure Python is installed

python --version

You should see Python 3.8 or higher.


2\. Create a virtual environment (recommended)

python -m venv venv

Activate it: 

for Windows,
venv\\Scripts\\activate

for Mac/Linux,
source venv/bin/activate


3\. Install dependencies

pip install -r requirements.txt

4\. Run the server

python app.py

Server will start at:

http://localhost:5000


📌 On first run:

Database will be created automatically

models/ folder will be generated

🧠 How the Learning Loop Works

EmoLearn improves over time using a feedback-driven learning system:

🔄 Step-by-step flow

User sends a message

→ A rule-based keyword detector runs first

Model selection

→ If enough user data exists, a personal ML model is used instead

User feedback

✅ Confirm → reinforces correct prediction

✏️ Correct → stores correction in database

Model update

→ On correction, the model is retrained instantly using SGDClassifier

Future predictions improve

Previously corrected patterns are matched first

Then ML model prediction is applied

🔌 API Endpoints

POST /analyze → Detect emotion from message

POST /correct → Correct detected emotion

POST /confirm → Confirm prediction

GET /stats/:userId → User stats

POST /chat → Generate AI response


🚀 Future Improvements

Better emotion model accuracy

Memory across sessions

Personalization per user

Mobile responsiveness

Voice-based interaction


🤝 Contributing

Contributions are welcome!

Feel free to open issues or submit pull requests.


📄 License

This project is open-source and available under the MIT License.


💡 Vision

EmoLearn aims to go beyond chat to create a system that listens, understands, and grows with the user.





