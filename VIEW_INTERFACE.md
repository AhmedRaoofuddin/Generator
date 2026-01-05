# 🖥️ Viewing the Generated Application Interface

This guide shows you how to generate a project and view its beautiful UI interface.

## Quick Start - See It In Action

### Step 1: Generate a Demo Project

```bash
# From the generator root directory
uv run python -m fastapi_gen.cli create demo_app \
  -o .demo_out \
  --preset ai-agent \
  --frontend nextjs \
  --database postgresql \
  --auth jwt \
  --websockets
```

### Step 2: Navigate to Generated Project

```bash
cd .demo_out/demo_app
```

### Step 3: Start the Application

#### Option A: Using Docker (Recommended - Easiest)

```bash
# Start backend + database + redis
docker-compose up -d

# Wait a few seconds for services to start, then:
# Create database migrations
docker-compose exec backend alembic upgrade head

# Create admin user
docker-compose exec backend uv run demo_app user create-admin
# Enter email: admin@example.com
# Enter password: (your choice)

# Start frontend (in a new terminal)
cd frontend
bun install
bun dev
```

#### Option B: Manual Setup

```bash
# Terminal 1: Start PostgreSQL
docker run -d \
  --name postgres-demo \
  -e POSTGRES_PASSWORD=secret \
  -e POSTGRES_DB=demo_app \
  -p 5432:5432 \
  postgres:16-alpine

# Terminal 2: Backend
cd backend
uv sync
cp .env.example .env
# Edit .env and set your OPENAI_API_KEY if using AI agent
alembic upgrade head
uv run demo_app user create-admin
uv run uvicorn app.main:app --reload

# Terminal 3: Frontend
cd frontend
bun install
bun dev
```

### Step 4: Access the Interfaces

Once everything is running, open your browser:

#### 🎨 Frontend Application
**URL**: http://localhost:3000

**What you'll see:**
- Beautiful landing page
- Login/Register pages
- Dashboard with AI chat interface
- Real-time WebSocket streaming
- Dark/Light mode toggle
- Responsive design

#### 📚 API Documentation
**URL**: http://localhost:8000/docs

**What you'll see:**
- Interactive Swagger UI
- All API endpoints
- Try-it-out functionality
- Request/response schemas
- Authentication testing

#### 🔐 Admin Panel
**URL**: http://localhost:8000/admin

**What you'll see:**
- SQLAdmin interface
- Database tables
- User management
- CRUD operations
- Authentication required

#### 🏥 Health Check
**URL**: http://localhost:8000/api/v1/health

**What you'll see:**
- API health status
- Database connection status
- Service dependencies

## Interface Features

### Frontend (Next.js 15)

1. **Landing Page** (`/`)
   - Welcome screen
   - Feature highlights
   - Call-to-action buttons

2. **Authentication** (`/login`, `/register`)
   - Modern form design
   - Validation feedback
   - OAuth integration (if enabled)

3. **Dashboard** (`/dashboard`)
   - User profile
   - Navigation sidebar
   - Quick stats

4. **AI Chat Interface** (`/chat`)
   - Real-time streaming
   - Message history
   - Tool call visualization
   - Markdown rendering
   - Copy functionality

5. **Profile** (`/profile`)
   - User settings
   - Account management

### Backend (FastAPI)

1. **API Endpoints**
   - RESTful API design
   - Versioned routes (`/api/v1/`)
   - JWT authentication
   - Rate limiting

2. **WebSocket** (`/api/v1/agent/ws`)
   - Real-time AI agent streaming
   - Event-based communication
   - Connection management

3. **Admin Panel**
   - Database CRUD
   - User management
   - Model inspection

## Customization

### Change Colors/Branding

The generated frontend uses Tailwind CSS. Customize colors in:

```bash
# Frontend theme configuration
cd frontend/src/app/globals.css
# Edit CSS variables for colors

# Or update Tailwind config
cd frontend
# Edit tailwind.config.ts
```

### Modify UI Components

All React components are in:
```
frontend/src/components/
├── auth/          # Login/Register forms
├── chat/          # Chat interface
├── layout/        # Header, Sidebar
├── theme/         # Dark/Light mode
└── ui/            # Reusable components
```

### Update Branding

1. **Logo**: Replace `frontend/public/` logo files
2. **Favicon**: Update `frontend/public/favicon.ico`
3. **Title**: Edit `frontend/src/app/layout.tsx`
4. **Meta tags**: Update in `layout.tsx`

## Troubleshooting

### Frontend won't start
```bash
# Check if Bun is installed
bun --version

# If not, install it:
curl -fsSL https://bun.sh/install | bash
```

### Backend connection errors
```bash
# Check if PostgreSQL is running
docker ps | grep postgres

# Check environment variables
cd backend
cat .env
```

### Port already in use
```bash
# Change ports in docker-compose.yml or .env
# Backend: 8000
# Frontend: 3000
# PostgreSQL: 5432
```

## Next Steps

1. **Customize the UI**: Edit components in `frontend/src/components/`
2. **Add features**: Follow patterns in existing code
3. **Deploy**: Use Docker or cloud platforms
4. **Monitor**: Set up Logfire/LangSmith for observability

---

**Need help?** Check the generated project's `README.md` for detailed documentation.

