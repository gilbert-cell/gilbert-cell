# Secure E-Commerce Platform

A full-stack e-commerce application with a Django REST Framework API,
a React client, and biometric facial-recognition verification at checkout.

## Features
- Secure user authentication and role-based access control
- Per-user data scoping: customers can only access their own orders
- Product catalogue, cart and order management
- Biometric facial-recognition verification before payment
- Transactions stored in PostgreSQL

## Tech stack
| Layer | Technology |
|-------|-----------|
| Backend | Python, Django, Django REST Framework |
| Frontend | React.js |
| Database | PostgreSQL |

## Architecture
React client → REST API (Django REST Framework) → PostgreSQL.
Facial verification runs as part of the checkout flow.
See `docs/` for the architecture and use-case diagrams.

## Getting started
```bash
git clone https://github.com/gilbert-cell/E-commerce-Application.git
cd E-commerce-Application

# Backend
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env        # add your own database settings and secret key
python manage.py migrate
python manage.py runserver

# Frontend
cd <frontend-folder>
npm install
npm start
```

## Author
Eusebius Gilbert Mathias
[github.com/gilbert-cell](https://github.com/gilbert-cell)


# AI-Powered SIEM

A Security Information and Event Management prototype that collects,
analyses and correlates security logs, using machine learning to detect
anomalies and classify attacks.

## Features
- Log collection and storage
- Event correlation to link related security events
- ML-based anomaly detection and attack classification
- Automated threat detection and alerting
- Dashboard built with React

## Tech stack
Python, Django, PostgreSQL, React.js, machine learning

## Documentation
The `docs/` folder contains the design work done before implementation:
- A requirements specification of 133+ functional, non-functional,
  ML and security requirements
- System architecture diagrams
- Use-case diagram (Security Administrator, System Administrator, Auditor)

## Getting started
```bash
git clone https://github.com/gilbert-cell/AI-POWERED-SIEMS.git
cd AI-POWERED-SIEMS
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
cp .env.example .env        # add your own database settings and secret key
python manage.py migrate
python manage.py runserver


## Author
Eusebius Gilbert Mathias
[github.com/gilbert-cell](https://github.com/gilbert-cell)
