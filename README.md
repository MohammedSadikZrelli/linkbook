# Linkbook

Tunisian student book exchange platform.

## Prerequisites

- Node.js v18+
- MongoDB (local or [Atlas](https://mongodb.com/atlas))

## Setup

```bash
# Install dependencies
cd server && npm install
cd ../frontend && npm install
cd ..

# Create environment file
cp .env.example server/.env
# Edit server/.env with your values
```

## Run

```bash
# Terminal 1 - Backend
cd server && npm run dev

# Terminal 2 - Frontend
cd frontend && npm run dev
```

Backend: http://localhost:5000  
Frontend: http://localhost:5173

## Environment Variables

| Variable | Required | Default |
|----------|----------|---------|
| `PORT` | No | 5000 |
| `MONGO_URI` | No | `mongodb://127.0.0.1:27017/linkbook` |
| `JWT_SECRET` | Yes | — |
| `EMAIL_USER` | No | Email for password reset |
| `EMAIL_APP_PASSWORD` | No | Email app password |
| `GOOGLE_CLIENT_ID` | No | Google OAuth |
| `GOOGLE_CLIENT_SECRET` | No | Google OAuth |
| `GEMINI_API_KEY` | No | AI chat feature |
| `CLOUDFLARE_ACCOUNT_ID` | No | Image upload |
| `CLOUDFLARE_API_TOKEN` | No | Image upload |
