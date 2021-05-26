# ARMDeploy
The old ARM deployment files Microsoft used to provide

# Modulo 1

```
Connect-AzAccount

Select-AzSubscription -SubscriptionID $subscriptionId

Get-AzVM

New-AzResourceGroup -Name az204-azpw -Location 'Brazil South'

New-AzVM -ResourceGroupName az204-azpw -name az204-vm -Location 'Brazil South' -VirtualNetworkName az204-vm-net -SubnetName default -SecurityGroupName az204-sg -PublicIpAddressName az204-pub-ip -OpenPorts 80,3389

```

```
az group create --name az204-cli --location eastus

az vm create --resource-group az204-cli --name az204-vm --image win2016datacenter --admin-username az204admin

```

