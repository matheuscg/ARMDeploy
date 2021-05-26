# Modulo 2 - Web App - Aplicativo Web

* Planos e suas vantagens;
    * https://azure.microsoft.com/en-us/pricing/details/app-service/windows/
* Plataformas:
    * Windows
    * Linux
    * Containers
* Auto Scale
    * Regra de scale up 
    * Regra de scale down
* Deployment slot (multiplas versões c/ balanceamento de carga)
    * canary test
    * Pode fazer um swap
    * Pode fazer por balanceamento por peso(weight)
* Monitoring - Alerts
    * Alerts my cpu, disk space
    * dashboards
* Monitoring - Diagnostics logs
    * Cant attach an external drive
        * Storage and its container (blob)
    * Rolling log system
    * all stack toogles log
* Monitoring - Log Stream
    * Need Local drive log (24h life)
    * "real time" log
* Command Line
    * Navegate trought webapp image storage
    * Hard Debug
* Advanced Tools (Kudu)
    * WebApp information
    * Debug Console (CMD/Powershell)
    * Process Explorer


## Powershell

'''
get-command *AzWebApp*


New-AzResourceGroup -Name az204-webapp-pwsh -Location 'Brazil South'

New-AzAppServicePlan -ResourceGroup az204-webapp-pwsh -Name az204-app-serv-plan -Location 'Brazil South' -Tier Free

New-AzWebApp -ResourceGroup az204-webapp-pwsh -Name az204-webapp -Location 'Brazil-South' -AppServicePlan az204-app-serv-plan
'''

## Az cli

'''
az group create --name <name> --location <location>

az appservice plan create -g <group-name> -n <name> 

az webapp create -g <group-name> -n <unique-name> -p <plan-name>
'''

Ou podemos usar essa magia 

'''
mkdir newwebapp
cd newwebapp
git clone https://github.com/Azure-Samples/html-docs-hello-world.git
cd html-docs-hello-world
az webapp up --location <location> --name <unique> --html
'''

Mais alguns exemplos magicos:

1. https://docs.microsoft.com/en-us/azure/app-service/deploy-local-git?tabs=cli

O magico: https://github.com/projectkudu/kudu/wiki

## Coding

* Visual Studio Webapp
    1. Criar um projeto do tipo webapp (talvez de qualquer tipo)
    1. publicar e siga o fluxo para plubicar um webapp na Azure
    1. selecione o seu webapp(aplicativo web)
        1. pode escolher outro deployment slot
* Visual Studio WebJob
    1. um projeto webjob
    1. publicar e siga o fluxo para plubicar um webjob na Azure
    1. selecione o seu webapp(aplicativo web)
