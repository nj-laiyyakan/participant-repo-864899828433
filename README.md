# Monorepo Project

This monorepo contains a FastAPI backend and AWS CDK infrastructure.

## Structure

```
.
├── backend/           # FastAPI REST API
├── infrastructure/    # AWS CDK TypeScript IaC
└── README.md
```

## Backend

FastAPI-based REST API with Python.

**Dependencies:**
- FastAPI 0.115.0
- Pydantic 2.9.2
- boto3 1.35.36
- uvicorn 0.32.0

See [backend/README.md](backend/README.md) for setup instructions.

## Infrastructure

AWS CDK TypeScript project for infrastructure-as-code.

See [infrastructure/README.md](infrastructure/README.md) for setup instructions.

## Getting Started

### Backend Setup
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Infrastructure Setup
```bash
cd infrastructure
npm install
npm run build
npx cdk synth
```

## Git

This repository is initialized with git. Use standard git commands to manage version control.
