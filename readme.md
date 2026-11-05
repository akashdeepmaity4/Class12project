# Raw Source Text to Relation Parser - Project Details


## Synopsys


Raw Source Text to Relation Parser : Python Application to turn everyday conversation into AI-guided SQL database for meetings, classes or notes. 

## Pipeline

User enters a API provider and an API. the API field is then locked in for the session and then destroyed post-session or if the app is ubruptly closed. The application asigns 'source' variable to the text. if any file is provided, the file is converted into text, then done the same. The app stitches 'pre_payload' (the prefix query prompt) and 'source' (user source text) into 'payload' (using concatination) an sends the payload to the API. the CSV is returned and the application uses interfacing sql with python to convert it into a relational database. Application Uses LLM support, UI is rendered using native Tkinter and Pillow Library and payload is dual-sanitized in the server side to avoid prompt-jacking. 

## Tech Stack

### Languages used

- Python 3.14

### Libraries & Modules used

- Pillow
- csv
- Tkinter
- sqlite3
- pathlib
- tabulate
- json

## How to use

### 2. Native Python Script

- go to the [Github Repository](https://github.com/akashdeepmaity4/rawstrap) and download the source code.
```bash
git clone https://github.com/akashdeepmaity4/rawstrap
```
- save it to your desired directory.
- run the run.py file via python
```bash
cd root/of/the/repository
python run.py
```
- The natively run python application will run.
