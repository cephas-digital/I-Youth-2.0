# I-Youth 2.0 PDMALS interface prototype

A responsive React and TypeScript user interface concept for the Project Data Measurement and Learning System (PDMALS) described in IITA RFP/Q VSM 10/2026.

## Run locally

```sh
npm install
npm run dev
```

Create a production build with `npm run build`.

## Prototype scope

This workspace is a front-end mockup. It uses representative sample data and local interactions for role switching, navigation, filters, record search, CSV export, notifications, forms, and action dialogs. It does not connect to a production database, identity provider, messaging gateway, GIS service, or offline synchronization API.

The earlier-version project was not present in the supplied `I-Youth 2.0` workspace when implementation began, so this interface was built from the attached RFP.

See [requirements coverage](docs/requirements-coverage.md) for the mapping from RFP requirements and dashboard personas to this interface.

## Workspace routes

Each primary workspace has a direct URL. The app supports browser back and forward navigation and normalizes `/` to `/overview`.

- `/overview`
- `/participants`
- `/field-operations`
- `/learning-cohorts`
- `/case-management`
- `/enterprise-jobs`
- `/grants-services`
- `/assessments`
- `/merl-indicators`
- `/reports`
- `/gis-coverage`
- `/communications`
- `/documents`
- `/administration`
