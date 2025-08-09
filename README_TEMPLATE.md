# QA Portfolio Project – UI + API + Performance

**What’s here**
- Manual tests + RTM + Defect log (docs/)
- Selenium + TestNG UI automation (ui-automation/)
- Postman collection + environment (api-tests/)
- JMeter performance smoke (performance/)
- Reports placeholders (reports/)

**How to use**
1) Upload these folders to your GitHub repo.  
2) Run UI tests: `cd ui-automation && mvn clean test`  
3) Run API tests: `newman run Ecommerce.postman_collection.json -e Ecommerce.postman_environment.json -r html`  
4) Open JMeter and run `performance/api_load_test.jmx`

Update screenshots and results into `reports/`.
