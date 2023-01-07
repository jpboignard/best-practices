---
title :  Réduire au nécessaire les logs des serveurs
GreenIT : 82
Weight : 103
activity : Production
tiers : Datacenter
responsable : Architecte Logiciel/Développeur
priority: 2
difficulty: 2
impact: 3
ressources:
- Processeur
- Mémoire vive
- Stockage
gr491Recommandation : "BACK-END 2. Utiliser les composants techniques qui améliorent les aspects NR, sécurité et performance"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=2-7037-backend-la-mise-en-oeuvre-de-services-est
gr491Search: https://gr491.isit-europe.org/search.php?search=logs&go=Rechercher&famille=&inc=
tag : [ Conseil, BACK-END ]
---
https://gr491.isit-europe.org/search.php?search=cache&go=Rechercher&famille=&inc=

## Réduire au nécessaire les logs des serveurs

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|   82   | 99  | 103  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Datacenter | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 2 | 2 | 3 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Mémoire vive / Stockage  |

### Description

Les logs des serveurs (web, applicatif, base de données) pouvant devenir très volumineux, il est recommandé de les configurer dans leur ensemble.
En réglant au plus juste le niveau log de l’application (exemple: uniquement information/warning/error) et en ne traçant que les informations pertinentes,
on évite des écritures sur le disque qui peuvent être massives, ce qui limite la consommation de cycles CPU et réduit l’espace de stockage nécessaire.

Pour éviter de saturer des disques, il est également recommandé de mettre en place une durée de rétention et une rotation des logs en fonction du besoin lors de l’exploitation du service.

### Exemple

Les logs d’accès d’un serveur Apache peuvent être configurés comme suit pour exclure les ressources statiques et flux RSS :

```apacheconf
SetEnvIf Request_URI "\.(ico|pdf|ﬂv|jpg|jpeg|png|gif| js|css|gz|swf|txt)$" dontlog
SetEnvIf Request_URI "^/rss/" dontlog
CustomLog /var/log/apache/access.log combined env=!dontlog
```

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
|de logs sans durée maximale de rétention   | 0  |
