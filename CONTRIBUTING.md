# Contributing to WebCheck-OSINT

Thank you for your interest in contributing to WebCheck-OSINT – a powerful web analysis and OSINT tool. We welcome contributions of all kinds: new check modules, UI improvements, documentation, bug fixes, and feature suggestions.

## Getting Started

1. **Fork** the repository and clone it locally.
2. Install dependencies: `npm install`
3. Copy `.env.example` (if provided) to `.env` and configure any optional API keys (e.g., for VirusTotal, Shodan).
4. Start the development server: `npm run dev`

## Development Workflow

- We use **GitHub Flow**: create a feature branch from `main`, make your changes, and open a pull request.
- Write clear, descriptive commit messages (e.g., `feat: add DNS lookup module`, `fix: handle timeout in HTTP check`).
- Include tests for new features or bug fixes (if applicable).
- Update the documentation (README, API docs, or inline comments) to reflect your changes.

## Code Style

- **Frontend**: Svelte (with Astro) – use the existing component structure.
- **Backend**: Node.js (server.js) – follow standard JavaScript/Node.js best practices.
- **API**: The tool exposes a REST API; keep endpoints consistent with existing ones.
- **Modules**: Each check (e.g., SSL, headers, WHOIS) should be a separate function or module.

## Testing

- Run unit tests: `npm test` (if available).
- Manually test your changes in the UI and via the API.
- Ensure that existing checks remain functional.

## Pull Request Guidelines

- Describe **what** you changed and **why**.
- Link any related issues (e.g., `Closes #123`).
- Ensure your branch is up-to-date with `main`.
- The CI pipeline (if set up) will run linting and tests – fix any failures.

## Adding a New Check Module

We love new modules! To add one:

1. Create a new file in `api/modules/` (or relevant directory).
2. Implement the logic to fetch and analyze the data.
3. Expose the result via the API endpoint and display it in the UI.
4. Document the module in the README.

## Reporting Issues

- Use the GitHub issue tracker.
- Provide a clear title, description, steps to reproduce, and environment details (OS, Node version, browser).
- For security issues, follow the guidelines in **SECURITY.md**.

## Feature Requests

- Open an issue with the `enhancement` label.
- Describe the use case and potential benefits.
- We'll discuss and prioritise based on the project roadmap.

## Code of Conduct

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) – we are committed to a respectful and inclusive community.

## Need Help?

- Feel free to ask questions in the issue tracker or discussions.
- We aim to respond within 2 business days.

Your contributions make WebCheck-OSINT better for everyone. Thank you! 🌐
