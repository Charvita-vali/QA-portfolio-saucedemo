# SauceDemo E-Commerce QA — Jira Project Tracking

**Project Key:** SDQA
**Project Type:** Software (Scrum)
**Companion to:** [QA-portfolio-saucedemo](https://github.com/Charvita-vali/QA-portfolio-saucedemo)

Live project: epics, user stories, and prioritized bug tickets tracked and worked through a real Jira Scrum board, with an active sprint.

## Epics

| Key | Epic |
|---|---|
| SDQA-1 | Login |
| SDQA-2 | Cart |
| SDQA-3 | Checkout |

## Backlog (User Stories)

| Key | Epic Link | Summary |
|---|---|---|
| SDQA-4 | Login | As a user, I can log in with valid credentials |
| SDQA-5 | Login | As a user, I see a clear error on invalid login |
| SDQA-6 | Cart | As a user, I can add multiple items to my cart |
| SDQA-9 | Cart | As a user, my cart persists across pages |
| SDQA-7 | Checkout | As a user, I can complete checkout with valid shipping info |
| SDQA-8 | Checkout | As a user, I receive an order confirmation after checkout |

## Bug Tickets

| Key | Summary | Priority | Epic Link |
|---|---|---|---|
| SDQA-10 | Product image fails to render on Product Details page | Medium | Cart |
| SDQA-11 | Checkout Finish button unresponsive | Highest (release blocker) | Checkout |
| SDQA-12 | Cart badge doesn't update after item removal | Low | Cart |
| SDQA-13 | Missing error on repeated invalid login | Medium | Login |

Each bug ticket includes full steps to reproduce, expected vs. actual result, and is linked to its parent epic.

## Sprint — Checkout Hardening

Sprint scope: SDQA-7, SDQA-8, SDQA-11 — validating and stabilizing the checkout flow. SDQA-11, the release-blocking bug, was moved to **In Progress** as active work.

---

*Built as a companion to the [SauceDemo manual testing project](https://github.com/Charvita-vali/QA-portfolio-saucedemo) to demonstrate hands-on Jira defect-tracking and sprint management.*
