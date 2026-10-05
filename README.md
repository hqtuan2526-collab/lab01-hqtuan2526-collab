# Lab 01 - Developer Environment

This repository contains the starter project for CSC10014 Lab 1 - Developer Environment & Reproducible Setup.

The project is a small rule-based Smart Virtual Assistant that can answer simple questions about university offices, such as their locations and opening hours.

## Prerequisites

Before setting up the project, make sure you have:

- Python 3.10 or newer
- Git
- Git Bash (recommended on Windows)
- Visual Studio Code (recommended)

Check your installations:

```bash
python --version
git --version
```

## Setup

Clone the repository:

```bash
git clone git@github.com:hqtuan2526-collab/lab01-hqtuan2526-collab.git
cd lab01-hqtuan2526-collab
```

Create a Python virtual environment:

```bash
python -m venv .venv
```

Activate the virtual environment.

On Windows using Git Bash:

```bash
source .venv/Scripts/activate
```

On Windows using PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

On macOS/Linux:

```bash
source .venv/bin/activate
```

After activation, the terminal should show `(.venv)`.

Install the required dependencies:

```bash
pip install -r requirements.txt
pip install -e .
```

## Run

Run the assistant with a question:

```bash
python -m assistant "where is the IT helpdesk?"
```

You can also start the assistant in interactive mode:

```bash
python -m assistant
```

Type `quit` to exit.

## Test

Run the automated tests:

```bash
pytest -q
```

The tests should complete successfully.

## Check Environment

Run the environment checking script:

```bash
python scripts/check_env.py
```

All checks should display:

```text
[ OK ]
```

## Project Structure

```text
lab01-hqtuan2526-collab/
├── data/               # Sample data
├── docs/               # Documentation
├── scripts/            # Helper scripts
├── src/
│   └── assistant/      # Assistant application code
├── tests/              # Automated tests
├── ui/                 # User interface files
├── .gitignore          # Files ignored by Git
├── README.md            # Project setup documentation
├── pyproject.toml       # Project configuration
└── requirements.txt     # Python dependencies
```

## Troubleshooting

### No module named assistant

Make sure the virtual environment is active and install the project in editable mode:

```bash
pip install -e .
```

### Virtual environment is not active

On Windows using Git Bash:

```bash
source .venv/Scripts/activate
```

On PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

### PowerShell blocks Activate.ps1

Run:

```powershell
Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
```

Then activate the environment again.

### VS Code uses the wrong Python interpreter

Press:

```text
Ctrl + Shift + P
```

Select:

```text
Python: Select Interpreter
```

Then choose the Python interpreter inside `.venv`.

## Author

GitHub: hqtuan2526-collab