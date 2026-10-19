# OtakuShop — Full-Stack Commerce Engineering

[← Back to portfolio](../../README.md) · [Source repository](https://github.com/haizzdungnay/WebSiteOtakuShopVer2) · [Live demo (availability may vary)](https://web-site-otaku-shop-ver2.vercel.app)

**Focus:** Full-stack web development, application security and delivery  
**Stack:** Next.js, React, TypeScript, Prisma, PostgreSQL, Docker

## Problem and scope

Build an e-commerce application with customer shopping flows and administrative workflows rather than a disconnected UI prototype. The public repository documents product discovery, cart, checkout, customer accounts, admin functions, and VNPAY sandbox integration.

## Engineering contributions

In this team-organized project, I handled the application implementation and integration work described in the repository, including:

- Web pages and application logic for browsing products, cart, checkout and account operations.
- Authentication and access-control flows protecting customer and admin functionality.
- Database-backed application services using Prisma and PostgreSQL.
- Docker configuration and deployment/build workflow integration.

These are **application features and engineering responsibilities**, not claims that payments were processed in production or that a security audit certified the product.

## Public evidence

| What to examine | Direct evidence |
| --- | --- |
| Product interface | [Homepage screenshot](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/blob/main/public/demo/homepage.png) · [Products screenshot](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/blob/main/public/demo/products.png) |
| Application structure | [App routes](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/tree/main/app) · [Prisma schema](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/tree/main/prisma) |
| CI and Docker | [CI workflow](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/blob/main/.github/workflows/ci.yml) · [Dockerfile](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/blob/main/Dockerfile) · [Workflow runs](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/actions) |
| Developer documentation | [Repository README](https://github.com/haizzdungnay/WebSiteOtakuShopVer2/blob/main/README.md) |

## Validation and limitations

The public CI workflow includes TypeScript checking, application build and Docker build stages. **Do not read a green workflow badge as proof of complete security or integration testing**: security-audit steps currently use `continue-on-error`, the integration-test job contains a placeholder command, and the deployment jobs are placeholders. These are transparent improvement opportunities, not completed production gates.

The payment reference describes **VNPAY sandbox** integration. Demo availability and deployment status should be verified at review time. No unverified user count, revenue, latency, test coverage or production-scale claim is made here.

## Interview discussion topics

Authentication vs authorization boundaries; server-side validation; database transaction design for checkout; secret management; and how to turn non-blocking scans plus placeholder CI stages into meaningful release gates.

---

*This case study summarizes verifiable public repository material and my stated engineering role. It is not a claim of an independent security certification.*