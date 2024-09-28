---
demo:
  title: "Démonstration\_02\_: surveiller une machine virtuelle Linux Azure"
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Démonstration 02 : surveiller une machine virtuelle Linux Azure

## Tâches des informations d’identification

+ Créez une machine virtuelle (modèle de démarrage rapide).
+ Configurez VM Insights.
+ Créez une alerte.  
+ Identifiez les problèmes de performances. 
+ Redimensionnez une machine virtuelle. 

## Besoins en ressources

+ Machine virtuelle Linux (créer à l’aide d’un modèle personnalisé)

## Diapositives de référence 

+ Modèles Microsoft Azure Resource Manager
+ Fonctionnalités clés d’Azure Monitor
+ Composants Azure Monitor
+ Métriques et journaux

  
## Étapes de référence

Les étapes détaillées sont fournies dans ces liens.

+ [Deploy a simple Ubuntu Linux VM](https://learn.microsoft.com/azure/virtual-machines/linux/quick-create-template)
+ [Activer VM Insights pour l’agent Azure Monitor](https://learn.microsoft.com/azure/azure-monitor/vm/vminsights-enable-portal#enable-vm-insights-for-azure-monitor-agent) 
+ [Tutoriel : Créer une alerte de métrique pour une ressource Azure](https://learn.microsoft.com/azure/azure-monitor/alerts/alerts-create-metric-alert-rule)


## Diapositives de référence (facultatif)

Utilisez ces diapositives pour un contexte supplémentaire.



## Éléments de discussion

1. Utilisez **Déployer un modèle personnalisé** pour une machine Ubuntu Linux simple. C’est ainsi que les étudiants créent la machine virtuelle dans l’exercice. Expliquez l’utilisation des modèles. 

1. Activez VM Insights. Passez en revue comment utiliser une règle de collecte de données et comment sélectionner un espace de travail Log Analytics. 

1. Créez une alerte basée sur les mesures. Par exemple, créez une règle d’alerte en fonction de l’utilisation du pourcentage d’UC.

1. Expliquez l’utilisation des groupes d’actions et la façon d’affecter un groupe d’actions à l’alerte. 

1. Passez en revue comment surveiller une alerte lorsqu’elle est déclenchée.

1. Concluez avec la façon d’exporter le modèle de ressource. 
