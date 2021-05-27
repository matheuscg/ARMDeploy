# Modulo 4 Functions APP

* Unique Name
* 1 Million executions per month is free
* 400000 GB-s per month is free
* Stateless
* Type:
    * Docker
    * Code (Runtime, Version)
        * nodejs, donet framework, dotnet core, python, powershell and custom
* Linux or Windows
* Plan type
    * Serverless, pay by execution and CPU
    * App Service Plan
    * Premium
* https://docs.microsoft.com/en-us/azure/azure-functions/functions-triggers-bindings?tabs=csharp
* https://docs.microsoft.com/en-us/learn/modules/create-serverless-logic-with-azure-functions/3-create-an-azure-functions-app-in-the-azure-portal?pivots=javascript
* https://github.com/Azure-Samples/durablefunctions-apiscraping-dotnet

## Functions 

* All functions will be written on the choosed language of the function app
* Development environment 
    * On Portal (web only for windows)
    * VSCode
* Trigger
    * HTTP
    * Timer
    * Azure Queue Storage
    * Azure Service Bus Queue/Topic
* Access Control
    * Function
    * Anonymous
    * Admin
* Integration
    * Input
    * Outputs

## Console

Access to cmd terminal of functions app server

## Deployments Slots

Multiples Environments

## Deployment Center

Continuos Delivery

## Configuration

* Application Settings, environment variables
* Function Runtime (Version and Quota)
* General Settings (Language Version, Plataform Architeture)

## Identity

Standalone identity or System Identity

## TLS/SSL

Certificate Stuf

## Networking

Firewall, CDN e Access Restrictions

## Scale Out

Manage de scale out limit

## API Management

Put the functions behind a gateway

## CORS

Enable/Disable CORS

## Durable Functions

* For long processes, greater than 30 minutes
* Stateful
* Suspend while waiting
* Types:
    * Client HTTP (Entry Point)
    * Orchestrator (Call other functions)
    * Activity (Perform an action)
* Uses:
    * Function Chaining Pattern
    * Fan out / Fan in
    * Asynchronous API Pattern
    * Monitor Pattern
    * Human Interaction Pattern

### Coding 

1. Create dumb package.json name and version
1. Install durable functions '''npm install durable-functions'''

## App Service Editor

Web editor for functions

## Command Line Azure Functions Core Tools

'''
mkdir testFunc
cd testFunc
func init
func new
func start &> /dev/null & # Local test
curl 'http://localhost:7071/api/testFunc'
pkill func
func azure functionapp publish "testFunc"
'''

## Costum Handler

For enable non suported languages do functions app.

1. Create a host.json to determine where de function are