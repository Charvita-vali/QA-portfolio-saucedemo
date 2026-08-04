# QA Testing Project — SauceDemo E-Commerce Application

A self-directed manual QA testing project built to practice real-world test design, exploratory testing, and professional bug reporting on [SauceDemo](https://www.saucedemo.com), a demo e-commerce site built for QA training.

## 🎯 Project Goals

- Practice writing structured, professional test cases (positive, negative, and boundary testing)
- Practice exploratory testing to uncover real defects
- Practice writing bug reports to industry standard (severity vs. priority, clear repro steps, evidence)
- Build a portfolio artifact demonstrating QA fundamentals for junior QA / SDET roles

## 🗂️ Repo Structure
## 🗂️ Repository Structure

```text
qa-portfolio-saucedemo/
├── README.md
├── requirements/
│   └── requirements.md
├── RTM.md
├── test-plan.md
├── test-summary-report.md
├── test-cases/
│   ├── login-test-cases.md
│   └── cart-checkout-test-cases.md
├── bug-reports/
│   ├── BUG-001-dog-image.md
│   └── BUG-002-checkout-blocker.md
└── screenshots/
```

## 🐞 Summary of Findings

| Bug ID | Title | Severity | Priority |
|--------|-------|----------|----------|
| BUG-001 | Incorrect product images displayed for problem_user | Medium | High |
| BUG-002 | Checkout blocked because Last Name field does not accept input for problem_user | Critical | Critical |

## 🧪 Test Coverage

- **Login Module (7 Test Cases)**
  - Positive & Negative Login
  - Empty Field Validation
  - Locked User Validation
  - SQL Injection Awareness Test
  - Username Case Sensitivity

- **Cart Module (8 Test Cases)**
  - Add to Cart
  - Remove from Cart
  - Cart Persistence
  - Continue Shopping
  - Empty Cart Validation
  - Navigation Testing

- **Checkout Module (10 Test Cases)**
  - Positive Checkout Flow
  - Mandatory Field Validation
  - Cancel Checkout
  - Order Summary Verification
  - Order Completion
  - Cart Reset After Purchase
  - XSS Security Awareness Test

## 🛠️ Application Under Test

- **URL:** https://www.saucedemo.com
- **Test users used:** `standard_user`, `problem_user`, `locked_out_user`, `performance_glitch_user`

## 💡 Skills Demonstrated

- Requirement Analysis
- Test Planning
- Test Case Design
- Manual Test Execution
- Exploratory Testing
- Functional Testing
- Positive & Negative Testing
- Validation Testing
- Basic Security Testing (SQL Injection & XSS Awareness)
- Bug Reporting
- Severity & Priority Assessment
- Requirement Traceability Matrix (RTM)
- Git & GitHub Documentation

## 🏆 Key Achievements

- Created a structured Test Plan defining project scope, testing approach, and environment.
- Designed 25 manual test cases covering Login, Cart, and Checkout modules.
- Executed all planned test cases and recorded execution results.
- Performed exploratory testing using the `problem_user` account and identified two reproducible defects.
- Created professional bug reports including severity, priority, reproduction steps, and screenshots.
- Developed a Requirement Traceability Matrix (RTM) to map functional requirements to test cases.
- Published all project artifacts in a well-structured GitHub repository.

## 📊 Project Metrics

| Metric | Value |
|---------|-------|
| Modules Tested | 3 |
| Test Cases Designed | 25 |
| Test Cases Executed | 25 |
| Test Cases Passed | 25/25 (100%)
| Exploratory Bugs Found | 2 |
| Bug Reports Created | 2 |
| Requirements Covered | 100% |
| Test Environment | Chrome (Desktop) |

## 🔗 Related QA Portfolio Projects

- **Manual Testing – SauceDemo** (Current Repository)
- **REST API Testing – JSONPlaceholder (Python + Pytest + Requests)**
- **SQL Database Testing** *(Coming Soon)*

---
> **Note:** This repository is a personal QA portfolio project created for learning and demonstrating manual testing skills. SauceDemo is a publicly available demo application provided by Sauce Labs for testing practice. This project is not affiliated with or endorsed by Sauce Labs.
