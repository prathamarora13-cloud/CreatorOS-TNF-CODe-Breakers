# CreatorOS — Team TNF Code Breakers

**College:** Rawal Institute of Engineering and Technology  
**Department:** Computer Science and Engineering  
**Course:** B.Tech CSE, 3rd Semester  
**Team members:** Piyush, Pratham Arora, Prajwal Singh  
**Project title:** CreatorOS — An AI-Powered Content Creation Assistant

## Features in this prototype
- Idea Generator
- Script Writer
- Caption Generator
- Shot List Generator
- Demo mode that works without an API key
- Optional AI generation through the OpenAI API
- Save, view, download, and delete projects using SQLite
- Download generated content as Markdown

## Requirements
- Python 3.11 or newer recommended
- Internet connection for installing libraries and using the AI API
- Visual Studio Code is recommended but not required

## Run on Windows
Open PowerShell in this project folder:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m streamlit run app.py
```

The app should open in your browser. If it does not, visit `http://localhost:8501`.

### If PowerShell blocks virtual-environment activation
You can skip activation and run the environment's Python directly:

```powershell
.\.venv\Scripts\python.exe -m pip install -r requirements.txt
.\.venv\Scripts\python.exe -m streamlit run app.py
```

## Enable AI mode (optional)
1. Copy `.env.example` and rename the copy to `.env`.
2. Open `.env` and replace `your_api_key_here` with your own API key.
3. Confirm `OPENAI_MODEL` is a model available to your account.
4. Restart the Streamlit app.

API usage may cost money and is separate from a ChatGPT subscription. Do not share your API key or commit `.env` to GitHub. The app works in demo mode without an API key.

## Project structure
```text
CreatorOS_TNF_Code_Breakers/
├── app.py
├── requirements.txt
├── .env.example
├── .gitignore
├── README.md
└── COLLEGE_PROJECT_REPORT.md
```

## Troubleshooting
- **`python` not found:** Install Python and enable the option to add Python to PATH, then reopen PowerShell.
- **`streamlit` not found:** Run `python -m pip install -r requirements.txt` in the project environment.
- **App already running:** Use the URL printed in the terminal; port 8501 may have changed.
- **AI not responding:** Check the API key, model access, network, and API billing. Demo mode is the fallback.
- **PowerShell activation error:** Use the no-activation commands above.

## Academic note
This is a working starter prototype. Features described as future scope in the report are not implemented unless they appear in the app. Update the report and screenshots to reflect what your team actually tests and demonstrates.
