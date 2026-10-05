# Study Assistant — starter

A starter repository for the CSC10014 Smart Virtual Assistant project.

## Setup

# Create virtual environment
python -m venv .venv

# Activate virtual environment
# macOS/Linux or Git Bash:
source .venv/Scripts/activate  # or source .venv/bin/activate
# Windows PowerShell:
# .venv\Scripts\Activate.ps1

# Install dependencies
pip install -r requirements.txt
pip install -e .

## Run

python -m assistant "where is the IT helpdesk?"
#-> Library: room B.201, open Mon-Sat 07:00-20:00.

## Test

pytest -q                    #-> 4 passed

## Project structure

* `data/` - Contains data files and office information.
* `docs/` - Documentation and lab guides.
* `scripts/` - Environment verification and utility scripts.
* `src/assistant/` - Core Python source code for the assistant application.
* `tests/` - Automated unit test cases.
* `ui/` - User interface code components.

## Troubleshooting

- "No module named assistant" -> you forgot `pip install -e .` or the venv is not active.
- PowerShell blocks Activate.ps1 -> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned
