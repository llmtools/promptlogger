# promptlogger

A simple Python utility for logging prompts and responses.

> ⚠️ **For educational use only.** This tool includes a function that sends logs to a remote server. Do not use it with sensitive data or in production environments.

---

## 📦 Features

- Logs prompt-response pairs to a local file (`log_inputs.txt`)
- Sends the same data to a remote server (for educational demonstration)
- Lightweight with minimal dependencies (`requests` only)
- Installable via pip directly from GitHub or from local clone

---

## 🚀 Installation

You can install `promptlogger` using one of the following two methods:

---

### ✅ Method 1: Install directly from GitHub (Recommended)

Install the latest version straight from GitHub:

```bash
pip install git+https://github.com/mjbbusiness/promptlogger.git
To install a specific branch or tag (e.g., v0.1.0):

pip install git+https://github.com/mjbbusiness/promptlogger.git@v0.1.0
```

🛠️ Method 2: Clone and install locally (Best for development)
Clone the repository:
```
git clone https://github.com/mjbbusiness/promptlogger.git
cd promptlogger
Install it in editable mode:


pip install -e .
This allows you to edit the code and see changes instantly without reinstalling.
```

🧪 Usage
After installation, import the logger in your script:
```
python

from promptlogger import log_pair

log_pair("What is the capital of France?", "Paris")
This will:

Append the prompt and response to log_inputs.txt

Send the same data as a JSON POST to a remote endpoint
```

📁 Project Structure
css
```
promptlogger/
├── pyproject.toml
├── README.md
├── src/
│   └── promptlogger/
│       ├── __init__.py
│       └── promptlogger.py

```
🤝 Contributing
Contributions are welcome!

To contribute:
```
bash

git clone https://github.com/mjbbusiness/promptlogger.git
cd promptlogger
pip install -e .
Then edit the files under src/promptlogger/.
```
📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

⚠️ Disclaimer
This code is intended for educational demonstration only.
It includes functionality that sends prompt and response data to a remote server.
Do not use it in production or with real user input.
