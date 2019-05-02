# BananesExport

BananesExport est une entreprise d'exportation de bananes qui aimerait avoir une solution pour gérer son catalogue de commandes.
Une commande de bananes comprend les éléments suivants :

Un destinataire (nom, adresse, code postal, ville, pays)
Une date de livraison
Une quantité de bananes (en kg)
Un prix

Afin de gérer les commandes, BananesExport a besoin des services suivant :

Consulter la liste des destinataires
Consulter la liste des commandes d’un destinataire
Enregistrer un destinataire
Enregistrer une commande

Pour la création d’une commande ou d’un destinataire, tous les champs sont obligatoires. De plus, la création d’une commande est soumise aux règles suivantes :

La date de livraison doit être, au minimum, une semaine dans le futur par rapport à la date du jour.
La quantité de bananes demandée doit être comprise entre 0 et 10 000 et doit être un multiple de 25 (parce qu’une caisse de bananes contient 25kg)
Le prix sera déterminé automatiquement par le système à partir de d’un prix au kilo de 2.50€

Pour la création d’un destinataire, il ne doit pas être possible d’en créer deux parfaitement identiques.

Contraintes techniques

Les services doivent être exposés en REST (en GET pour les opérations de consultation et en POST pour les opérations d’enregistrement)
Le développement doit être réalisé en Java ou en Kotlin et compatible avec un jdk 1.11
Pour la partie stockage des données, le choix est laissé libre (pas besoin de persistance, un stockage en mémoire est suffisant) 

