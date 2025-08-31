# 🩺 Diagnosis Assistant

**Diagnosis Assistant** is a Streamlit application powered by OpenAI's GPT API. It allows healthcare professionals and users to input patient symptoms, medical history, and test results to generate probable diagnoses efficiently.

---

## 🌟 Features

* Multi-language support
* Patient data input fields:

  * Symptoms
  * Medical history
  * Examination results
  * Lab test results
* GPT-powered diagnosis generation
* Responsive and user-friendly UI built with Streamlit
* Easy deployment on Streamlit Cloud

  ![App Screenshot](Screenshot.png)

---

## 💻 Installation & Setup

### Prerequisites

* Python 3.8 or later
* pip (Python package manager)
* OpenAI API key
* Streamlit

### Clone the Repository

```bash
git clone https://github.com/your-username/diagnosis-assistant.git
cd diagnosis-assistant
```

### Create a Virtual Environment (Recommended)

```bash
python -m venv venv

# Activate environment:
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

### Install Dependencies

```bash
pip install --upgrade pip setuptools wheel
pip install -r requirements.txt
```

### Configure API Keys

1. Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key_here
```

2. Configure Streamlit secrets:

* Windows: `C:\Users\<your-user>\.streamlit\secrets.toml`
* macOS/Linux: `~/.streamlit/secrets.toml`

```toml
[general]
openai_api_key = "your_openai_api_key_here"
openai_api_model = "gpt-4"
openai_api_temp = 0.7
openai_api_maxtok = 500
openai_api_freqp = 0
openai_api_presp = 0.5

[prompt_canvas]
prompt_system = "You are a helpful medical assistant."
prompt_words = ["Patient details: ", "Pregnancy status: ", "Medical history: ", "Symptoms: ", "Examination results: ", "Lab test results: ", "Language: "]
```

### Run the Application

```bash
streamlit run app.py
```

Open the URL displayed in the terminal (e.g., [http://localhost:8501](http://localhost:8501)).

---

## ⚠️ Troubleshooting

* Ensure API keys are set correctly.
* Verify dependencies: `pip list`
* Clear Streamlit cache if needed: `streamlit cache clear`
* Check terminal logs for errors

---

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature-name`)
3. Make changes and commit (`git commit -m "Add feature"`)
4. Push to your branch (`git push origin feature-name`)
5. Open a Pull Request

---

## 📜 License

MIT License. See [LICENSE](LICENSE) for details.

---

## 📞 Contact

For feedback, issues, or suggestions, open an issue on GitHub or contact the author.
