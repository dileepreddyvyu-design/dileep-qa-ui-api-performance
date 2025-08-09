# QA Portfolio Project – UI, API, and Performance Testing

This project demonstrates a full QA lifecycle for a demo e-commerce application, covering:

- **Manual Testing** – Test cases, RTM, defect log
- **UI Automation** – Selenium WebDriver (Java + TestNG)
- **API Testing** – Postman + Newman CLI
- **Performance Testing** – Apache JMeter
- **Database Validation** – SQL queries for backend checks

---

## 🛠 Tools & Technologies
- **Manual Testing:** Excel, Jira/GitHub Issues
- **UI Automation:** Selenium WebDriver, Java, TestNG, Maven, WebDriverManager
- **API Testing:** Postman, Newman CLI
- **Performance Testing:** Apache JMeter
- **Database:** MySQL / Oracle SQL
- **Version Control:** Git, GitHub
- **Methodologies:** Agile/Scrum, STLC

---

## 📂 Project Structure
/docs
TestPlan.md
TestCases.xlsx
TraceabilityMatrix.xlsx
DefectLog.xlsx
/ui-automation
pom.xml
testng.xml
src/test/java/... (automation scripts)
/api-tests
Ecommerce.postman_collection.json
Ecommerce.postman_environment.json
/performance
api_load_test.jmx
/reports
manual-test-report.md
automation-report.md
performance-summary.md

---

## 📋 Manual Testing Deliverables
- **Test Plan:** Scope, objectives, risks, entry/exit criteria
- **Test Cases:** 40+ manual cases for functional, regression, smoke, and negative testing
- **Traceability Matrix:** Mapping requirements to test cases
- **Defect Log:** Realistic bug reports with severity, steps, and screenshots

---

## UI Automation
- Automated critical flows for login, sorting, cart, and checkout
- Cross-browser support (Chrome, Edge)
- Assertions for validation of UI elements and text

**Run automation:**
```bash
cd ui-automation
mvn clean test
mvn clean test-Dbrowser=edge
```

API Testing
Tested CRUD operations on https://reqres.in
Validated status codes, response bodies, and performance
Generated HTML reports with Newman
**Run API tests:**
```bash
newman run api-tests/Ecommerce.postman_collection.json\
    -e api-tests/Ecommerce.postman_environment.json-r html
```

Performance Testing
JMeter test with 25 virtual users and 30-second ramp-up
Collected throughput, 90th/95th percentile, and error rates

| Test Type   | Location                       |
| ----------- | ------------------------------ |
| Manual      | reports/manual-test-report.md  |
| Automation  | reports/automation-report.md   |
| API         | reports/api-newman-report.html |
| Performance | reports/performance-summary.md |

Author
Dileep Reddy Vuyyuru
📧 vuyyurudileepreddy@gmail.com
🔗 LinkedIn(https://www.linkedin.com/in/dileepreddyvuyyuru/)
