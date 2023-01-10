---
title :  Utiliser un cache HTTP
GreenIT : 72
Weight : 99
activity : Production
tiers : Réseau
responsable : Administrateur systèmes
priority: 4
difficulty: 3
impact: 5
ressources:
- Processeur
- Mémoire vive
gr491Recommandation : "BACK-END 2. Utiliser les composants techniques qui améliorent les aspects NR, sécurité et performance"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=2-7031-backend-la-reduction-des-volumes-dechanges-des-operations
gr491Search : https://gr491.isit-europe.org/search.php?search=cache&go=Rechercher&famille=&inc=
tag : [ Cache, BACK-END ]
---

## Utiliser un cache HTTP

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  72    | 103  | 99  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Réseau | Administrateur systèmes |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 4 | 3 | 5 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Mémoire vive  |

### Description

Les reverse proxies (Varnish, Squid ou Nginx) sont optimisés pour servir du contenu (pages HTML, images, etc.) de façon rapide, tout en consommant le moins de cycles CPU possible. En évitant de solliciter inutilement le serveur d’applications, ils permettent d’utiliser une infrastructure plus réduite.

### Exemple

Le recours à un reverse proxy spécialisé comme Varnish réduit drastiquement le temps nécessaire pour servir les pages dynamiques, tout en augmentant la capacité du CMS (Drupal, ici)
à en délivrer un grand nombre en même temps. On constate également qu’un cache généraliste comme APC n’est pas adapté (source : Asymptotix).

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
|  d'entêtes sans cache HTTP identifié | 0  |
