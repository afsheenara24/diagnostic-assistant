[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://medicaldiagnosticassistant.streamlit.app)

# Diagnosis Assistant

This is a **Diagnosis Assistant** application built with Streamlit and OpenAI's GPT API. It allows users to input patient symptoms, medical history, and test results to generate a possible diagnosis.

---

**Installation & Setup**

**Prerequisites**
Make sure you have the following installed:
- Python 3.8 or later
- `pip` (Python package manager)
- OpenAI API key
- Streamlit

**Clone the Repository**

git clone https://github.com/your-repo/diagnosis-assistant.git
cd diagnosis-assistant

**Create a Virtual Environment (Recommended)**
It's best to use a virtual environment to manage dependencies:

python -m venv venv  # Create a virtual environment
source venv/bin/activate  # On macOS/Linux
venv\Scripts\activate  # On Windows


**Install Dependencies**

pip install -r requirements.txt


**Set Up API Keys**
Create a `.env` file in the project root and add your OpenAI API key:

OPENAI_API_KEY=your_openai_api_key_here


Also, ensure your Streamlit secrets file (`~/.streamlit/secrets.toml` or `C:\Users\your-user\.streamlit\secrets.toml`) is properly configured:

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

**Running the Application**
After setting up the environment and dependencies, run the following command:

streamlit run app.py

This will start the Streamlit web application. Open the displayed URL (e.g., `http://localhost:8501`) in your browser.

**Features**
- Multi-language support
- Patient data input fields (symptoms, history, lab results, etc.)
- OpenAI GPT-based diagnosis generation
- Responsive UI with Streamlit
- User-friendly interface

**Troubleshooting**
If you run into issues:
- Make sure your API keys are correctly set.
- Ensure all dependencies are installed using `pip list`.
- Run `streamlit cache clear` if the app is not updating.
- Check logs for errors when running `streamlit run app.py`.

**Contributing**
Feel free to fork this repository and submit pull requests with improvements!

**License**
This project is licensed under the MIT License. See `LICENSE` for details.

---

## Contact
For any issues or suggestions, please open an issue on GitHub or contact the author.


