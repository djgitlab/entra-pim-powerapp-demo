# Architecture

## Components

- **Power Apps (Canvas)**: UI and business logic
- **Microsoft Graph**: Source of truth for PIM role data and activation workflows
- **Connector strategy**: Custom connector or Entra ID protected HTTP action, depending on environment constraints
- **Configuration**: Environment variables and connection references to avoid hardcoding tenant-specific values

## Data Flow (Conceptual)

User action in app
→ validate inputs
→ call Graph endpoint
→ parse response
→ update UI and state
→ handle errors explicitly

## Diagram

Add a simple diagram here once screenshots are ready:

- Put images in `docs/diagrams/`
- Reference them from this doc
