# Quick Start Guide

## Start The application in Development Mode

- Clone the Application `git clone <this-repo-address>`
- Install the dependencies `npm install`
- Start the application `npm start`

## Start The application in Production Mode

- Install the dependencies `npm install`
- Create the build `npm run build`
- Start the application `npm run start:production`
- Before starting make sure to creat prod environment `.env.prod` file

## Project Structure

| Name                              | Description |
| --------------------------------- | ----------- |
| **src/**                          | Source files |
| **src/abstractions**              | Abstarct classes and Interfaces  |
| **src/components**                | REST API Components & Controllers  |
| **src/environments**              | Application Environments Handling utility  |
| **src/lib**                       | Reusable utilities and library source code like a logger|
| **src/middleware/**               | Express Middlewares like error handler feature |
| **build/**                        | Compiled source files |
| **tests/**                        | Test cases |
| **tests/helpers/**                | Helpers for test cases |
| **tests/unit-tests/**             | Unit Test cases |
| **tests/integration-tests/**      | API routes (Integration) Test cases |

## Encryption

Set the `APPLY_ENCRYPTION` environment variable to `true` to enable encryption.

## Global Environment Object

You can directly access the environment attributes in any component/file using global environment object. For more details check this file: `src/global.ts`.

*Example*

To access the `applyEncryption` attribute from `Environment` class to Response Handler, write `environment.applyEncryption`;

## Default System Health Status API

- `${host}/api/status/system` - Return the system information in response
- `${host}/api/status/time` - Return the current time in response
- `${host}/api/status/usage` - Return the process and system memory usage in response
- `${host}/api/status/process` -  Return the process details in response
- `${host}/api/status/error` - Return the error generated object in response

