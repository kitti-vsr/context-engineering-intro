### 🔄 Project Awareness & Context

- **Always read `PLANNING.md`** at the start of a new conversation to understand the project's architecture, goals, style, and constraints.
- **Check `TASK.md`** before starting a new task. If the task isn’t listed, add it with a brief description and today's date.
- **Use consistent naming conventions, file structure, and architecture patterns** as described in `PLANNING.md`.
- **Use the project's configured Node.js environment and package manager** whenever executing commands, including for tests.

### 🧱 Code Structure & Modularity

- **Never create a file longer than 500 lines of code.** If a file approaches this limit, refactor by splitting it into modules or helper files.
- **Organize code into clearly separated modules**, grouped by feature or responsibility.
- **Use clear, consistent imports** (prefer relative imports within packages).
- **Use clear, consistent imports** (prefer relative imports within packages).
- **Use environment variables through Next.js configuration and `.env` files**.

### 🧪 Testing & Reliability

- **Always create unit tests for new features** (functions, components, routes, etc.) using the project's configured testing framework.
- **After updating any logic**, check whether existing unit tests need to be updated. If so, do it.
- **Tests should live in a `/tests` folder** mirroring the main app structure.
  - Include at least:
    - 1 test for expected use
    - 1 edge case
    - 1 failure case

### ✅ Task Completion

- **Mark completed tasks in `TASK.md`** immediately after finishing them.
- Add new sub-tasks or TODOs discovered during development to `TASK.md` under a “Discovered During Work” section.

### 📎 Style & Conventions

- **Use TypeScript and Next.js** as the primary technologies.
- **Follow the project's ESLint and Prettier configuration**, use strict types, and maintain consistent formatting.
- **Use appropriate validation libraries** for data validation.
- Use **Next.js route handlers or Server Actions** for APIs, and use the project's configured database or ORM when applicable.
- Write **clear JSDoc comments for public functions and complex logic**:

  ```typescript
  /**
   * Brief summary.

   * @param param1 Description.
   * @returns Description.
   */
  function example(param1: string): string {
      return param1;
  }
  ```

### 📚 Documentation & Explainability

- **Update `README.md`** when new features are added, dependencies change, or setup steps are modified.
- **Comment non-obvious code** and ensure everything is understandable to a mid-level developer.
- When writing complex logic, **add an inline `# Reason:` comment** explaining the why, not just the what.

### 🧠 AI Behavior Rules

- **Never assume missing context. Ask questions if uncertain.**
- **Never hallucinate libraries or functions** – only use known, verified packages.
- **Always confirm file paths and module names** exist before referencing them in code or tests.
- **Never delete or overwrite existing code** unless explicitly instructed to or if part of a task from `TASK.md`.
