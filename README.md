# enhance-existing-features

A Codex skill for safely extending brownfield codebases.

## What this skill does

This skill guides an agent to:

1. Explore the existing codebase and map dependencies before editing.
2. Verify current behavior against authoritative, up-to-date documentation.
3. Implement minimal, focused feature changes by reusing existing patterns.
4. Add or update tests that match the change scope.

## Skill files

- `SKILL.md`: Core workflow and operating rules.
- `agents/openai.yaml`: Agent interface metadata and default prompt.
- `references/unit-tests.md`: Unit testing guidance.
- `references/property-based-tests.md`: Property-based testing guidance.
- `references/integration-tests.md`: Integration testing guidance.
- `references/e2e-tests.md`: End-to-end testing guidance.

## Workflow summary

1. Map entry points, data flow, dependencies, and integration boundaries.
2. Confirm APIs/framework behavior with official documentation.
3. Implement only the required change in existing conventions.
4. Select and update the right test level (unit/property/integration/e2e).

## Usage

Use this skill when working on existing projects where safety, compatibility,
and test coverage are critical.

Example prompt:

```text
Use $enhance-existing-features to add the new behavior, verify docs, and update tests.
```

## License

This repository currently does not define a license.
