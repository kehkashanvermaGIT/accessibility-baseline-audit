# Accessibility Baseline & Repository Architecture Audit

## Project Overview

This repository contains an accessibility audit and a monorepo-style project skeleton for a web application.

The project is organized into separate client, server, documentation, and testing areas so that each part of the application has a clear responsibility.

## Repository Structure

```text
accessibility-audit/
├── client/
│   └── README.md
├── server/
│   └── README.md
├── docs/
│   ├── accessibility-audit.md
│   └── screenshots/
├── tests/
│   └── README.md
└── README.md
## Architecture Boundaries

### Client
The `client/` directory contains the frontend of the application.

Responsibilities:
- User interface
- User interactions
- Forms and page components
- Communication with the server/API

### Server
The `server/` directory contains backend functionality.

Responsibilities:
- API endpoints
- Application logic
- Data processing
- Server-side validation

### Docs
The `docs/` directory contains project documentation and accessibility audit evidence.

Responsibilities:
- Accessibility audit report
- Lighthouse screenshots
- Architecture documentation

### Tests
The `tests/` directory contains automated tests.

Responsibilities:
- Unit tests
- Integration tests
- API tests
- Validation of important application behaviour

## Local Setup

### Prerequisites
- Git
- A code editor
- Python 3
- A modern web browser

### Setup
Clone the repository and enter the project directory:

```bash
git clone https://github.com/kehkashanvermaGIT/accessibility-baseline-audit.git
cd accessibility-baseline-audit
```

## First Vertical Feature Slice

The first vertical feature slice will demonstrate communication between the frontend and backend.

### Flow

```text
User
  ↓
Client UI
  ↓
Server/API
  ↓
Application Logic
  ↓
Response
  ↓
Client UI
```

The initial implementation establishes the client-server boundary before more complex features are added.

## Accessibility Audit

The public-facing website selected for the audit was Engineering College Ajmer.

The detailed Lighthouse and keyboard-only accessibility findings are documented in `docs/accessibility-audit.md`.

Evidence screenshots are stored in `docs/screenshots/`.

## Development Approach

Frontend, backend, documentation, and testing are separated into clear repository boundaries. Future implementation can add application code, APIs, dependencies, configuration, and automated tests without changing the basic architecture.
