# MLOps

A small Python project scaffolded with Poetry for building an AI/ML service. The current dependencies include FastAPI and Google GenAI.

## Requirements

- Python 3.13 or newer
- Poetry

## Setup

Install dependencies:

```powershell
poetry install
```

Create your local environment file:

```powershell
Copy-Item env.example .env
```

Then edit `.env` and add your real Google API key:

```env
GOOGLE_API_KEY=your_real_key_here
```

## Environment Variables

| Variable | Description |
| --- | --- |
| `GOOGLE_API_KEY` | API key used by Google GenAI. |
| `APP_NAME` | Application name. Defaults to `mlops`. |
| `APP_ENV` | Runtime environment, such as `development` or `production`. |

## Usage

Activate the Poetry environment:

```powershell
poetry shell
```

Run a Python file inside the environment:

```powershell
poetry run python ai_model.py
```

## Project Files

- `ai_model.py` - main Python file for model or API code.
- `pyproject.toml` - project metadata and dependencies.
- `poetry.lock` - locked dependency versions.
- `.env` - local environment variables, ignored by git.
- `env.example` - template for required environment variables.
