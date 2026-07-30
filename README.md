# QA Testing Project — SauceDemo E-Commerce Application

A self-directed manual QA testing project built to practice real-world test design, exploratory testing, and professional bug reporting on [SauceDemo](https://www.saucedemo.com), a demo e-commerce site built for QA training.

## 🎯 Project Goals

- Practice writing structured, professional test cases (positive, negative, and boundary testing)
- Practice exploratory testing to uncover real defects
- Practice writing bug reports to industry standard (severity vs. priority, clear repro steps, evidence)
- Build a portfolio artifact demonstrating QA fundamentals for junior QA / SDET roles

## 🗂️ Repo Structure

```
qa-portfolio-saucedemo/
├── README.md
├── test-plan.md                          # Scope, environment, approach
├── test-cases/
│   ├── login-test-cases.md               # 7 test cases
│   └── cart-checkout-test-cases.md       # 18 test cases
├── bug-reports/
│   ├── BUG-001-dog-image.md              # Medium severity, High priority
│   └── BUG-002-checkout-blocker.md       # Critical severity, Critical priority
└── screenshots/
    └── (evidence for each bug report)
```

## 🐞 Summary of Findings

| Bug ID | Title | Severity | Priority |
|--------|-------|----------|----------|
| BUG-001 | Product images incorrect for `problem_user` | Medium | High |
| BUG-002 | Checkout blocked — Last Name field unresponsive for `problem_user` | Critical | Critical |

## 🧪 Test Coverage

- **Login module:** 7 test cases (valid/invalid login, empty fields, locked account, injection attempt, case sensitivity)
- **Cart module:** 8 test cases (add/remove items, persistence, navigation)
- **Checkout module:** 10 test cases (validation, cancel flow, order summary, XSS input handling)

## 🛠️ Application Under Test

- **URL:** https://www.saucedemo.com
- **Test users used:** `standard_user`, `problem_user`, `locked_out_user`, `performance_glitch_user`

## 📌 Next Steps

- Automate a subset of these test cases with Playwright (in progress — see `qa-automation-saucedemo` repo)
- Add API testing project
- Add CI/CD pipeline for automated regression runs

---
*This is a personal learning project, not affiliated with Sauce Labs. SauceDemo is a public demo application built for QA practice.*
