# playwright-cucumber-sample

## **Overview:**

This is a sample test automation framework developed using **Playwright** with **Cucumber**.

For Demo purpose web UI test cases are created on [ecommerce-playground.lambdatest.io](https://ecommerce-playground.lambdatest.io/index.php) site and API test cases are created on these [SOAP Calculator API](http://www.dneonline.com/calculator.asmx) & [REST Library Information System API](https://www.libraryinformationsystem.org/Services/RestService.svc) endpoints.

## Supported Browsers

1. Chrome - default browser
2. Firefox
3. MS Edge
4. WebKit - web browser engine used by Safari

#### Steps to use

##### 1. Installation

Playwright framework requires [Node.js](https://nodejs.org/) v14+ to run.

Installing the dependencies.

```sh
npm ci
```

##### 2. Execution

To run test scenarios use below command.

```sh
npm run test
```

To run specific scenario, use tags command. Below are few examples.

```sh
npm run test:tags @sanity
npm run test:tags "@calculator or @author"
npm run test:tags "@rest and @author"
```

To dry run test scenarios use below command.

```sh
npm run dry:test
```

To rerun the failed test scenarios use below command.

```sh
npm run failed:test
```

To change any environment configuration in .env file at run time use set command.
Eg: To change browser to Firefox use below command

```sh
set BROWSER=firefox
```

Similar command can be used to update other environment configuration

To generate HTML and Cucumber report use below command

```sh
npm run report
```

##### 4. Report & Logs

Cucumber HTML report will be present inside

```sh
test-results/reports/cucumber.html
```

HTML report will be present inside

```sh
test-results/reports/html/index.html
```

Execution log will be present in the log file.

```sh
test-results/logs/execution.log
```
