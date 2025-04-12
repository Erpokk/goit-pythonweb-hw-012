# goit-pythonweb-hw-12


## Used libs and technology

- Python 3.11
- FastAPI
- PostgreSQL
- ORM SQLAlchemy
- Alembic
- Swagger
- Pydantic
- Docker
- Poetry
- JWT
- Gravatar
- Dotenv
- Slowapi
- Cloudinary
- pytest
- Sphinx
- Redis

## Terms of reference

## Installation and launch

1. Clone the repository

2. Go to the project directory

```
cd goit-pythonweb-hw-12
```

3. Create and configure the `.env' file in the project root following the example:

```
JWT_SECRET=<your jwt secret>

DB_NAME=contacts_db
DB_USER=postgres
DB_PASSWORD=<your db password>
DB_PORT=5432
DB_HOST=<host>
DB_URL=postgresql+asyncpg://${DB_USER}:${DB_PASSWORD}@${DB_HOST}:${DB_PORT}/${DB_NAME}

CLD_NAME=<your cloudinary name>
CLD_API_KEY=<your cloudinary API key>
CLD_API_SECRET=<your cloudinary API secret>
```

4. Use Docker Compose to build and run your environment.

```
docker-compose up --build
```

5. The web application runs on port 8000:

Swagger: http://localhost:8000/docs


### Test

To run the tests, use the command:
```
poetry run pytest
```
Check for test coverage

```
pytest --cov=src tests
```

### Docs

To generate documentation with Sphinx

1. Run the Windows command:

```
.\\make.bat html
```

Linux:

```
make html
```

2. Open in a browser `docs/_build/html/index.html`
