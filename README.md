# Intelligent Healthcare Diagnostic Assistant

> **AI & Software Engineering End-of-Semester Capstone Project**

An AI-powered healthcare diagnostic system that assists users by analyzing symptoms and providing possible medical condition predictions using machine learning.

The application combines a modern web interface, a secure backend API, and an intelligent diagnostic model to deliver fast and accurate predictions with confidence scores.

> **Disclaimer:** This project is developed for academic purposes only and should **not** be used as a substitute for professional medical advice.

---

## Project Overview

The system is composed of four major components:

- **AI Engine** – Processes datasets, trains the model, and performs diagnosis.
- **Backend API** – Handles business logic, database operations, authentication, and communication with the AI model.
- **Frontend** – Provides an intuitive interface for patient symptom submission and result visualization.
- **DevOps & QA** – Maintains development workflow, testing, CI/CD, and code quality.

---

## Repository Structure

```text
Capstone-Project-Intelligent-Healthcare-Diagnostic-Assistant/
│
├── .github/
│   └── workflows/              # GitHub Actions CI/CD workflows
│
├── ai_engine/                  # AI / Machine Learning
│   ├── data/
│   │   ├── raw/
│   │   └── processed/
│   ├── models/
│   ├── preprocess.py
│   ├── train.py
│   └── predict.py
│
├── backend/                    # Backend API
│   ├── config/
│   ├── api/
│   ├── models/
│   ├── manage.py
│   └── .env.example
│
├── frontend/                   # React / Next.js Frontend
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── styles/
│   ├── package.json
│   └── next.config.js
│
├── docs/                       # Project Documentation
│   ├── architecture_diagram.png
│   └── system_design_spec.md
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Team Roles

| Role | Responsibilities |
|------|------------------|
| Project Manager | Project planning, documentation, code reviews, Trello management, final integration |
| AI/ML Engineer | Dataset preparation, preprocessing, model training, evaluation, inference |
| Backend Developer | API development, database management, authentication, AI integration |
| Frontend Developer | User interface development, responsiveness, API integration |
| DevOps & QA | Git workflow, testing, CI/CD, linting, code quality |

---

## Tech Stack

### Frontend
- Next.js
- React
- Tailwind CSS

### Backend
- Django
- Django REST Framework

### Machine Learning
- Python
- Scikit-learn
- Pandas
- NumPy

### Database
- SQLite

### Version Control
- Git
- GitHub

### DevOps
- GitHub Actions

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Biden254/Capstone-Project-Intelligent-Healthcare-Diagnostic-Assistant.git

cd Capstone-Project-Intelligent-Healthcare-Diagnostic-Assistant
```

---

### 2. Create a Virtual Environment

#### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

#### Linux/macOS

```bash
python3 -m venv venv

source venv/bin/activate
```

Install the project dependencies:

```bash
pip install -r requirements.txt
```

---

### 3. Install Frontend Dependencies

```bash
cd frontend

npm install
```

---

## Running the Project

### Backend

```bash
cd backend

python manage.py runserver
```

### Frontend

```bash
cd frontend

npm run dev
```

### AI Model

```bash
cd ai_engine

python train.py
```

---

## Git Workflow

To maintain a clean Git history, **never push directly to `main` or `dev`.**

Always create a feature branch from `dev`.

Example:

```bash
git checkout dev

git pull origin dev

git checkout -b feature/frontend-intake-form
```

Other examples:

```bash
feature/backend-auth-api

feature/ai-model-training

feature/devops-testing
```

Push your work:

```bash
git push origin feature/your-branch-name
```

Finally, open a Pull Request targeting the **dev** branch.

---

## Pull Request Checklist

Before requesting a review, ensure:

- [ ] Project builds successfully.
- [ ] Code has been tested locally.
- [ ] No unnecessary files are committed.
- [ ] Code follows project conventions.
- [ ] Pull Request targets the `dev` branch.
- [ ] Changes are clearly described.

---

## Development Guidelines

- Keep commits focused and meaningful.
- Follow the agreed project structure.
- Avoid creating unnecessary directories.
- Write readable, maintainable, and documented code.
- Test before opening a Pull Request.
- Ask for reviews whenever you're unsure.

---

## Documentation

Project documentation will be maintained inside the **`docs/`** directory and will include:

- Software Requirements Specification (SRS)
- Software Design Specification (SDS)
- Architecture Diagrams
- API Documentation
- User Manual
- Testing Documentation

---

## Contributing

1. Pull the latest changes from `dev`.
2. Create a feature branch.
3. Implement your changes.
4. Test locally.
5. Commit using meaningful commit messages.
6. Push your branch.
7. Open a Pull Request.

---