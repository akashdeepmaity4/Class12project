# Raw Source Text to Relation Parser - Project Details

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![MySQL](https://img.shields.io/badge/MySQL-darkblue?style=for-the-badge&logo=mysql&logoColor=ffdd54)
![SQLite](https://img.shields.io/badge/SQLite-351111?style=for-the-badge&logo=sqlite&logoColor=ffdd54)
![Git CLI](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

## What is it?


![class 12](https://shields.io/badge/Class-12-green)
![ MIT license](https://shields.io/badge/MIT-License-yellow)

Raw Source Text to Relation Parser is a Python-based text parsing tool designed to transform unstructured human-language content into a structured relational database using SQL. Its core purpose is to take raw unordered source text, identify meaningful entities and relationships, and convert them into database-ready data that can be queried, analyzed, and reused.

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

- go to the [Github Repository](https://github.com/akashdeepmaity4/class12project) and download the source code.
```bash
git clone https://github.com/akashdeepmaity4/class12project
```
- save it to your desired directory.
- run the run.py file via python
```bash
cd root/of/the/repository
python run.py
```
- The natively run python application will run.
