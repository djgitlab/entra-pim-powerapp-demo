# Entra ID PIM Roles Power Apps Demo

This repository contains a **sanitized demonstration** of a Power Apps solution that interacts with **Microsoft Entra ID Privileged Identity Management (PIM)** roles using **Microsoft Graph**.

The purpose is to showcase real-world patterns for building a secure, maintainable app that supports **viewing eligible roles** and **requesting role activation** with governance in mind.

No client data, credentials, or tenant-specific identifiers are included.

---

## What This Demo Shows

- Power Apps interacting with Microsoft Graph
- PIM role eligibility and activation workflows
- Delegated permission patterns
- Defensive error handling and user-friendly messaging
- Separation between UI, logic, and API concerns
- Documentation suited for architecture and security review

---

## Core Capabilities

- View eligible and active PIM roles
- Request role activation with justification and duration
- Display activation status and expiration
- Support approval-based flows (where configured by policy)
- Surface API failures clearly without exposing sensitive details

---

## Architecture Overview

High-level flow:

1. User interacts with the Power App
2. App validates inputs and intent
3. Graph request is issued using delegated permissions
4. Response is parsed and surfaced in the UI
5. Errors and edge cases are handled explicitly

See:

- `docs/architecture.md`
- `docs/security-and-governance.md`

---

## Repository Structure

- `docs/`          Architecture, diagrams, and security notes
- `powerapp/`      App behavior, Power Fx examples, screenshots
- `graph/`         Graph endpoints, permissions, sample requests
- `deployment/`    Setup guidance and environment variable patterns
- `samples/`       Fully anonymized example data

---

## Notes on Security and Privacy

This repository is intentionally sanitized.

- No tenant IDs or environment IDs
- No internal domains or email addresses
- No secrets or connection tokens
- Sample data is fully anonymized

See `DISCLAIMER.md`.
