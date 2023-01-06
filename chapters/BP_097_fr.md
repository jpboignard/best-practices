---
title :  Utiliser un serveur asynchrone
GreenIT : 77
id : 97
category : Production
tiers : Datacenter
responsable : Administrateur systèmes
priority: 3
difficulty: 3
impact: 4
ressources:
- Processeur
- Mémoire vive
gr491Recommandation : "BACK-END 2. Utiliser les composants techniques qui améliorent les aspects NR, sécurité et performance"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=2-7023-backend-les-architectures-physiques-des-serveurs-disposent-de
tag : [ Conseil, BACK-END ]
---

## Utiliser un serveur asynchrone

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  77    | 94  | 97  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Datacenter | Administrateur systèmes |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 3 | 3 | 4 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Processeur / Mémoire vive  |

### Description

Les serveurs (web, d’applications, etc.) tels que Nginx, node.js ou Gwan sont conçus pour utiliser le minimum de ressources possible. Grâce à leur fonctionnement en mode asynchrone, ils ne sont pas tenus de créer un processus ou un thread pour chaque requête. Ils évitent ainsi de gaspiller leurs ressources.

Alors que la plupart des serveurs web augmentent leur consommation de mémoire vive au fur et à mesure des sollicitations, les serveurs asynchrones demeurent eux très stables.

### Exemple

Nginx a la réputation d’être plus performant qu’Apache. Il peut ainsi servir 2,1 fois plus de requêtes par seconde que ce serveur.

Pour aller plus loin :
 - https://nbonvin.wordpress.com/2011/03/14/apache-vs-nginx-vs-varnish-vs-gwan
 - https://nbonvin.wordpress.com/2011/03/24/serving-small-static-files-which-server-to-use


### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de serveurs applicatifs synchrones  | 1  |
