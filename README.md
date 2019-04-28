# Postman Multiple Workflows
A workaround to have multiple simple workflows in a postman collection

## Usage
```
newman run <collection.json> --global-var "workflow=<json list of request names>"
newman run Postman_Multiple_Workflows_Sample.postman_collection.json --global-var "workflow=[\"Create Employee\",\"Update Employee\"]"
```

