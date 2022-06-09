# Spring Boot Microservice Take Home Project

### Description
Build a simple SpringBoot  micro-service using the provided template which includes the following required endpoints and api functionalities

```shell
# To start up the application:
./mvnw spring-boot:run
```

### Required Endpoint
Build a GET and PUT endpoint with the following spec:
* route - **/api/:version/resource/:resourceId**
* header param - **X-User-Id** - customizable string identifying a user
* PUT return payload JSON structure:
``` json
{
  "data": {
    "resourceId": 1,
    "resource": "RESOURCE"
  }
}
```
* version - only include 1 version, **v1**

### Required Functionality
1. Local file persistence for storing PUT request and retrieving GET request (can be temporary storage in the repo)
2. Built-in API versioning to facilitate endpoint changes (i.e. /api/v1/resource, /api/v2/resource, ...)
3. Unit testing of business logic for both endpoints.

### Bonus Functionality
1. Validating api request path, header and payload data

### Submission
Submit your project as a zip file with your name (e.g. **john_doe.zip**).  Include any necessary execution instructions in a file: **instructions.txt** (feel free to Dockerize the project using the given Dockerfile).  The project reviewer must be able to (without complications) verify the following:
1. The microservice runs locally using the given applicant instructions
2. The GET and PUT endpoints can be successfully accessed using the given **curl_client.sh** sample script
3. Unit tests can be successfully run using the given applicant instructions

Any comments, explanations or project feedback included in **instructions.txt** is appreciated
Have fun :)

### Notes
* All required npm packages are included in **package.json**: a fully satisfactory solution was built with these dependencies.  Feel free to add any additional dependencies, but try to understand and use the included dependencies if possible.
