---
name: simplicity
description: Enforce DRY and KISS principles
patterns:
  - "**/*.ts"
  - "**/*.tsx"
  - "**/*.js"
  - "**/*.jsx"
  - "**/*.py"
  - "**/*.go"
  - "**/*.rs"
  - "**/*.java"
  - "**/*.rb"
  - "**/*.php"
agent: general
severity: medium
---

Flag DRY and KISS violations.

## Flag
- **DRY**: identical logic in 2+ places (>5 lines), copy-paste with minor changes
- **KISS**: Factory/Builder/Registry with single implementation
- **KISS**: wrapper that only delegates
- **KISS**: file >300 lines mixing responsibilities
- **KISS**: vague names (`Manager`, `Handler`, `Utils`, `Helper`)

## Ignore
- Complexity from external API/library
- Abstraction with 2+ implementations
- Test duplication
