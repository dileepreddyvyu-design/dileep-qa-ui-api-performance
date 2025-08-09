# Test Plan – E‑Commerce Demo (Swag Labs + ReqRes)

## 1. Objective
Validate core user journeys and APIs for a demo e‑commerce flow: login, browse inventory, add to cart, checkout; and CRUD API requests.

## 2. In Scope
- UI: https://www.saucedemo.com/
- Browsers: Chrome, Edge (local)
- API: https://reqres.in/ (users endpoints)
- Testing types: Smoke, Functional, Regression (subset), API tests, Perf smoke

## 3. Out of Scope
- Payments, emails, real orders
- Mobile app, localization

## 4. Test Approach
- **Manual**: 40+ cases with RTM and screenshots
- **Automation**: Selenium (Java + TestNG) for happy paths and common negatives
- **API**: Postman tests + Newman CLI report
- **Performance**: JMeter smoke (25 VUs, 30s ramp)
- **Defects**: Logged in Jira or GitHub Issues; exported to docs/DefectLog.xlsx

## 5. Environments
- UI: https://www.saucedemo.com/ (demo)
- API: https://reqres.in/
- Data: Demo creds (e.g., standard_user / secret_sauce)

## 6. Entry/Exit Criteria
**Entry:** Environment reachable, test data ready.  
**Exit:** Critical bugs closed or triaged, smoke & happy paths pass, reports published.

## 7. Risks & Mitigations
- Demo sites may change → keep tests small and resilient.
- Local browser updates may break runs → pin WebDriver versions via WebDriverManager.

## 8. Deliverables
- TestCases.xlsx, TraceabilityMatrix.xlsx, DefectLog.xlsx
- Automation scripts + TestNG report
- Newman HTML report
- JMeter summary
