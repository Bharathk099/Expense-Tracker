# AGENTS.md — Expense Tracker

## Project Overview
- Project: Expense Tracker
- Stack: React, Vite, JavaScript, Vitest, React Testing Library, Cypress.

## Project Structure
- `src/App.jsx`: Main application and expense state.
- `src/App.css`: Application component styling.
- `src/index.css`: Global styling.
- `src/components/`: Reusable UI components.
- `src/utils/`: Reusable validation and calculation functions.
- `src/__tests__/`: Unit and component tests.
- `cypress/e2e/`: End-to-end tests.
- `AGENTS.md`: Coding-agent instructions.
- `prompts.md`: Reusable agent prompts.

## Application Requirements
- Add expenses with a title, amount, and category.
- Categories: Food, Travel, Bills, Other.
- Reject blank titles, non-numeric amounts, zero, negative values, and amounts above ₹1,00,000.
- Display expenses, running total, category filter, delete controls, and visible count.
- Format currency amounts to two decimal places.
- Keep the total and count consistent with the currently displayed expenses.

## Coding Conventions
- Use React functional components and hooks.
- Keep main application state in `App.jsx`.
- Use one component per file.
- Use clear, descriptive variable and function names.
- Add a short comment explaining the props and state responsibilities of each retained component.
- Keep reusable business logic in utility functions.
- Use accessible labels and stable `data-cy` attributes.
- Avoid unnecessary abstractions and unrelated features.

## Agent Rules
- Inspect existing files and Git status before changing anything.
- Explain the plan and wait for approval before implementation.
- Never overwrite uncommitted user changes.
- Never work directly on `main` for feature development.
- Use a separate branch for each scoped feature.
- Do not install additional dependencies without permission.
- Do not commit, push, merge, or open a pull request without explicit approval.
- Review diffs and run relevant tests after each feature.
- Report actual test results honestly.
- Summarize changes and provide a pull-request description after each task.

## Commands
- Install dependencies: `npm install`
- Start development server: `npm run dev`
- Production build: `npm run build`
- Lint: `npm run lint`
- Unit tests: `npx vitest run`
- Unit test coverage: `npx vitest run --coverage`
- Cypress interactive mode: `npm run cy:open`
- Cypress headless mode: `npm run cy:run`

Check `package.json` before using any test command. Configure missing scripts or tools only after obtaining approval.

## Testing Requirements
- Write meaningful tests for validation, totals, adding, filtering, deletion, and invalid input.
- Include a test-first exercise for rejecting amounts above ₹1,00,000.
- Use Cypress to test the main user journey and invalid input.
- Never change a test merely to make an implementation pass.
- Verify failures occur for the expected reasons.

## Git Workflow
- Keep `main` as the stable branch.
- Commit the starter project before feature development.
- Create a feature branch for each task.
- Review `git diff`, run tests, and request approval before committing.
- Use pull requests for proposed changes to `main`.