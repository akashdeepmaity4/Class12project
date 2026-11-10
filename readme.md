# Raw Source Text to Relation Parser
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

This is a Python-based text parsing tool designed to transform unstructured human-language content into a structured relational database using SQL. Its core purpose is to take raw unordered source text, identify meaningful entities and relationships, and convert them into database-ready data that can be queried, analyzed, and reused. 

The project is aimed at users who want to bridge the gap between natural language and formal data models without manually coding extraction logic. This makes the tool useful for:

1. knowledge extraction
1. Structured data conversion
1. Simplifying the raw information

## Usage

RawSTRaP is a Python desktop utility for transforming raw, unstructured text into a clean CSV dataset and then saving that dataset to a database. The app accepts pasted text, sends it through a selected AI provider, and converts the response into database-ready rows.

### Data Pipeline

- Accepts source text from a pasted document or file
- Validates a supported AI provider key
- Selects a model automatically from the provider's available list
- Prepares the source text into a structured conversion prompt
- Extracts CSV output from the model response
- Validates the CSV headers and row structure
- Saves the parsed records to SQLite or MySQL

### Supported providers (i will be adding more in the future)

- Google Gemini
- OpenAI
- xAI
- Anthropic Claude
- Groq-hosted Llama

### Supported databases

- SQLite
- MySQL

### Typical workflow

1. Open the app.
2. Choose a provider and enter the API key.
3. Paste the document content you want to structure.
4. Click PROCESS.
5. Review the generated CSV output.
6. Save the result to SQLite or MySQL.

## Steps to run

1. Open a terminal in the project folder.
2. Create and activate a virtual environment if needed:

Windows PowerShell:

```ps1
.\.venv\Scripts\Activate.ps1
```

Windows Command Prompt:

```bash
.\.venv\Scripts\activate.bat
```

macOS/Linux:

```bash
source .venv/bin/activate
```

3. Install the dependencies:

```bash
pip install -r requirements.txt
```

4. Start the application:

```bash
cd path/of/root/directory
python run.py
```

5. Choose an AI provider and enter its API key when prompted.
6. Paste the text to be converted and click PROCESS.
7. Select the output database type:
   - SQLite for local storage in the project folder
   - MySQL for a remote database connection
8. Once saved, the parsed records can be reviewed and queried from the generated database.

### Notes

- The project requires internet access for the selected AI provider API.
- MySQL support requires valid host, port, username, and password details.
- SQLite output is stored in the project directory and is the easiest option for a quick start.
- Keep the source document clean and readable for best extraction quality.