<div align="center">

# FastAPI Fullstack Generator

### Production-Ready FastAPI + Next.js Generator for AI Applications

[![GitHub Stars](https://img.shields.io/github/stars/AhmedRaoofuddin/Generator?style=for-the-badge&logo=github&color=yellow&labelColor=1a1a1a)](https://github.com/AhmedRaoofuddin/Generator/stargazers)
[![License](https://img.shields.io/github/license/AhmedRaoofuddin/Generator?style=for-the-badge&color=blue&labelColor=1a1a1a)](https://github.com/AhmedRaoofuddin/Generator/blob/main/LICENSE)
[![Python](https://img.shields.io/badge/python-3.11%20%7C%203.12%20%7C%203.13-blue?style=for-the-badge&logo=python&logoColor=white&labelColor=1a1a1a)](https://www.python.org/)
[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen?style=for-the-badge&labelColor=1a1a1a)](https://github.com/AhmedRaoofuddin/Generator)
[![Integrations](https://img.shields.io/badge/integrations-20%2B-brightgreen?style=for-the-badge&labelColor=1a1a1a)](https://github.com/AhmedRaoofuddin/Generator)

**Generate enterprise-grade full-stack applications with AI agents, authentication, real-time streaming, and observability in minutes.**

[Quick Start](#quick-start) • [Features](#key-features) • [Documentation](#documentation) • [Examples](#examples)

---

</div>

## Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Quick Start](#quick-start)
- [Architecture](#architecture)
- [AI Agent Support](#ai-agent-support)
- [Enterprise Integrations](#enterprise-integrations)
- [Configuration Options](#configuration-options)
- [Documentation](#documentation)
- [Contributing](#contributing)

---

## Overview

**FastAPI Fullstack Generator** is a powerful CLI tool that scaffolds production-ready full-stack applications with AI capabilities. Built for developers who need enterprise-grade infrastructure without the boilerplate.

### Demo & Interface Preview

<div align="center">

#### Generator in Action

![Generator Demo](assets/app_start.gif)

#### Generated Application Interface

The generator creates a complete full-stack application with a modern, professional UI:

**API Documentation & Observability**
| FastAPI Swagger UI | Logfire Dashboard | LangSmith Dashboard |
|:---:|:---:|:---:|
| ![API Docs](assets/docs_2.png) | ![Logfire](assets/logfire.png) | ![LangSmith](assets/langsmith.png) |

**Chat Interface (AI Agent)**
| Light Mode | Dark Mode |
|:---:|:---:|
| ![Chat Light](assets/new_chat_light.png) | ![Chat Dark](assets/new_chat_dark.png) |

**Admin Panel & Monitoring**
| SQLAdmin Panel | Celery Flower |
|:---:|:---:|
| ![Admin](assets/admin.png) | ![Flower](assets/flower.png) |

**Authentication Pages**
| Register | Login |
|:---:|:---:|
| ![Register](assets/new_register.png) | ![Login](assets/new_login.png) |

</div>

### Why Choose This Generator?

| Feature | Benefit |
|---------|---------|
| ![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi) **Modern Stack** | FastAPI + Next.js 15 + React 19 + TypeScript |
| ![AI](https://img.shields.io/badge/AI-First-FF6F00?style=flat-square&logo=tensorflow) **AI-First** | Built-in support for PydanticAI, LangChain, LangGraph, and CrewAI |
| ![Security](https://img.shields.io/badge/Security-JWT%20%7C%20OAuth2-green?style=flat-square&logo=key) **Security** | JWT auth, OAuth2, rate limiting, CSRF protection out of the box |
| ![Observability](https://img.shields.io/badge/Observability-Logfire%20%7C%20LangSmith-blue?style=flat-square&logo=grafana) **Observability** | Logfire, LangSmith, Sentry, and Prometheus integration |
| ![Performance](https://img.shields.io/badge/Performance-Async--First-orange?style=flat-square&logo=speedtest) **Performance** | Async-first architecture with WebSocket streaming |
| ![Enterprise](https://img.shields.io/badge/Enterprise-Ready-purple?style=flat-square&logo=building) **Enterprise-Ready** | Admin panels, webhooks, background tasks, and more |

### Perfect For

- ![Startups](https://img.shields.io/badge/Startups-Ship%20Fast-blue?style=flat-square&logo=rocket) **Startups** - Ship MVPs fast with production-ready infrastructure
- ![Enterprise](https://img.shields.io/badge/Enterprise-Standardized-red?style=flat-square&logo=building) **Enterprise Teams** - Standardized project structure and best practices
- ![AI Dev](https://img.shields.io/badge/AI%20Dev-Pre--configured-green?style=flat-square&logo=brain) **AI Developers** - Pre-configured AI agent frameworks and tooling
- ![Full-Stack](https://img.shields.io/badge/Full--Stack-Complete-orange?style=flat-square&logo=code) **Full-Stack Developers** - Complete frontend + backend in one command

---

## Key Features

### AI Agent Frameworks

<div align="center">

| Framework | Provider Support | Best For |
|-----------|-----------------|----------|
| ![PydanticAI](https://img.shields.io/badge/PydanticAI-Type--Safe-blue?style=flat-square&logo=python) | OpenAI, Anthropic, OpenRouter | Type-safe agents, simple use cases |
| ![LangChain](https://img.shields.io/badge/LangChain-Complex%20Chains-green?style=flat-square&logo=link) | OpenAI, Anthropic | Complex chains, many integrations |
| ![LangGraph](https://img.shields.io/badge/LangGraph-State%20Machines-purple?style=flat-square&logo=diagram-project) | OpenAI, Anthropic | Multi-step reasoning, state machines |
| ![CrewAI](https://img.shields.io/badge/CrewAI-Multi--Agent-orange?style=flat-square&logo=users) | OpenAI, Anthropic | Multi-agent teams, complex workflows |

</div>

**Features:**
- ✅ Real-time WebSocket streaming
- ✅ Conversation persistence
- ✅ Custom tool/function calling
- ✅ Multi-provider LLM support
- ✅ Built-in observability

### Backend Architecture

```
┌─────────────────────────────────────────┐
│         FastAPI Application             │
├─────────────────────────────────────────┤
│  • Async-first architecture             │
│  • Repository + Service pattern         │
│  • Django-style CLI commands            │
│  • Auto-generated API documentation     │
└─────────────────────────────────────────┘
```

**Tech Stack:**
- ![FastAPI](https://img.shields.io/badge/FastAPI-High--Performance-005571?style=flat-square&logo=fastapi) **FastAPI** - High-performance async API framework
- ![Pydantic](https://img.shields.io/badge/Pydantic%20v2-Data%20Validation-92000B?style=flat-square&logo=pydantic) **Pydantic v2** - Data validation and settings
- ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-ORM-029CDB?style=flat-square&logo=sqlalchemy) **SQLAlchemy/SQLModel** - Database ORM
- ![Alembic](https://img.shields.io/badge/Alembic-Migrations-009639?style=flat-square&logo=alembic) **Alembic** - Database migrations
- ![JWT](https://img.shields.io/badge/JWT%20%2B%20OAuth2-Auth-000000?style=flat-square&logo=jsonwebtokens) **JWT + OAuth2** - Authentication & authorization

### Frontend Experience

```
┌─────────────────────────────────────────┐
│      Next.js 15 Application             │
├─────────────────────────────────────────┤
│  • React 19 + TypeScript                │
│  • Tailwind CSS v4                      │
│  • Dark/Light mode                      │
│  • Real-time WebSocket chat              │
│  • Responsive design                    │
└─────────────────────────────────────────┘
```

**Highlights:**
- ![TypeScript](https://img.shields.io/badge/TypeScript-Type--Safe-3178C6?style=flat-square&logo=typescript) **Type-Safe** - Full TypeScript coverage
- ![React](https://img.shields.io/badge/React%2019-Modern%20UI-61DAFB?style=flat-square&logo=react) **Modern UI** - Beautiful, accessible components
- ![WebSocket](https://img.shields.io/badge/WebSocket-Real--Time-010101?style=flat-square&logo=socket.io) **Real-Time** - WebSocket streaming for AI responses
- ![Responsive](https://img.shields.io/badge/Responsive-Mobile--First-FF6B6B?style=flat-square&logo=mobile) **Responsive** - Mobile-first design
- ![Themes](https://img.shields.io/badge/Themes-Dark%2FLight-FFA500?style=flat-square&logo=palette) **Themes** - Dark/light mode support

---

## Quick Start

### Installation

```bash
# Using uv (recommended - fastest)
uv tool install fastapi-fullstack

# Or using pip
pip install fastapi-fullstack

# Or using pipx
pipx install fastapi-fullstack
```

### Generate Your First Project

```bash
# Interactive wizard (recommended for first-time users)
fastapi-fullstack new

# Quick mode with presets
fastapi-fullstack create my_ai_app --preset ai-agent --frontend nextjs

# Production-ready setup
fastapi-fullstack create my_ai_app --preset production

# Minimal setup (no extras)
fastapi-fullstack create my_ai_app --minimal
```

### Start Development

```bash
cd my_ai_app

# Install dependencies
make install

# Start database (Docker)
make docker-db

# Run migrations
make db-migrate
make db-upgrade

# Create admin user
make create-admin

# Start backend
make run

# In another terminal - start frontend
cd frontend
bun install && bun dev
```

**Access your application:**
- ![Frontend](https://img.shields.io/badge/Frontend-localhost:3000-blue?style=flat-square&logo=next.js) **Frontend**: http://localhost:3000
- ![API Docs](https://img.shields.io/badge/API%20Docs-localhost:8000/docs-green?style=flat-square&logo=swagger) **API Docs**: http://localhost:8000/docs
- ![Admin](https://img.shields.io/badge/Admin%20Panel-localhost:8000/admin-red?style=flat-square&logo=adminer) **Admin Panel**: http://localhost:8000/admin

---

## Architecture

### System Architecture

```mermaid
graph TB
    subgraph Client["Client Layer"]
        Browser[Web Browser]
        Mobile[Mobile App]
    end
    
    subgraph Frontend["Frontend - Next.js 15"]
        UI[React Components]
        WS[WebSocket Client]
        State[Zustand Store]
    end
    
    subgraph Backend["Backend - FastAPI"]
        API[REST API]
        WS_Server[WebSocket Server]
        Services[Business Logic]
        Repos[Data Access]
        Agents[AI Agents]
    end
    
    subgraph Infrastructure["Infrastructure"]
        DB[(PostgreSQL/MongoDB)]
        Cache[(Redis)]
        Queue[Task Queue]
    end
    
    subgraph External["External Services"]
        LLM[LLM Providers]
        Webhooks[Webhook Endpoints]
    end
    
    Browser --> UI
    UI --> API
    UI --> WS
    WS <--> WS_Server
    API --> Services
    WS_Server --> Agents
    Services --> Repos
    Agents --> LLM
    Repos --> DB
    Services --> Cache
    Services --> Queue
    Services --> Webhooks
```

### Code Organization

```
generated_project/
├── backend/
│   ├── app/
│   │   ├── api/          # REST endpoints
│   │   ├── agents/       # AI agent implementations
│   │   ├── core/         # Configuration & security
│   │   ├── db/           # Database models
│   │   ├── repositories/ # Data access layer
│   │   ├── services/     # Business logic
│   │   └── schemas/      # Pydantic models
│   ├── cli/              # Management commands
│   └── tests/            # Test suite
└── frontend/
    ├── src/
    │   ├── app/          # Next.js App Router
    │   ├── components/   # React components
    │   ├── hooks/        # Custom React hooks
    │   ├── stores/       # State management
    │   └── lib/          # Utilities
    └── e2e/              # End-to-end tests
```

---

## AI Agent Support

### Framework Comparison

| Feature | PydanticAI | LangChain | LangGraph | CrewAI |
|---------|-----------|-----------|-----------|--------|
| ![Type Safety](https://img.shields.io/badge/Type%20Safety-Native-success?style=flat-square) | ✅ Native | ⚠️ Manual | ⚠️ Manual | ⚠️ Manual |
| ![Multi-Agent](https://img.shields.io/badge/Multi--Agent-Supported-success?style=flat-square) | ❌ | ⚠️ Complex | ⚠️ Complex | ✅ Native |
| ![Tool Calling](https://img.shields.io/badge/Tool%20Calling-Supported-success?style=flat-square) | ✅ | ✅ | ✅ | ✅ |
| ![Streaming](https://img.shields.io/badge/Streaming-Supported-success?style=flat-square) | ✅ | ✅ | ✅ | ✅ |
| ![Memory](https://img.shields.io/badge/Memory-Built--in-success?style=flat-square) | ✅ Built-in | ✅ Chains | ✅ Checkpointer | ✅ Built-in |
| ![Complexity](https://img.shields.io/badge/Complexity-Level-info?style=flat-square) | Low | Medium | Medium | High |

### Quick Example

```python
# Generated agent code (PydanticAI example)
from pydantic_ai import Agent
from app.agents.tools import get_current_datetime

agent = Agent(
    model="openai:gpt-4o-mini",
    system_prompt="You are a helpful assistant.",
)

@agent.tool
async def current_time() -> str:
    """Get the current date and time."""
    return get_current_datetime()

# WebSocket streaming endpoint included
@router.websocket("/ws")
async def agent_ws(websocket: WebSocket):
    async for event in agent.iter(user_input):
        await websocket.send_json({"type": "token", "content": event.content})
```

---

## Enterprise Integrations

### Available Integrations

<div align="center">

| Category | Technologies |
|----------|------------|
| ![Databases](https://img.shields.io/badge/Databases-PostgreSQL%20%7C%20MongoDB%20%7C%20SQLite-blue?style=flat-square&logo=postgresql) | PostgreSQL, MongoDB, SQLite |
| ![Auth](https://img.shields.io/badge/Authentication-JWT%20%7C%20OAuth2%20%7C%20API%20Keys-green?style=flat-square&logo=key) | JWT, OAuth2 (Google), API Keys |
| ![Caching](https://img.shields.io/badge/Caching-Redis%20%7C%20fastapi--cache2-red?style=flat-square&logo=redis) | Redis, fastapi-cache2 |
| ![Observability](https://img.shields.io/badge/Observability-Logfire%20%7C%20LangSmith%20%7C%20Sentry-purple?style=flat-square&logo=grafana) | Logfire, LangSmith, Sentry, Prometheus |
| ![Tasks](https://img.shields.io/badge/Background%20Tasks-Celery%20%7C%20Taskiq%20%7C%20ARQ-orange?style=flat-square&logo=celery) | Celery, Taskiq, ARQ |
| ![Security](https://img.shields.io/badge/Security-Rate%20Limiting%20%7C%20CORS%20%7C%20CSRF-yellow?style=flat-square&logo=shield) | Rate limiting, CORS, CSRF protection |
| ![Admin](https://img.shields.io/badge/Admin-SQLAdmin%20Panel-teal?style=flat-square&logo=adminer) | SQLAdmin panel |
| ![Events](https://img.shields.io/badge/Events-Webhooks%20%7C%20WebSockets-cyan?style=flat-square&logo=webhook) | Webhooks, WebSockets |
| ![DevOps](https://img.shields.io/badge/DevOps-Docker%20%7C%20Kubernetes%20%7C%20CI%2FCD-indigo?style=flat-square&logo=docker) | Docker, Kubernetes, CI/CD |

</div>

### Integration Examples

```bash
# Enable specific integrations
fastapi-fullstack create my_app \
  --redis \
  --rate-limiting \
  --admin-panel \
  --sentry \
  --prometheus \
  --webhooks
```

---

## Configuration Options

### Core Configuration

| Option | Values | Default | Description |
|--------|--------|---------|-------------|
| ![Database](https://img.shields.io/badge/Database-Option-blue?style=flat-square&logo=database) **Database** | `postgresql`, `mongodb`, `sqlite`, `none` | `postgresql` | Database backend |
| ![ORM](https://img.shields.io/badge/ORM-Option-green?style=flat-square&logo=code) **ORM** | `sqlalchemy`, `sqlmodel` | `sqlalchemy` | ORM library |
| ![Auth](https://img.shields.io/badge/Auth-Option-red?style=flat-square&logo=key) **Auth** | `jwt`, `api_key`, `both`, `none` | `jwt` | Authentication method |
| ![AI](https://img.shields.io/badge/AI-Option-purple?style=flat-square&logo=brain) **AI Framework** | `pydantic_ai`, `langchain`, `langgraph`, `crewai` | `pydantic_ai` | AI agent framework |
| ![LLM](https://img.shields.io/badge/LLM-Option-orange?style=flat-square&logo=openai) **LLM Provider** | `openai`, `anthropic`, `openrouter` | `openai` | LLM service provider |
| ![Frontend](https://img.shields.io/badge/Frontend-Option-cyan?style=flat-square&logo=next.js) **Frontend** | `none`, `nextjs` | `nextjs` | Frontend framework |
| ![Tasks](https://img.shields.io/badge/Tasks-Option-yellow?style=flat-square&logo=clock) **Background Tasks** | `none`, `celery`, `taskiq`, `arq` | `none` | Task queue system |

### Presets

```bash
# Production preset - everything enabled
fastapi-fullstack create my_app --preset production

# AI Agent preset - optimized for AI applications
fastapi-fullstack create my_app --preset ai-agent

# Minimal preset - bare bones
fastapi-fullstack create my_app --minimal
```

---

## Documentation

### Comprehensive Guides

| Document | Description |
|----------|-------------|
| ![Architecture](https://img.shields.io/badge/Architecture-Guide-blue?style=flat-square&logo=book) [Architecture](docs/architecture.md) | System design and patterns |
| ![Frontend](https://img.shields.io/badge/Frontend-Guide-green?style=flat-square&logo=react) [Frontend Guide](docs/frontend.md) | Next.js setup and components |
| ![AI Agent](https://img.shields.io/badge/AI%20Agent-Guide-purple?style=flat-square&logo=brain) [AI Agent Guide](docs/ai-agent.md) | Agent frameworks and tools |
| ![Observability](https://img.shields.io/badge/Observability-Guide-orange?style=flat-square&logo=chart-line) [Observability](docs/observability.md) | Monitoring and tracing |
| ![Deployment](https://img.shields.io/badge/Deployment-Guide-red?style=flat-square&logo=rocket) [Deployment](docs/deployment.md) | Production deployment |
| ![Development](https://img.shields.io/badge/Development-Guide-cyan?style=flat-square&logo=code) [Development](docs/development.md) | Local development setup |
| ![Changelog](https://img.shields.io/badge/Changelog-History-yellow?style=flat-square&logo=history) [Changelog](docs/CHANGELOG.md) | Version history |

### Quick Reference

- ![Interface](https://img.shields.io/badge/View%20Interface-Guide-blue?style=flat-square&logo=eye) [View Interface Guide](VIEW_INTERFACE.md) - See the generated app in action
- ![Review](https://img.shields.io/badge/Repository-Review-green?style=flat-square&logo=file-text) [Repository Review](REPO_REVIEW.md) - Detailed repository analysis
- ![Contributing](https://img.shields.io/badge/Contributing-Guide-purple?style=flat-square&logo=handshake) [Contributing Guide](CONTRIBUTING.md) - How to contribute

---

## Examples

### Example 1: AI Chatbot Application

```bash
fastapi-fullstack create chatbot_app \
  --preset ai-agent \
  --ai-framework pydantic_ai \
  --llm-provider openai \
  --frontend nextjs \
  --database postgresql \
  --auth jwt \
  --websockets
```

**Result:** Full-stack chatbot with real-time streaming, conversation history, and user authentication.

### Example 2: Enterprise SaaS Platform

```bash
fastapi-fullstack create saas_platform \
  --preset production \
  --database postgresql \
  --auth jwt \
  --oauth-google \
  --redis \
  --admin-panel \
  --sentry \
  --prometheus \
  --kubernetes
```

**Result:** Production-ready SaaS with admin panel, monitoring, and Kubernetes deployment configs.

### Example 3: Minimal API Service

```bash
fastapi-fullstack create api_service \
  --minimal \
  --database postgresql \
  --auth api_key \
  --frontend none
```

**Result:** Lightweight API service with authentication and database support.

---

## Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details.

### How to Contribute

1. ![Fork](https://img.shields.io/badge/1.-Fork-blue?style=flat-square&logo=git-fork) Fork the repository
2. ![Branch](https://img.shields.io/badge/2.-Create%20Branch-green?style=flat-square&logo=git-branch) Create a feature branch (`git checkout -b feature/amazing-feature`)
3. ![Code](https://img.shields.io/badge/3.-Make%20Changes-purple?style=flat-square&logo=code) Make your changes
4. ![Test](https://img.shields.io/badge/4.-Run%20Tests-orange?style=flat-square&logo=test-tube) Run tests (`uv run pytest`)
5. ![Commit](https://img.shields.io/badge/5.-Commit-red?style=flat-square&logo=git-commit) Commit your changes (`git commit -m 'Add amazing feature'`)
6. ![Push](https://img.shields.io/badge/6.-Push-cyan?style=flat-square&logo=upload) Push to the branch (`git push origin feature/amazing-feature`)
7. ![PR](https://img.shields.io/badge/7.-Pull%20Request-yellow?style=flat-square&logo=git-pull-request) Open a Pull Request

---

<div align="center">

## Built with ❤️ by Ahmed Raoofuddin

[![Star](https://img.shields.io/badge/⭐-Star%20on%20GitHub-yellow?style=for-the-badge&logo=github)](https://github.com/AhmedRaoofuddin/Generator) • 
[![Bug](https://img.shields.io/badge/🐛-Report%20Bug-red?style=for-the-badge&logo=bug)](https://github.com/AhmedRaoofuddin/Generator/issues) • 
[![Discuss](https://img.shields.io/badge/💬-Discussions-blue?style=for-the-badge&logo=comments)](https://github.com/AhmedRaoofuddin/Generator/discussions) • 
[![Docs](https://img.shields.io/badge/📖-Documentation-green?style=for-the-badge&logo=book)](https://github.com/AhmedRaoofuddin/Generator#documentation)

**Generating production-ready AI applications since 2025**

---

[⬆ Back to Top](#fastapi-fullstack-generator)

</div>
