---
demo:
  title: "Démonstration\_01\_: configurer une machine virtuelle Azure Linux"
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Démonstration 01 : configurer une machine virtuelle Azure Linux

## Tâches des informations d’identification

Utilisez cette démonstration pour passer en revue ces tâches d’informations d’identification :
+ Créez une machine virtuelle Linux (portail).
+ Configurez une machine virtuelle Linux.
+ Connectez-vous à une machine virtuelle Linux avec SSH.  
+ Mettez à jour les systèmes d’exploitation des machines virtuelles Linux.
+ Installez et exécutez une dépendance de charge de travail.

## Besoins en ressources

Cette ressource peut être créée avant ou pendant la démonstration. 

+ Groupe de ressources. 

## Diapositives de référence (facultatif)

+ Plan pour des machines virtuelles
+ Distributions de Linux prises en charge
+ Tailles des machines virtuelles
+ Organisation des ressources Azure
+ Outils des administrateurs Azure

## Étapes de référence

Les étapes détaillées sont fournies dans ces liens.

+ [Provisionner une machine virtuelle Linux en utilisant le portail Azure](https://learn.microsoft.com/training/modules/provision-linux-virtual-machine-in-azure/2-provision-linux-virtual-machine-using-the-azure-portal)
+ [Démarrage rapide : créer une machine virtuelle Linux](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-portal?tabs=ubuntu)

## Éléments de discussion

**Création et configuration de la machine virtuelle**

1. Utilisez le portail pour créer une machine virtuelle Linux. Expliquez comment, dans les exercices ultérieurs, les modèles de CLI et de démarrage rapide seront utilisés pour créer des machines virtuelles. 

1. Utilisez le lien du portail pour passer en revue la sélection d’**images** Linux.  Identifiez la dernière distribution Ubuntu.

1. Utilisez le lien du portail pour passer en revue les sélections de **taille**.  Expliquez comment mettre à l’échelle les paramètres processeur et mémoire.

1. Expliquez les effets du redimensionnement. Le redimensionnement sera effectué dans un prochain labo. 

1. Expliquez les différentes façons de se connecter à une machine virtuelle Linux (clé publique SSH et mot de passe).
   
1. Expliquez l’importance des **règles de trafic entrant pour un port**. Plus précisément, le port 22 pour SSH et le port 80 pour Nginx. 

1. Utilisez l’onglet **Disques** pour montrer comment un disque de données serait ajouté. L’ajout d’un disque de données sera effectué dans un prochain exercice. 
 
1. Utilisez la page **Avancé** pour montrer où un fichier cloud-init peut être fourni.

1. En outre, les prochains exercices utilisent des modèles et l’interface CLI pour installer des machines virtuelles. 

**Accéder à la machine virtuelle et installer Nginx**

1. Déployez la machine virtuelle. Expliquez la phase de validation et la façon de surveiller les notifications.

1. Ouvrez une fenêtre CMD et accédez à la machine virtuelle avec SSH. Expliquez le format de la commande SSH et l’emplacement du fichier de clé. 

1. Installez Nginx et vérifiez que la page d’accueil s’affiche. 
