```markdown
# skills-secure-code-game Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill demonstrates best practices for developing secure code in TypeScript, focusing on consistent code style, modular file organization, and test-driven development. The repository provides a foundation for building secure code games or exercises, emphasizing maintainability and clarity.

## Coding Conventions

### File Naming
- Use **kebab-case** for all file names.
  - Example: `secure-code-utils.ts`, `game-engine.ts`

### Import Style
- Use **relative imports** for referencing modules within the project.
  - Example:
    ```typescript
    import { validateInput } from './input-validator';
    ```

### Export Style
- Use **named exports** for all exported functions, classes, or constants.
  - Example:
    ```typescript
    export function validateInput(input: string): boolean { ... }
    ```

### Commit Messages
- Commit messages are **freeform** and may or may not use prefixes.
- Average commit message length is about 63 characters.

## Workflows

### Adding a New Secure Code Challenge
**Trigger:** When you want to add a new secure coding exercise to the game.
**Command:** `/add-challenge`

1. Create a new file in `challenges/` using kebab-case (e.g., `sql-injection-challenge.ts`).
2. Implement the challenge logic using named exports.
3. Add a corresponding test file (e.g., `sql-injection-challenge.test.ts`).
4. Import and register the new challenge in the main game logic file.
5. Commit your changes with a descriptive message.

### Running Tests
**Trigger:** When you want to verify code correctness.
**Command:** `/run-tests`

1. Ensure all test files follow the `*.test.*` naming pattern.
2. Use the project's test runner (framework unknown; check project docs or scripts).
3. Run the test command (e.g., `npm test` or equivalent).
4. Review test output and address any failures.

## Testing Patterns

- Test files are named with the `*.test.*` pattern (e.g., `input-validator.test.ts`).
- The specific testing framework is not detected; refer to project documentation or scripts for details.
- Tests should cover both typical and edge-case scenarios for secure code challenges.

## Commands
| Command         | Purpose                                         |
|-----------------|-------------------------------------------------|
| /add-challenge  | Scaffold and add a new secure code challenge    |
| /run-tests      | Run all project tests                           |
```
