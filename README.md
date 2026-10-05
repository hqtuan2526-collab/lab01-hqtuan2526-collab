# Study Assistant — starter

A starter repository for the CSC10014 Smart Virtual Assistant project.

## Setup

Prerequisites: Python 3.10+ and Git.

```bash
python -m venv .venv
source .venv/Scripts/activate
pip install -r requirements.txt
pip install -e .

For Windows PowerShell:

```powershell
.venv\Scripts\Activate.ps1
```

## Run

Run the assistant with:

```bash
python -m assistant "where is the IT helpdesk?"
```

The assistant will return the office location and opening hours.

## Test

Run the tests with:

```bash
pytest -q
```

All tests should pass successfully.

## Project structure

```text
data/           Sample data
docs/           Documentation
scripts/        Helper scripts
src/assistant/  Assistant application code
tests/          Automated tests
ui/             User interface
