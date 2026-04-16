# Microcontroller Tracker

A web-based tracking system for microcontroller replacements on probers. Supports both single-serial and multi-part serial number tracking.

## Overview

This system tracks microcontroller replacements with:
- Single serial number tracking (1 serial per unit)
- Multi-part serial number tracking (3 parts per unit)
- Automated status transitions
- Prober integration
- Real-time analytics and alerts
- Comprehensive replacement history

## Tech Stack

- **Frontend**: React 18+ with TypeScript
- **Backend**: Node.js + Express
- **Database**: PostgreSQL 14+
- **Containerization**: Docker & Docker Compose
- **CI/CD**: GitHub Actions
- **Authentication**: JWT

## Quick Start

### Prerequisites
- Docker & Docker Compose
- Node.js 18+
- PostgreSQL 14+

### Development Setup

```bash
# Clone the repository
git clone https://github.com/SebastianCarrion-qorvo/microcontroller-tracker.git
cd microcontroller-tracker

# Start with Docker Compose
docker-compose up -d

# Install dependencies
cd backend && npm install
cd ../frontend && npm install

# Run migrations
cd ../backend && npm run migrate

# Start development servers
# Backend: npm run dev (from backend directory)
# Frontend: npm start (from frontend directory)
```

### Endpoints Documentation
See [API_DOCS.md](./docs/API_DOCS.md)

### Database Schema
See [DATABASE_SCHEMA.md](./docs/DATABASE_SCHEMA.md)

## Project Structure

```
microcontroller-tracker/
├── backend/                 # Node.js/Express API
├── frontend/                # React application
├── database/                # PostgreSQL migrations & seeds
├── .github/
│   └── workflows/           # GitHub Actions
├── docs/                    # Documentation
├── docker-compose.yml
└── README.md
```

## Features

### Core Features
- [x] Multi-part microcontroller tracking
- [x] QR code serial number scanning (planned)
- [x] Automated status transitions
- [x] Prober assignment
- [x] Replacement history tracking
- [x] Real-time notifications
- [x] Analytics dashboard

### Automation
- [x] Batch import (CSV/JSON)
- [x] Duplicate detection
- [x] Scheduled reports
- [x] Webhook integrations
- [x] Email/Slack notifications

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md)

## License

MIT
