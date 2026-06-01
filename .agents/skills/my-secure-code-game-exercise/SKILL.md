```markdown
# my-secure-code-game-exercise Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill covers the development patterns and conventions used in the `my-secure-code-game-exercise` TypeScript repository. It documents file organization, code style, commit conventions, and testing patterns to help contributors write consistent, maintainable, and secure code. No framework is used, and the repository emphasizes clarity and modularity.

## Coding Conventions

### File Naming
- Use **camelCase** for all file names.
  - Example: `secureGameLogic.ts`, `userProfile.test.ts`

### Import Style
- Use **relative imports** for modules within the project.
  - Example:
    ```typescript
    import { validateMove } from './gameUtils';
    ```

### Export Style
- Use **named exports** for all modules.
  - Example:
    ```typescript
    // In gameUtils.ts
    export function validateMove(move: string): boolean { ... }
    ```

### Commit Messages
- Follow **conventional commit** format.
- Use the `build` prefix for build-related changes.
- Keep commit messages concise (average ~76 characters).
  - Example:
    ```
    build: update TypeScript configuration for stricter type checks
    ```

## Workflows

### Code Contribution
**Trigger:** When adding or updating code in the repository  
**Command:** `/contribute`

1. Create or update files using camelCase naming.
2. Use relative imports and named exports.
3. Write or update tests in files matching `*.test.*`.
4. Commit changes using the conventional commit format (e.g., `build: ...`).
5. Push changes and open a pull request.

### Testing
**Trigger:** When verifying code correctness  
**Command:** `/test`

1. Identify or create test files with the pattern `*.test.*`.
2. Run tests using the project's test runner (framework not specified; check project scripts or documentation).
3. Ensure all tests pass before merging changes.

## Testing Patterns

- Test files follow the `*.test.*` naming convention (e.g., `gameLogic.test.ts`).
- The testing framework is not specified; check the repository or package scripts for details.
- Tests should cover core logic and edge cases.
- Example test file structure:
  ```typescript
  // userProfile.test.ts
  import { getUserProfile } from './userProfile';

  describe('getUserProfile', () => {
    it('returns user data for valid ID', () => {
      // test implementation
    });
  });
  ```

## Commands
| Command      | Purpose                                      |
|--------------|----------------------------------------------|
| /contribute  | Steps for contributing code                  |
| /test        | Steps for running and verifying tests        |
```
