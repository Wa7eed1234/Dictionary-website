# English dictionary lookup

Flask form that requests a word from Dictionary API and shows its first definition, phonetic spelling and part of speech.

## Run locally

Use Python 3 in an isolated environment. The following dependency list is inferred from source imports; this repository has no tested dependency lockfile.

```bash
python -m venv .venv
# Windows PowerShell: .venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
python -m pip install Flask Flask-SQLAlchemy Flask-Login Flask-Admin requests
python -m flask --app main run --host 127.0.0.1 --port 5000
```

Open http://127.0.0.1:5000. Use only synthetic local records. Complete the known repairs below first; dependency compatibility and full application flows have not been verified.

## Current status and known limitations

Handle missing words, missing phonetic fields and network failures. Remove unused database/login/admin imports in a separate code change.

## Review status

Documentation drafted from repository source on 13 September 2026. This review did not run the application or certify it for production.
