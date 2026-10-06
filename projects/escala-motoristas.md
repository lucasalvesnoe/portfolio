# Driver rostering optimisation

| | |
|---|---|
| **Client** | Intercity bus operator |
| **Sector** | Transport and logistics |
| **Source code** | not versioned on GitHub — available on request |

## What it is

Driver and vehicle rostering optimisation engine for an intercity bus operator. This is an operations research problem, not CRUD: generate a roster that covers 100% of operational demand while respecting the working-hours rules that apply to the profession. It has a data layer loaded with real data, a demo API, its own frontend, cost modelling and Docker packaging with Compose. Python.

## Stack

```
fastapi · uvicorn · pydantic · pydantic-settings · ortools · pulp · scipy · numpy ·
sqlalchemy · alembic · psycopg2-binary · redis · asyncpg · pandas · openpyxl · python-
dateutil · httpx · python-multipart · python-jose · passlib · python-dotenv · reportlab ·
jinja2 · matplotlib · seaborn · celery · flower · prometheus-client · python-json-logger ·
pytest · pytest-asyncio · pytest-cov · faker · black · flake8 · mypy · pre-commit · mkdocs ·
mkdocs-material
```

---

[← back to index](../README.md)
