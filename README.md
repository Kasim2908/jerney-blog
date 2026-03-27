# jerney-blog

Monorepo for the Jerney blog platform.

This repository contains a full-stack blog app under the `Jerney/` directory:
- Frontend: React + Vite
- Backend: Node.js + Express
- Database: PostgreSQL
- Deployment assets: Nginx config and EC2 setup script

## Repository Structure

```
jerney-blog/
├── README.md
└── Jerney/
	├── README.md
	├── backend/
	├── frontend/
	└── deploy/
```

## Quick Start (Local)

### 1) Backend

```bash
cd Jerney/backend
npm install
```

Create environment variables for database connection and API port.

Example values:

```bash
DB_HOST=localhost
DB_PORT=5432
DB_USER=jerney_user
DB_PASSWORD=jerney_pass_2026
DB_NAME=jerney_db
PORT=5000
```

Start backend:

```bash
npm start
```

### 2) Frontend

```bash
cd Jerney/frontend
npm install
npm run dev
```

Frontend runs on `http://localhost:3000` (Vite).

## Deployment

For EC2 deployment, use:

```bash
cd Jerney
chmod +x deploy/setup.sh
./deploy/setup.sh
```

See `Jerney/README.md` for full deployment and architecture details.

## Git Remote

Configured remote:

```bash
origin: https://github.com/Kasim2908/jerney-blog.git
```
