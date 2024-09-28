---
demo:
  title: "Démonstration\_04\_: sauvegarder des machines virtuelles Linux Azure"
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Démonstration 04 : sauvegarder des machines virtuelles Linux Azure

## Tâche des informations d’identification

+ Configurer la sauvegarde Azure 

## Besoins en ressources

+ Machine virtuelle Linux

## Étapes de référence

Les étapes détaillées sont fournies dans ce lien.

+ [Démarrage rapide : sauvegarder des machines virtuelles dans le portail](https://learn.microsoft.com/azure/backup/quick-backup-vm-portal)
+ [Démarrage rapide : créer et déployer des modèles ARM à l’aide du portail Azure](https://learn.microsoft.com/azure/azure-resource-manager/templates/quickstart-create-templates-use-the-portal)

## Diapositives de référence

Utilisez ces diapositives pour un contexte supplémentaire.  

+ Qu’est-ce qu’Azure Backup ?
+ Options de protection des machines virtuelles

## Éléments de discussion

1. Passez en revue l’importation d’un modèle. Il s’agit de la quatrième façon dont ils ont créé une machine virtuelle dans la classe.
   
1. Expliquez la nécessité d’un coffre Recovery Services. Ce coffre doit se trouver dans la même région que la source de données. 

1. Passez en revue la façon dont la sauvegarde de machine virtuelle est accessible et activée dans le portail. 

1. Expliquez la différence entre les stratégies de sauvegarde standard et améliorée. 

1. Utilisez la liste déroulante de **types de sources de données** pour passer en revue les ressources que le Centre de sauvegarde peut protéger.

1. Indiquez la stratégie de sauvegarde par défaut et qu’une stratégie de sauvegarde personnalisée peut être créée.

1. Expliquez comment une stratégie de sauvegarde unique peut être utilisée sur de nombreuses machines virtuelles différentes.

1. Passez en revue les paramètres de configuration de la stratégie de sauvegarde (planification et rétention).

1. Passez en revue comment surveiller des travaux de sauvegarde.

1. Passez en revue la façon dont vous pouvez restaurer des machines virtuelles (et non sur les informations d’identification). 
