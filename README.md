# gh-events

Practice GitHub workflow trigger events with React and Vite

[![JavaScript](https://img.shields.io/badge/language-JavaScript-blue.svg)] [![React](https://img.shields.io/badge/react-18.2.0-green.svg)] [![License](https://img.shields.io/badge/license-MIT-yellow.svg)] [![npm](https://img.shields.io/npm/v/gh-events.svg)] [![GitHub Workflow Status](https://github.com/PartORG/gh-events/workflows/demo1.yml/badge.svg)] [![Code Climate Maintainability](https://api.codeclimate.com/v1/badges/your-badge-id/maintainability)] [![Test Coverage](https://img.shields.io/codecov/c/github/PartORG/gh-events.svg)] [![GitHub stars](https://img.shields.io/github/stars/PartORG/gh-events.svg?style=social&label=Stars)] [![GitHub forks](https://img.shields.io/github/forks/PartORG/gh-events.svg?style=social&label=Forks)]

## Introduction

`gh-events` is a practical example of using GitHub workflows to trigger events in a React application built with Vite. This project demonstrates how to set up continuous integration and delivery (CI/CD) pipelines, ensuring that your codebase remains robust and up-to-date.

The primary workflow involves:

1. **Development**: Writing and testing code locally.
2. **Build**: Compiling the application for production.
3. **Preview**: Serving the built application locally.
4. **Testing**: Running automated tests to ensure functionality.
5. **Deployment**: Triggering deployment events based on GitHub actions.

This project is ideal for developers looking to understand how to integrate GitHub workflows with modern web development frameworks like React and Vite.

## Features

### 1. React Application
- **What it does**: A simple React application showcasing event handling and state management.
- **Why it exists**: To demonstrate the use of React in a practical scenario.
- **Why it is useful**: Provides a solid foundation for building more complex applications.

### 2. Vite Integration
- **What it does**: Uses Vite for fast development server and build process.
- **Why it exists**: To leverage Vite's performance benefits during development.
- **Why it is useful**: Accelerates the development cycle, making it faster to see changes in real-time.

### 3. GitHub Actions Workflow
- **What it does**: Automates various tasks such as linting, testing, and deployment.
- **Why it exists**: To ensure code quality and automate repetitive tasks.
- **Why it is useful**: Reduces manual effort and minimizes the risk of human error.

## How It Works

The project uses Vite for development and production builds. The GitHub Actions workflow triggers on various events such as push, pull request, and release creation. Here's a high-level overview:

1. **Development**:
   - Run `npm run dev` to start the development server.
   - Changes are hot-reloaded in real-time.

2. **Build**:
   - Run `npm run build` to compile the application for production.
   - The output is placed in the `dist` directory.

3. **Preview**:
   - Run `npm run preview` to serve the built application locally.
   - This allows you to test the final product before deployment.

4. **Testing**:
   - Run `npm run test` to execute automated tests.
   - The tests are written using Jest and React Testing Library.

5. **Deployment**:
   - GitHub Actions triggers on specific events (e.g., push to main branch).
   - Deployment can be configured to various platforms like Netlify, Vercel, or AWS.

## Technology Stack

| Technology | Purpose |
|------------|---------|
| **React** | JavaScript library for building user interfaces. |
| **Vite** | Build tool that aims to provide a faster and leaner development experience for modern web projects. |
| **prop-types** | Runtime type checking for React props. |
| **Jest** | Testing framework for JavaScript applications. |
| **React Testing Library** | Testing utilities for React components. |
| **ESLint** | Tool for identifying and reporting on patterns found in ECMAScript/JavaScript code, with the goal of making code more consistent and avoiding errors. |

## Requirements

- Node.js 14 or higher
- npm (comes with Node.js)

## Installation

To get started, clone the repository and install dependencies:

```bash
git clone https://github.com/PartORG/gh-events.git
cd gh-events
npm install
```

## Configuration

No additional configuration is required for this project.

## Quick Start

1. **Start Development Server**:
   ```bash
   npm run dev
   ```

2. **Build for Production**:
   ```bash
   npm run build
   ```

3. **Preview Build Locally**:
   ```bash
   npm run preview
   ```

4. **Run Tests**:
   ```bash
   npm run test
   ```

## Usage

### Development

To start the development server, simply run:

```bash
npm run dev
```

This will open a new tab in your browser at `http://localhost:3000`, showing the application.

### Build and Preview

After making changes, build the project for production:

```bash
npm run build
```

Preview the built application locally:

```bash
npm run preview
```

### Testing

Run automated tests to ensure everything works as expected:

```bash
npm run test
```

## Project Structure

```
gh-events/
├── .eslintrc.json
├── .github/workflows/demo1.yml
├── .gitignore
├── index.html
├── package-lock.json
├── package.json
├── public/vite.svg
├── src/
│   ├── App.jsx
│   ├── assets/
│   │   └── images/logo.png
│   ├── components/
│   │   ├── HelpArea.css
│   │   ├── HelpArea.jsx
│   │   ├── HelpBox.css
│   │   ├── HelpBox.jsx
│   │   └── MainContent.jsx
│   │       └── MainContent.test.jsx
│   ├── index.css
│   └── main.jsx
├── src/test/
│   └── setup.js
└── vite.config.js
```

- **src/**: Contains the source code of the React application.
- **public/**: Static files like `index.html`.
- **.github/workflows/demo1.yml**: GitHub Actions workflow configuration.

## Development

The development workflow involves:

1. **Coding**: Write your React components and logic in `src/`.
2. **Testing**: Use Jest and React Testing Library to write tests.
3. **Linting**: Run ESLint to ensure code quality.
4. **Preview**: Use `npm run dev` to see changes in real-time.

## Testing

This project includes automated tests using Jest and React Testing Library:

- Unit tests for components are located in the same directory as the component files.
- Integration tests can be added in the `src/test/` directory.

## Limitations

- This is a basic example, so it may not cover all edge cases.
- Continuous deployment is configured but requires additional setup for specific platforms.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.