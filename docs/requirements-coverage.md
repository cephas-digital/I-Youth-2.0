# RFP interface coverage

Source: *Request for Proposal/Quotation for the Design, Development, and Deployment of PDMALS for I-Youth 2.0*, IITA RFP/Q VSM 10/2026 (23 pages).

This prototype translates the software and dashboard requirements into screen concepts. The RFP's vendor instructions (proposal content, pricing, eligibility, submission address and deadline, evaluation, contract terms) are procurement directions to bidders, not requirements for the programme software, and are intentionally not represented as application features.

## Dashboard personas (Annex B)

The top-right **View as role** selector previews each persona. Navigation is scoped by persona, and the participant view is an individual self-service dashboard. Sensitive GESI and identity information is presented as role-restricted. The 12 requested views are represented by these personas:

| RFP dashboard | Prototype persona and view |
| --- | --- |
| Executive / Program Leadership | Program leadership · programme overview, KPI cards, trends, country snapshot, exceptions |
| MERL / Results | MERL specialist · indicator registry, targets, verification, data-quality queue |
| Country | Country coordinator · country results, cohorts, locations, field actions |
| Component / Intervention | Component manager · pathway milestones, services, cohort delivery |
| State / District / Field Coordination | Field supervisor · assignment, validation, sync and follow-up queues |
| Enumerator / Data Collection | Enumerator · personal caseload, returned records and offline queue |
| Participant Workspace | Participant · profile completeness, private journey, tasks, support, documents |
| Inclusion / GESI | Inclusion specialist · reach, participation and outcome indicators with protected attributes |
| Enterprise, Employment & Livelihood Outcomes | Outcomes officer · enterprise survival, jobs, verification and follow-up |
| GIS / Spatial | GIS analyst · programme locations, geocoding and coverage gaps |
| Data Quality & System Health | System administrator · access requests, integrations, availability and operational controls |
| Partner / Donor Read-only | Partner / donor · approved aggregate indicators and report/map access |

## Operational requirements (RFP sections 4–7 and Annex B)

| Requirement area | Interface coverage |
| --- | --- |
| Recruitment, intake, screening, deduplication, consent | Participants directory, status filters, registration action, consent field, duplicate review alerts |
| Participant identity, onboarding, longitudinal profile | Participant master-record table and participant journey preview |
| Enumerator workforce and offline capture | Field operations dashboard, workload/validation queues, sync-health indicators and offline guidance |
| Training and learning journey | Learning & cohorts workspace, attendance/completion metrics and learning milestones |
| Case management and progression | Case management workspace, at-risk cases, milestones, referrals and overdue actions |
| Enterprise, employment, livelihood outcomes | Enterprise & jobs workspace with activity, verification and follow-up indicators |
| Grants, assets, finance and market linkages | Grants & services workspace and reconciliation indicators |
| Surveys and assessments | Assessments workspace, schedules, completion and verification queues |
| Indicator and results framework | MERL & indicators registry and target/actual status |
| Role-based dashboards, filters, exports, scheduled reports | Persona switcher, country and period controls, Reports workspace, CSV action and report export action |
| GIS, geospatial privacy | GIS & coverage workspace, location coverage preview, sensitive-location notice |
| Communications and consent | Communications workspace, delivery/opt-out indicators and notification controls |
| Documents and evidence | Documents workspace with evidence status and linkage to programme records |
| RBAC, partners, configuration, audit logs | Role-scoped navigation, access-control notes, Administration workspace and audit-trail actions |
| API integrations and data exchange | Administration integrations status for KoBo, SMS and BI; monitoring and error states are represented visually |
| Legacy data migration | Administration workspace shows source record mapping, exception count and reconciliation status |
| Privacy, safeguarding, security and governance | Restricted-field messages, participant privacy notice, role-aware views, approved-data badges and export/audit cues |
| Hosting, availability, backup and continuity | Administration workspace includes availability, encrypted-backup and restore-check status; detailed incident response and recovery procedures remain implementation work |
| Accessibility, mobile and offline requirements | Responsive layout, keyboard focus treatment, reduced-motion support, mobile navigation, visible sync state |

## Visual direction and interaction

The page uses a calm agricultural green palette, warm off-white surfaces, compact data tables, clear status labels and a farm photograph. The live IITA homepage and the official DHIS2 analytics and KoBoToolbox collection documentation were reviewed for visual and workflow references. DM Sans and Manrope are used as close web-font choices; the public IITA page did not expose a verifiable institutional typeface in the reviewed sources, so these are not represented as exact IITA brand fonts.

Navigation, selectors, filters, dialogs, form validation, profile actions, quick actions, pagination, dashboard save, CSV generation and notifications are connected as client-side prototype interactions. They do not persist to a server.

## Known mockup limits

- All programme figures, people and timelines are sample data, not IITA records.
- Authentication, MFA, field-level permissions, server-side audit immutability, consent retention, data-subject requests and sensitive-cell suppression need implementation and UAT against the real access model.
- Offline encryption, queued synchronization and conflict resolution need a field data layer; this interface only shows sync state and pending work.
- APIs, SMS/email delivery, GIS boundaries and precise-location controls, BI connections, scheduled exports, backups, disaster recovery and data migration need service integration.
- Forms currently demonstrate interaction; each form type still needs its own RFP-aligned field schema and workflow.
