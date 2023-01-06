---
title :  Désactiver les logs binaires
GreenIT : 93
Weight : 106
category : Support / Maintenance
tiers : Datacenter
responsable : Administrateur systèmes
priority: 2
difficulty: 2
impact: 2
ressources:
- Processeur
- Mémoire vive
- Stockage
gr491Recommandation : "BACK-END 2. Utiliser les composants techniques qui améliorent les aspects NR, sécurité et performance"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=2-7037-backend-la-mise-en-oeuvre-de-services-est
gr491Search : https://gr491.isit-europe.org/search.php?search=logs&go=Rechercher&famille=&inc=
tag : [ Conseil, BACK-END ]
---

## Désactiver les logs binaires

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
| 83     | 93  | 106  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 6. Support / maintenance | Datacenter | Administrateur systèmes |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 2 | 2 | 2 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Mémoire vive / Stockage  |

### Description

Les logs binaires du serveur MySQL ou MariaDB peuvent devenir très volumineux, consommant des cycles CPU tout en générant des entrées-sorties (I/O) sur le disque dur, puisque chaque requête de modification/suppression est inscrite dans le fichier de log. Aussi, si vous avez la possibilité de désactiver ces logs, vous économiserez beaucoup de ressources.
Avant de désactiver, il faut s'assurer qu'une réplication de la base de données n'est pas nécessaire et que la perte des données depuis le dernier backup est acceptable.

### Exemple

Pour MySQL, ajouter la configuration suivante :
```
skip-log-bin
```

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| d'options --skip-log-bin et --disable-log-bin non activées dans le cas où les logs binaires ne sont pas utiles  | 0  |
