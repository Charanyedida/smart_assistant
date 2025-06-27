🧠 Smart Research Assistant
Smart Research Assistant is an AI-powered tool that helps users interact intelligently with research documents (PDF/TXT). It enables summarization, Q&A, logic-based challenges, and answer evaluation — all grounded directly in the document content.

🔗 Live App: https://smartassistant-charan.streamlit.app/
📦 Tech Stack: Python · Streamlit · Hugging Face Transformers · OpenRouter API · PDF/Text Parsing

✨ Features
Feature	Description
📄 Upload Docs	Upload any PDF or TXT file to analyze its content
📝 Auto Summary	Generate concise summaries (≤150 words) using Transformer-based models
💬 Ask Anything	Ask any question grounded in the document, with justification
🧠 Challenge Me	Auto-generate 3 logic/comprehension questions + evaluate user answers
☁️ Local + Cloud Mode	Toggle between free local models and powerful cloud APIs via OpenRouter

🚀 Getting Started
1. Clone the Repo
bash
Copy
Edit
git clone https://github.com/yourusername/smart-research-assistant.git
cd smart-research-assistant
2. Setup Virtual Environment
bash
Copy
Edit
python -m venv smart_env
source smart_env/bin/activate  # or smart_env\Scripts\activate on Windows
3. Install Requirements
bash
Copy
Edit
pip install -r requirements.txt
4. Run the App Locally
bash
Copy
Edit
streamlit run app.py
🧰 Configuration
🔐 API Key (for Cloud Mode)
To use OpenRouter AI models:

python
Copy
Edit
api_key = "your_openrouter_api_key"
For security, you may store it via environment variables or use Streamlit secrets in production.

📁 Project Structure
bash
Copy
Edit
smart-research-assistant/
│
├── app.py                        # Main Streamlit App
├── modules/
│   ├── file_handler.py          # Extracts text from PDF/TXT
│   ├── summarizer.py            # Summarizes content
│   ├── qa_module.py             # Handles Q&A (local)
│   ├── question_gen.py          # Question generation (local)
│   └── evaluator.py             # Answer evaluation (local)
├── assets/                      # Static resources, if needed
├── requirements.txt             # Dependencies
└── README.md
🧪 Future Enhancements
🎙️ Whisper Integration for audio-based inputs

🧵 Session memory across interactions

🎯 Feedback-based question refinement

📊 Admin dashboard for document analytics

🙌 Credits
Built by Charan Yedida using:

Streamlit

Hugging Face Transformers

OpenRouter AI
