# Paypal Payment Integration Demo

## Project Objectives
- Validate PayPal payment flows (one-time and recurring) interactively with a Jupyter notebook.
- Integrate and test the verified payment logic in a FastAPI backend and Next.js frontend application.
- Provide seamless end-to-end testing both locally and via Docker Compose.

## Clone from GitHub
```bash
git clone https://github.com/NoManNayeem/PayPal_Subscription.git
cd PayPal_Subscription
```

## Run Locally

### Jupyter Notebook
```bash
cd Notebook
pip install -r requirements.txt
jupyter notebook PayPal_Subscription_Notebook.ipynb
```

### FastAPI + Next.js App

#### Backend (FastAPI)
```bash
cd Backend-FastAPI
pip install -r requirements.txt
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

#### Frontend (Next.js)
```bash
cd frontend-nextjs
npm install
npm run dev
```

## Run with Docker Compose

Ensure Docker and Docker Compose are installed.

```bash
docker-compose up --build
```

This will:
- Launch the Jupyter notebook service at http://localhost:8888
- Start the FastAPI backend at http://localhost:8000
- Serve the Next.js frontend at http://localhost:3000
