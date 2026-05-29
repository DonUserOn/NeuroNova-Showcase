# NeuroNova Architecture

## Public-Safe Overview

NeuroNova v1.0 is a Streamlit MVP built with modular Python components. The public showcase repository does not include private source code, credentials, databases, prompts, or internal implementation details.

## Streamlit MVP Frontend

The current prototype uses Streamlit to deliver a fast, interactive web app experience. Streamlit was chosen for MVP speed, iteration, and simple deployment.

## Modular Python Modules

The private app is organized into separate modules for major product areas such as:

- AI tutoring
- Notebook and saved study material
- Study planning
- Review and memory workflows
- Progress dashboards
- Weekly reporting
- Personalization
- Upload validation and processing
- Export and deployment support

## AI Router And Fallback Concept

NeuroNova uses an AI routing/fallback concept so the app can choose available providers and keep parts of the experience usable when a provider is unavailable. API keys are not stored in this public showcase repo.

## Local/Session Storage And Prototype Database Concept

The MVP uses local/session-based state and a prototype database concept for development and demonstration. This is suitable for showcasing the product workflow, but a production version should use a managed database and stronger authentication.

## Future Production Architecture

```text
Next.js -> FastAPI -> PostgreSQL/Supabase -> AI Router -> Storage
```

## Production Direction

- Next.js for a responsive production frontend
- FastAPI for backend APIs
- PostgreSQL or Supabase for structured data
- Managed object storage for files
- Real authentication and authorization
- Observability, logging, and admin tools
- Stronger security review before handling sensitive data
