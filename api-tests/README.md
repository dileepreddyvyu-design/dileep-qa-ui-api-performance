# API Tests (Postman)

Import the collection and environment into Postman and click **Run**.

CLI:
```bash
newman run Ecommerce.postman_collection.json -e Ecommerce.postman_environment.json -r html
```
The HTML report will be saved in the current folder.
