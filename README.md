# ManageEmployees API

.NET 8 Web API with Clean Architecture, ADO.NET, ASP.NET Identity, and JWT authentication.

## Tech Stack

- .NET 8 / C# 12
- SQL Server with raw ADO.NET (no ORM)
- Custom ASP.NET Identity stores
- JWT Bearer + Refresh Tokens
- NUnit (186 tests — 111 unit + 75 integration)
- SonarQube analyzed (82% coverage, 0 bugs, 0 code smells)

## Running

```bash
# Local
dotnet run --project ManageEmployees.Api    # https://localhost:64715

# Docker (full stack)
docker compose up --build                   # http://localhost:64715
```

Swagger UI is available at the root URL.  
Database is auto-initialized on startup (schema, seeds, indexes).

## Default Login

- **Email:** `admin@company.com`
- **Password:** `Admin123!`

### Project Documentation
The files are in the “docs” folder

| Document | Description |
|----------|-------------|
| [PRESENTATION.md](docs/PRESENTATION.md) | Architecture decisions and technical summary |
| [GENAI_USAGE.md](docs/GENAI_USAGE.md) | AI usage methodology and contributions |
| [TEST_VALIDATION_PLAN.md](docs/TEST_VALIDATION_PLAN.md) | Requirement traceability matrix |