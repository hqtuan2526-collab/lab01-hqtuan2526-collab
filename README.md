## Setup
Prerequisites: Python 3.10+, Git.
 git clone https://github.com/hqtuan2526-collab/lab01-hqtuan2526-collab.git
cd lab01-hqtuan2526-collab
 python -m venv .venv
 source .venv/bin/activate # Windows: .venv\Scripts\Activate.ps1
 pip install -r requirements.txt
 pip install -e .
## Run
 python -m assistant "where is the library?"
 # -> Library: room B.201, open Mon-Sat 07:00-20:00.
## Test
 pytest -q # -> 4 passed
## Troubleshooting
- "No module named assistant" -> you forgot `pip install -e .` or the venv is not active.
- PowerShell blocks Activate.ps1 -> Set-ExecutionPolicy -Scope CurrentUser RemoteSigned