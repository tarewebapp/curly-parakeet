# Contributing to T-ARE Website

Thank you for your interest in contributing to the T-ARE Trading and Consultancy website! This document provides guidelines and instructions for contributing.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Setup](#development-setup)
- [How to Contribute](#how-to-contribute)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Pull Request Process](#pull-request-process)
- [Issue Guidelines](#issue-guidelines)
- [Code Style](#code-style)
- [Questions?](#questions)

---

## Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment. Please be considerate of others and follow standard open-source community guidelines.

---

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Git
- Basic knowledge of HTML, CSS, and JavaScript

### Quick Start

```bash
# Clone the repository
git clone https://github.com/your-username/curly-parakeet.git
cd curly-parakeet

# Open the project in your browser
open index.html
# or
python -m http.server 8000
```

No build step is required — this is a static website.

---

## Development Setup

1. Fork the repository
2. Clone your fork locally
3. Create a new branch from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. Make your changes
5. Test thoroughly in multiple browsers
6. Commit your changes using our [commit message guidelines](#commit-message-guidelines)
7. Push to your fork and open a Pull Request

---

## How to Contribute

### Reporting Bugs

- Use the **Bug Report** issue template
- Include steps to reproduce, expected vs actual behavior
- Add screenshots if possible
- Mention your browser and device

### Suggesting Features

- Use the **Feature Request** issue template
- Clearly explain the problem you're trying to solve
- Describe your proposed solution

### Improving Documentation

- Documentation improvements are always welcome
- Follow the existing style and tone

### Code Contributions

- Follow our existing code style
- Write clear, self-documenting code
- Add comments for complex logic
- Test your changes across different screen sizes

---

## Commit Message Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.

### Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Common Types

| Type       | Description                     |
|------------|---------------------------------|
| `feat`     | New feature                     |
| `fix`      | Bug fix                         |
| `docs`     | Documentation only              |
| `style`    | Formatting, no code change      |
| `refactor` | Code refactoring                |
| `perf`     | Performance improvement         |
| `chore`    | Maintenance / tooling           |

### Example

```bash
git commit -m "feat(hero): add staggered entrance animation to logo bars"
git commit -m "fix(form): add missing autocomplete attributes"
git commit -m "docs(brand): update DNS configuration guide"
```

See [`.github/COMMIT_TEMPLATE.md`](.github/COMMIT_TEMPLATE.md) for the full template.

---

## Pull Request Process

1. **Create a Pull Request** from your feature branch to `main`
2. **Fill out the PR Template** completely
3. **Ensure all status checks pass** (`Lint & Validate`)
4. **Request review** (if applicable)
5. **Address review feedback** promptly
6. Once approved, your PR will be merged

### Requirements

- All CI checks must pass
- Branch must be up to date with `main`
- PR description must follow the template
- At least one approval is required (for team projects)

See [`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md) for the template.

---

## Issue Guidelines

We use structured issue templates to keep things organized:

- **Bug Report** – For reporting issues
- **Feature Request** – For suggesting new features or improvements

Please use the appropriate template when opening an issue.

---

## Code Style

- Use **semantic HTML**
- Follow existing **CSS naming conventions**
- Keep JavaScript **vanilla** and lightweight
- Use **meaningful variable and function names**
- Add comments for complex logic
- Maintain **mobile-first** responsive design

---

## Questions?

If you have any questions or need help getting started:

- Open an issue with the label `question`
- Reach out via email: info@t-areph.com

---

Thank you for contributing to T-ARE! Your efforts help us maintain a high-quality, professional website.

---

*Last updated: June 2026*