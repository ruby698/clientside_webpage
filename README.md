# insta485 - Instagram Clone

A full-stack Instagram clone built with React (frontend) and Flask (backend), featuring real-time interactions like likes, comments, and infinite scroll.

## Overview

**insta485** is an educational project demonstrating modern web development practices with a focus on:
- **Frontend**: React component architecture with dynamic state management
- **Backend**: Flask RESTful API with database integration
- **Testing**: Comprehensive end-to-end testing with Cypress
- **Code Quality**: ESLint, Prettier, and Python linting

## Features

- **User Authentication**: Login/logout and account management
- **Posts**: Create, view, edit, and delete posts with image uploads
- **Interactions**: Like and comment on posts in real-time
- **Social Features**: Follow/unfollow users, view follower/following lists
- **Infinite Scroll**: Lazy-loaded feed for better performance
- **REST API**: Complete REST API for all operations

## Tech Stack

### Frontend
- **React 18** - UI library
- **Webpack** - Module bundler
- **Babel** - JavaScript transpiler
- **ESLint & Prettier** - Code quality & formatting
- **Cypress** - End-to-end testing

**Node.js**: >= 22.0.0  
**Package Manager**: npm

### Backend
- **Flask** - Web framework
- **SQLite** - Database (via schema.sql)
- **Python** - >= 3.12

**Dependencies**: Arrow, BeautifulSoup4, Markdown, pytest, requests, and more

## Quick Start

### Prerequisites
- Node.js >= 22.0.0
- Python >= 3.12
- npm

### Installation

```bash
# Install frontend dependencies
npm install

# Install backend dependencies
pip install -r requirements.txt
```

### Running the Application

```bash
# Build frontend (webpack)
npm run build

# Start backend server (Flask)
flask run

# In another terminal, run tests
npm run test
```

### Running Tests

```bash
# Unit and integration tests
npm run test

# Cypress E2E tests
npm run cypress:open
```

## Project Structure

```
insta485/
├── api/                    # REST API endpoints
├── js/                     # React components and main.jsx
├── static/                 # Static assets (CSS, images)
│   ├── css/
│   └── images/
├── templates/              # HTML templates
├── views/                  # Flask view handlers
├── config.py               # Configuration
├── model.py                # Database models
└── __init__.py             # Flask app initialization

sql/
├── schema.sql              # Database schema
└── data.sql                # Sample data

tests/
├── cypress/                # End-to-end tests
├── test_*.py               # Python unit tests
└── conftest.py             # Pytest configuration

docs/
├── images/                 # Documentation images & architecture diagrams
└── ...                     # Additional documentation

Config Files:
├── package.json            # Frontend dependencies
├── pyproject.toml          # Backend project config
├── requirements.txt        # Python dependencies
├── tsconfig.json           # TypeScript configuration
├── webpack.config.js       # Webpack build config
├── cypress.config.js       # Cypress configuration
└── .eslintrc               # Linting rules
```

## Documentation

All documentation images and diagrams are located in [`docs/images/`](docs/images/). Key diagrams include:

- **API Architecture**: RESTful endpoint diagrams
- **Component Hierarchy**: React component structure
- **Database Schema**: Entity relationship diagrams
- **UI Mockups**: Application screenshots

## Development Workflow

1. **Frontend Development**: Modify React components in `insta485/js/`
2. **Backend Development**: Update Flask views in `insta485/views/`
3. **Testing**: Run Cypress tests for E2E validation and Python tests for unit testing
4. **Building**: Use `npm run build` to bundle frontend code with Webpack

## Scripts

```bash
npm run build          # Build frontend with Webpack
npm run start          # Start development server
npm run test           # Run Cypress tests
npm run cypress:open   # Open Cypress Test Runner
npm run lint           # Run ESLint
npm run format         # Format code with Prettier
```

## License

MIT

## Authors

- awdeorio (Original author)
- Team contributions via live coding sessions

---

For more details on project decisions and development experiences, see the [original project documentation](https://github.com/awdeorio).
