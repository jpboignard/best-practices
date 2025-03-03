---
title :  Mettre les caches entièrement en RAM (opcode et kvs)
GreenIT : 85
Weight : 92
activity : Production
tiers : Datacenter
responsable : Administrateur systèmes
priority: 2
difficulty: 2
impact: 3
ressources:
- Processeur
- Stockage
gr491Recommandation : "BACK-END 2. Utiliser les composants techniques qui améliorent les aspects NR, sécurité et performance"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=2-7031-backend-la-reduction-des-volumes-dechanges-des-operations
gr491Search : https://gr491.isit-europe.org/search.php?search=cache&go=Rechercher&famille=&inc=
tag : [ Cache, BACK-END ]
---

## Mettre les caches entièrement en RAM (opcode et kvs)

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  85    | 90  | 92  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Datacenter | Administrateur systèmes |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 2 | 2 | 3 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
| Processeur / Stockage   |

### Description

Les systèmes de cache doivent être, autant que possible, montés entièrement en mémoire vive (RAM). Cette mesure permet d’éviter des entrées/sorties sur les disques durs, ainsi que des cycles CPU pour les gérer.

L’objectif est double : servir rapidement une réponse au client, et limiter le nombre de composants matériels (et logiciels) impliqués dans la réponse retournée par le serveur.

La mémoire vive étant très rapide en termes d’accès en lecture/écriture, la durée de consommation des ressources est particulièrement courte. En outre, la durée de vie des composants est allongée avec cette bonne pratique, puisqu’il n’y pas de mouvement mécanique comme lors d’un recours au disque dur.

### Exemple

Exemples d’intégration d’un cache RAM à Drupal :
 - intégration de Memcache : https://drupal.org/project/memcache
 - intégration de Varnish : https://drupal.org/project/varnish

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de caches non mis en RAM  | 0  |
