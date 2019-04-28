# Postman Multiple Workflows
A workaround to have multiple simple workflows in a postman collection

You need to pass in a global variable "workflow". The value should be a json list of the names of the requests to be called in order of execution desired.

## Usage

### Postman 
	1.	Set a global variable named workflow.
	2.	Run the collection

### Newman :
```
newman run <collection.json> --global-var "workflow=<json list of request names>"
newman run Postman_Multiple_Workflows_Sample.postman_collection.json --global-var "workflow=[\"Create Employee\",\"Update Employee\"]"
```



Note : Do not remove the initial dummy init request.
