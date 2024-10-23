# learningpostman
Repos from learning postman

# What is 
This repos was created for bootcamp of Testing API Rest.

# Tecnologies used
- Postman  web version
- node version v20.18.0
- newman 6.2.1
- newman-reporter-html
  
# Documentation
- API: [Consulte Swagger](https://serverest.dev/#/)

# How to install environment
- First: Install node on your computador [baixe aqui](https://nodejs.org/en/download)
- Second : Install newman as global [baixe aqui a dependencia](https://www.npmjs.com/package/newman)
```
npm install -g newman
```
- Third : Install depencies of report (opcional) [newman-reporter-html
](https://www.npmjs.com/package/newman-reporter-html)
```
npm install -g newman-reporter-html
```
## How to run test
### By Postman web or desktop
- Import collection and environment
- Execute test manually or automated
### By newman
- Open console 
- Execute command line to execute tests
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
```
- Execute test with report 
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
```
### Report
If you chose to run the tests with the htmlextra report, you generated an HTML file with the test results and to check the validations

