# Performance Smoke Test (JMeter)

## Goal
Quickly check API responsiveness and error rate for `GET /api/users?page=2` on https://reqres.in.

## Steps
1. Open **Apache JMeter**.
2. File → Open → `api_load_test.jmx` (included here), or create it manually:
   - Thread Group: Users=25, Ramp-Up=30s, Loop=1
   - HTTP Request Defaults: `https://reqres.in`
   - HTTP Request: GET `/api/users?page=2`
   - Listener: Summary Report
3. Click **Start** (green play). Export the results to `reports/jmeter-summary.csv`.

## What to Capture
- Throughput
- 90th/95th percentile
- Error %

Record your findings in `reports/performance-summary.md`.
