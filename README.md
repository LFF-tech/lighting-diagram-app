# Lighting Diagram App

The product application for creating and managing lighting diagrams for **Lighting for Film**.

This repository is separate from the public website so the diagram editor can have its own architecture, release cycle, testing strategy, and product roadmap.

## Repository purpose

- Build the interactive lighting diagram editor
- Manage diagram-specific UI, data models, and export workflows
- Support reusable lighting assets and project files
- Keep product code independent from the marketing website

## Initial structure

```text
docs/                         Product architecture and technical decisions
public/                       Static assets
src/components/               Shared interface components
src/features/diagram-editor/  Diagram editor feature code
src/lib/                      Shared utilities and integrations
src/types/                    Shared data and domain types
tests/                        Automated tests
```

The application framework, canvas/rendering engine, data layer, and hosting platform have not been chosen yet. The starter layout leaves those decisions open.

## Working agreement

- `main` is the stable branch.
- Create a short-lived branch for each feature or fix.
- Use pull requests to review meaningful changes before merging.
- Never commit passwords, API keys, or local `.env` files.
- Record durable technical decisions in `docs/`.

## Next steps

1. Define the minimum viable diagram workflow.
2. Choose the application framework and rendering approach.
3. Specify the diagram data model and file format.
4. Build a small editor prototype.
5. Add local development, testing, and deployment commands.
