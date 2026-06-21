# Commit Message Template

## Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

## Types

| Type     | Description                              | Example                     |
|----------|------------------------------------------|-----------------------------|
| `feat`   | A new feature                            | feat(hero): add 3D logo tilt |
| `fix`    | A bug fix                                | fix(form): correct validation |
| `docs`   | Documentation only changes               | docs(readme): update deployment guide |
| `style`  | Changes that do not affect the meaning of the code (formatting, etc.) | style(css): improve spacing |
| `refactor` | A code change that neither fixes a bug nor adds a feature | refactor(logo): simplify animation logic |
| `perf`   | A code change that improves performance  | perf(images): optimize hero assets |
| `test`   | Adding missing tests or correcting existing tests | test(workflow): add link checker validation |
| `chore`  | Changes to the build process or auxiliary tools | chore(deps): update actions/checkout |

## Rules

- Use the **present tense** ("add feature" not "added feature")
- Use the **imperative mood** ("move cursor to..." not "moves cursor to...")
- Limit the **subject line to 72 characters**
- Separate **subject** from **body** with a blank line
- Use the body to explain **what** and **why** (not how)
- Reference issues and pull requests liberally

## Example

```
feat(hero): add staggered bar animation on load

- Implement CSS animation for ascending bars in logo
- Add entrance timing for professional feel
- Ensure animation only runs once on initial page load

Closes #42
```

## Quick Commit Examples

```bash
git commit -m "feat(dns): update records for Cloudflare Pages"
git commit -m "fix(accessibility): add proper form labels"
git commit -m "docs(brand): update clear space guidelines"
```