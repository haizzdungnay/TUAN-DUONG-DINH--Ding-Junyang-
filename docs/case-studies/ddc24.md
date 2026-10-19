# DDC24 — Industrial Edge Application & DevOps

[← Back to portfolio](../../README.md) · [Source repository](https://github.com/haizzdungnay/DDC24)

**Focus:** Frontend, backend application logic and DevOps for a Linux-based BMS edge controller  
**Project stack:** React, TypeScript, Go, CMake, systemd, Linux

## My role and boundaries

During my Mekong Technologies employment, my confirmed responsibilities on DDC24 were:

- Developing the **frontend**.
- Implementing **backend application logic**.
- Handling **DevOps**, including development/deployment workflows.

I did **not** own hardware development, device specifications or hardware design. The public repository describes a larger system, and that wider scope must not be mistaken for work I personally authored.

## Engineering context

The repository describes an industrial edge runtime with web/API components, Linux services, packaging and deployment support, plus interfaces to industrial I/O. My area of work centered on software/application functionality and operating that software in a reproducible engineering workflow.

## Public evidence

| What to examine | Direct evidence |
| --- | --- |
| System overview | [Project README](https://github.com/haizzdungnay/DDC24/blob/main/README.md) |
| Web/backend modules | [Applications](https://github.com/haizzdungnay/DDC24/tree/main/apps) |
| Development and operations | [Development & Operations](https://github.com/haizzdungnay/DDC24/blob/main/docs/06_operations/DEVELOPMENT_AND_OPERATIONS.md) |
| Build, release and tests | [Verification script](https://github.com/haizzdungnay/DDC24/blob/main/scripts/verify-project.sh) |
| Workflow definitions | [Build/test workflow](https://github.com/haizzdungnay/DDC24/blob/main/.github/workflows/build-and-test.yml) · [Security workflow](https://github.com/haizzdungnay/DDC24/blob/main/.github/workflows/security.yml) |

## Validation and limitations

The repository includes **workflow definitions** for build/test and security scanning. During this review, no corresponding GitHub Actions runs were returned, so the existence of YAML files must not be presented as proven passing CI.

The public technical material is the only basis used here. Device-specific optimizations, proprietary runtime details and enterprise-only configuration are **not** reproduced in this case study. Running on compatible hardware and runtime/field validation are distinct from host-only build validation.

## Interview discussion topics

Maintaining frontend/backend contracts; service lifecycle and failure recovery on Linux; repeatable packaging; CI vs real-device validation; and boundaries between application code and hardware specifications.

---

*Responsibilities above reflect the project owner's confirmed account; linked artifacts establish public technical context, not sole authorship of the entire device.*