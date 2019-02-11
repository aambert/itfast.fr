**Getting Started AKS**
[https://docs.microsoft.com/fr-fr/cli/azure/install-azure-cli?view=azure-cli-latest](https://docs.microsoft.com/fr-fr/cli/azure/install-azure-cli?view=azure-cli-latest)

  *Etape 1- Installation du client en ligne de commande*
  
    az aks install-cli
    
*Etape 2 - Connexion sur le cluster Kubernetes via la ligne de commande ou ressource group correspond au nom du ressource group utilisé pour K8S et le nom du cluster AKS ici K8S*

    az login
    

> Saisir vos identifiants Azure dans la page web qui va s'ouvrir

![enter image description here](https://github.com/aambert/itfast.fr/blob/master/img/AzLogin.png?raw=true)
   

     az aks get-credentials --resource-group azure-k8s --name k8s

*Etape 3 - Montage d'un tunnel pour rapporter le port 8001 en local et accès en http à la console AKS*

    az aks browse --resource-group azure-k8s --name k8s

*Etape 4 - Lancer le navigateur internet*

    http://127.0.0.1:8001

Ensuite vous aurez accès à l'interface Web d'AKS

![enter image description here](https://raw.githubusercontent.com/aambert/itfast.fr/master/img/K8S-Dashboard.png)


Connexion en ligne de commande :
