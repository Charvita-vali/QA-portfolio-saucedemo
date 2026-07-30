# Test Cases — Login Module

**Application:** SauceDemo
**Module:** Login / Authentication
**URL:** https://www.saucedemo.com
**Executed by:** Charvita Vali
**Execution date:** July 2026

| ID | Title | Preconditions | Steps | Expected Result | Priority | Status |
|----|-------|---------------|-------|------------------|----------|--------|
| TC_LOGIN_01 | Valid login | None | 1. Enter `standard_user` / `secret_sauce`<br>2. Click Login | User lands on Products page | High | Pass |
| TC_LOGIN_02 | Invalid password | None | 1. Enter `standard_user` / wrong password<br>2. Click Login | Error message shown, user stays on login page | High | Pass |
| TC_LOGIN_03 | Empty username | None | 1. Leave username blank, enter password<br>2. Click Login | Error: "Username is required" | Medium | Pass |
| TC_LOGIN_04 | Empty password | None | 1. Enter username, leave password blank<br>2. Click Login | Error: "Password is required" | Medium | Pass |
| TC_LOGIN_05 | Locked out user | None | 1. Enter `locked_out_user` / `secret_sauce`<br>2. Click Login | Error: "Sorry, this user has been locked out." | High | Pass |
| TC_LOGIN_06 | SQL injection attempt | None | 1. Enter `' OR '1'='1` in username field<br>2. Click Login | Login fails gracefully, no crash or bypass | Medium | Pass |
| TC_LOGIN_07 | Case sensitivity | None | 1. Enter `STANDARD_USER` (uppercase) / `secret_sauce`<br>2. Click Login | Login fails — usernames are case-sensitive | Low | Pass |

## Execution Summary
- **Total test cases:** 7
- **Passed:** 7
- **Failed:** 0
- No defects found in the login module.

## Notes
- TC_LOGIN_06 is a light security-awareness test — not a full penetration test, but shows QA thinking around input handling
