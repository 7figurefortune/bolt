# Contribution Guidelines

Welcome! This guide provides all the details you need to contribute effectively to the project. Thank you for helping us make **d3ploy** a better tool for developers worldwide. 💡

---

## 📋 Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [How Can I Contribute?](#how-can-i-contribute)
3. [Pull Request Guidelines](#pull-request-guidelines)
4. [Coding Standards](#coding-standards)
5. [Development Setup](#development-setup)
6. [Testing](#testing)
7. [Deployment](#deployment)

---

## 🛡️ Code of Conduct

This project is governed by our **Code of Conduct**. By participating, you agree to uphold this code. Report unacceptable behavior to the project maintainers.

---

## 🛠️ How Can I Contribute?

### 1️⃣ Reporting Bugs or Feature Requests

- Check the [issue tracker](#) to avoid duplicates.
- Use issue templates (if available).
- Provide detailed, relevant information and steps to reproduce bugs.

### 2️⃣ Code Contributions

1. Fork the repository.
2. Create a feature or fix branch.
3. Write and test your code.
4. Submit a pull request (PR).

### 3️⃣ Join as a Core Contributor

Interested in maintaining and growing the project? Fill out our [Contributor Application Form](https://forms.gle/TBSteXSDCtBDwr5m7).

---

## ✅ Pull Request Guidelines

### PR Checklist

- Branch from the **main** branch.
- Update documentation, if needed.
- Test all functionality manually.
- Focus on one feature/bug per PR.

### Review Process

1. Manual testing by reviewers.
2. At least one maintainer review required.
3. Address review comments.
4. Maintain a clean commit history.

---

## 📏 Coding Standards

### General Guidelines

- Follow existing code style.
- Comment complex logic.
- Keep functions small and focused.
- Use meaningful variable names.

---

## 🖥️ Development Setup

### 1️⃣ Initial Setup

- Clone the repository:
  ```bash
  git clone https://github.com/7figurefortune/bolt.git
  ```
- Install dependencies:
  ```bash
  pnpm install
  ```
- Set up environment variables:
  1. Rename `.env.example` to `.env.local`.
  2. Add your API keys:
     ```bash
     GROQ_API_KEY=XXX
     HuggingFace_API_KEY=XXX
     OPENAI_API_KEY=XXX
     ...
     ```
  4. Optionally set:
     - Debug level: `VITE_LOG_LEVEL=debug`
     - Context size: `DEFAULT_NUM_CTX=32768`

**Note**: Never commit your `.env.local` or `.env` files to version control. They're already in `.gitignore`.

### 2️⃣ Run Development Server

```bash
pnpm run dev
```

**Tip**: Use **Google Chrome Canary** for local testing.

---

## 🧪 Testing

Run the test suite with:

```bash
pnpm test
```

---

## 🚀 Deployment

### Deploy to Cloudflare Pages

```bash
pnpm run deploy
```

Ensure you have required permissions and that Wrangler is configured.

---



## 🔑 Environment Variables

Ensure `.env.local` is configured correctly with:

- API keys.
- Context-specific configurations.

Example for the `DEFAULT_NUM_CTX` variable:

```bash
DEFAULT_NUM_CTX=24576 # Uses 32GB VRAM
```
