# Study Assistant — starter

A starter repository for the CSC10014 Smart Virtual Assistant project.

## Setup

# Clone the repository
git clone [https://github.com/hqtuan2526-collab/lab01-hqtuan2526-collab.git](https://github.com/hqtuan2526-collab/lab01-hqtuan2526-collab.git)
cd lab01-hqtuan2526-collab

# Create virtual environment
python -m venv .venv

# Activate virtual environment
# macOS/Linux or Git Bash:
source .venv/Scripts/activate  # or source .venv/bin/activate
# Windows PowerShell:
.venv\Scripts\Activate.ps1

# Install dependencies
pip install -r requirements.txt
pip install -e . (Lab 1): write the exact steps a new teammate needs, from a fresh machine to
running the app and the tests. Your partner will follow them without your help.

## Run

python -m assistant "where is the IT helpdesk?"
# -> Library: room B.201, open Mon-Sat 07:00-20:00.

## Test

pytest -q                    # -> 4 passed

## Project structure

data/ - Contains data files and office information.

docs/ - Documentation and lab guides.

scripts/ - Environment verification and utility scripts.

src/assistant/ - Core Python source code for the assistant application.

tests/ - Automated unit test cases.

ui/ - User interface code components.

## Troubleshooting
- "No module named assistant" -> you forgot `pip install -e .` or the venv is not active.
- PowerShell blocks Activate.ps1 -> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned