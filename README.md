# Hopscotch Exchange Desk

Reads a customer's exchange request, checks the facts with tools, and picks **Approve**, **Decline** or **Escalate**.

## Setup

```bash
python -m venv .venv
.venv\Scripts\activate          # macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env            # add your OPENROUTER_API_KEY
```

## Run

```bash
python main.py                  # all test messages
streamlit run app.py            # UI
```

## Build it during the session

`desk/` starts with only `__init__.py`. You'll create the other files in it as you follow the session.

`main.py` and `app.py` import from `desk`, so they won't run until those files exist. A `ModuleNotFoundError` before then is expected.
