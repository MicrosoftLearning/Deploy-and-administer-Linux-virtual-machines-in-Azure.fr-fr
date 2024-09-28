---
demo:
  title: "Démonstration\_03\_: accéder au stockage pour une machine virtuelle Linux Azure"
  module: 'Guided Project: Deploy and administer Linux virtual machines'
---

# Démonstration 03 : accéder au stockage pour une machine virtuelle Linux Azure

## Tâches des informations d’identification

+ Créez une machine virtuelle (CLI).
+ Ajoutez les disques de données de la machine virtuelle et configurez des partitions. 
+ Montez un partage de fichiers SMB Azure sur une machine virtuelle Linux.
+ Attribuez une identité managée sur une machine virtuelle Linux. 
+ Attribuez des rôles Azure. 
+ Transférez des données vers et depuis une machine virtuelle Linux à l’aide d’AzCopy. 

## Besoins en ressources

Ces ressources peuvent être créées avant ou pendant la démonstration. 
+ Resource group
+ Machine virtuelle Linux.
+ Comptes de stockage avec partage de fichiers et conteneur d’objets blob.
+ Fichiers chargés à utiliser pour les tests.
+ Identité managée. 

## Étapes de référence

Les étapes détaillées sont fournies dans ces liens.

+ [Démarrage rapide : créer une machine virtuelle Linux avec Azure CLI sur Azure](https://learn.microsoft.com/en-us/azure/virtual-machines/linux/quick-create-cli)
+ [Attacher un disque de données à une machine virtuelle Linux](https://learn.microsoft.com/azure/virtual-machines/linux/attach-disk-portal)
+ [Créer un partage de fichiers SMB](https://learn.microsoft.com/azure/storage/files/storage-how-to-create-file-share?tabs=azure-portal)
+ [Bien démarrer avec AzCopy](https://learn.microsoft.com/azure/storage/common/storage-use-azcopy-v10)


## Diapositives de référence

Utilisez ces diapositives pour un contexte supplémentaire. 
+ Comptes de stockage
+ Conteneurs d’objets blob et fichiers
+ Fichiers contre objets blob
+ Identités managées
+ Contrôle d’accès basé sur les rôles

## Éléments de discussion

**Créer une machine virtuelle à l’aide de l’interface CLI** - Référence #1

>Vous pouvez utiliser une machine virtuelle existante au lieu d’en créer une.

1. Accéder à Cloud Shell.

1. Créez la machine virtuelle avec l’interface CLI. Indiquez qu’il s’agit de la troisième façon montrée aux étudiants pour créer des machines virtuelles.
   
**Ajouter un disque de données à une machine virtuelle Linux** - Référence #2

1. Passez en revue comment utiliser le portail pour ajouter un disque de données à une machine virtuelle. Les étudiants utiliseront l’interface CLI dans l’exercice.

1. Connectez-vous à la machine virtuelle et utilisez cette option `lsblk` pour répertorier les disques. Notez la taille du disque et que le disque n’est pas monté.

1. Préparez le disque avec `parted` et `partprobe`. Utilisez le code dans le lien de référence.

1. Montez le disque et utilisez `df` pour répertorier le point de montage. 

**Accéder à un partage de fichiers SMB à partir de la machine virtuelle** - Référence #3 et instructions du labo d’étudiant

1. Recherchez le compte de stockage et expliquez les partages de fichiers.

1. Attribuez une identité managée à une machine virtuelle. L’identité doit avoir accès au compte de stockage.

1. Copiez le script du portail pour accéder au partage de fichiers à partir d’une machine virtuelle Linux.

1. Connectez-vous à la machine virtuelle et créez un fichier avec le script. Vous pouvez utiliser l’éditeur vi.

1. Exécutez le script et montez le partage de fichiers. 

**Utiliser AzCopy pour copier un fichier d’objets blob dans le lecteur de données** - Référence #4 et instructions du labo d’étudiant

1. Ajoutez le rôle Contributeur au stockage de données Blob à la machine virtuelle. Passez en revue les autres rôles d’objets blob. 

1. Connectez-vous à la machine virtuelle et installez AzCopy. Passez en revue d’autres outils qui peuvent être utilisés pour transférer des fichiers. 

1. Utilisez AzCopy pour transférer un fichier du stockage d’objets blob vers le lecteur de données. Vous pouvez également transférer un fichier vers le stockage d’objets blob.  
