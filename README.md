# Asha-Bot-Empowering-Women-in-Careers

# 🤖 Asha Bot – Her Career Compass

Asha Bot is a context-aware AI chatbot designed to empower women re-entering the workforce. With voice-enabled interaction, personalized guidance, real-time job and mentor lookup, bias detection, and skill-building tips, Asha provides a privacy-first and inclusive experience.

🔗 **Live Demo:** [https://her-career-compass.lovable.app](https://her-career-compass.lovable.app)

---

## 🚀 Features

- 🎙️ **Voice Input**  
  Hands-free conversation for accessible interaction

- 🧭 **Personalized Career Navigation**  
  Curated job and mentorship recommendations based on user goals

- 🧠 **Bias Detection & Reframing**  
  Detects discouraging language and reframes it using Perspective API and custom prompts

- 📊 **Empowerment Pulse**  
  Visual dashboard showing progress, goals, and confidence trends

- 🧩 **Modular Architecture**  
  Easily extensible with CSVs, Airtable, or custom APIs

- 🌐 **Zero-login Experience**  
  Fully client-side with no data stored; privacy by design

- 🔧 **Admin Panel** *(Admin only)*  
  Real-time content management via Airtable backend

---

## 🧱 Architecture

![Architecture Diagram](architecture.png)

- **Rasa + Transformers** – NLP for intent classification & dialogue
- **Perspective API** – Reframes limiting or biased input in real-time
- **Semantic Search** – Matches user profiles with jobs & mentors from CSV
- **Gradio or React Frontend** – Voice-enabled UI embedding the chatbot
- **Dockerized Setup** – Run locally or deploy to cloud effortlessly
- **Serverless Hosting** – Powered by Railway or A0.dev

---

## 🖼️ UI Previews

![Wireframes](wireframes.png)

---

## 📦 Installation

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/asha-bot.git
cd asha-bot

# 2. Set up virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Train and start the Rasa server
rasa train
rasa run --enable-api

# 5. Launch frontend
# Option A: Gradio
python app.py

# Option B: React (from frontend directory)
cd frontend
npm install
npm start


📁 Project Structure

asha-bot/
│
├── data/                   # Rasa domain, stories, and rules
├── actions/                # Custom Python actions (e.g., bias reframing)
├── nlu/                    # Training data for intents
├── frontend/               # Gradio or React UI
├── docker-compose.yml      # Optional Docker setup
├── requirements.txt
└── README.md

🛡️ Ethical AI & Privacy
✅ No personally identifiable information collected
✅ No login, cookies, or trackers
✅ Transparent NLP intent handling
✅ Reframes limiting beliefs using GenAI responsibly

👩‍💻 Contributing
We welcome all contributors passionate about equity and inclusion in tech!
Please feel free to open an issue, submit a pull request, or share ideas 💡


---
📄 License
MIT License © 2025 Sudarshanam Yessasvini

Let me know if you'd like:
- A `requirements.txt` or `docker-compose.yml` generated
- A ZIP archive of this project structure
- Shields.io badges (like `Built with Rasa`, `MIT Licensed`, `Python 3.x`)
- GitHub Actions for testing or deployment

Ready to push this to a repo? I can help with the commit message, repo description, and first release setup too!
