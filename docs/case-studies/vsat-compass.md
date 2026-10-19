# V-SAT Compass — Android & Backend Engineering

[← Back to portfolio](../../README.md) · [Source repository](https://github.com/haizzdungnay/VSAT_COMPASS)

**Focus:** Native mobile and REST API integration, student assessment workflows  
**Stack:** Android (Java), Spring Boot (Java), PostgreSQL, JWT, Gradle

## Problem and scope

Provide a practice and mock-exam experience across an Android client and a server-backed application. The public project documents student authentication, exam delivery, sessions, results/history and administrative content workflows.

## Engineering contributions

I handled the application implementation and integration work described in the public project:

- Android user flows for login, exam selection, timed sessions and result review.
- Spring Boot API-backed workflows and PostgreSQL persistence.
- Authentication/session integration between mobile application and backend.
- Documentation and repeatable validation procedures for client and server changes.

The system has multiple moving parts: a database, a REST service and an Android client. Keeping the API contract and user/session state consistent is a central engineering challenge.

## Public evidence

| What to examine | Direct evidence |
| --- | --- |
| Android app | [App source](https://github.com/haizzdungnay/VSAT_COMPASS/tree/main/app) |
| Backend services | [Spring Boot module](https://github.com/haizzdungnay/VSAT_COMPASS/tree/main/VSAT/vsat-compass-api) |
| Architecture and documentation | [Project README](https://github.com/haizzdungnay/VSAT_COMPASS/blob/main/README.md) · [Design notes](https://github.com/haizzdungnay/VSAT_COMPASS/blob/main/docs/DESIGN.md) |
| Testing and release | [Smoke checklist](https://github.com/haizzdungnay/VSAT_COMPASS/blob/main/docs/SMOKE_CHECKLIST.md) · [Deployment runbook](https://github.com/haizzdungnay/VSAT_COMPASS/blob/main/docs/DEPLOY_RUNBOOK.md) |

## Validation and limitations

The repository contains manual smoke-test documentation and instructions for Android/backend testing. During the portfolio review, a dedicated repository-owned `.github/workflows` CI pipeline was **not confirmed**. Do not treat the documentation, a static badge or Copilot code-review activity as evidence of a passing end-to-end CI pipeline.

Any production availability, current health and individual milestone claims should be rechecked against the deployed service and up-to-date repository state.

## Interview discussion topics

Client/server contracts; session consistency and exam submission; secure authentication; failure handling; migration/versioning; and how to automate Android plus backend smoke checks.

---

*Scope and evidence are taken from the public repository; no unverified benchmark or adoption claim is included.*