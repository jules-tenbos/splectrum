# PROJECT KEYWORD_REGISTRY

This file maintains project-specific workflow trigger keywords that extend the base WoW KEYWORD_REGISTRY.

## Project-Specific Workflow Keywords

| Keyword | File | Purpose | Trigger Context | Sesame Alias |
|---------|------|---------|-----------------|--------------|
| **OUTBOX** | `OUTBOX.md` | General outbox processing including external task distribution | Cross-repository task distribution, external task processing | `outbox sesame` |

## Future Project Keywords

Reserved for project-specific workflows when needed:

| Epic | Potential Keywords | Status |
|------|-------------------|--------|

## Sesame Alias Mapping

Project-specific sesame triggers:

```
outbox sesame → OUTBOX workflow (general outbox processing)
```

## Registry Inheritance

This project registry extends the base WoW registry located at `../wow/KEYWORD_REGISTRY.md`. All base workflow keywords are inherited and available in this project context.

## Usage Pattern

For project-specific workflows:
```markdown
**PROJECT_KEYWORD** → See [workflows/PROJECT_FILENAME.md](./workflows/PROJECT_FILENAME.md)
```

For inherited WoW workflows, refer to the base registry at `../wow/KEYWORD_REGISTRY.md`.