---
title :  Limiter le nombre de domaine servant les ressources
GreenIT : 170
Weight : 18
category : Production
tiers : Réseau
responsable : Architecte Logiciel/Développeur
priority: 3
difficulty: 3
impact: 4
ressources:
- Requêtes
gr491Recommandation : "FRONT-END 6. S'assurer que l'utilisation du service permet le contrôle des impacts"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=6-5044-frontend-les-mecanismes-de-cache-et-la-mise
mesurer : Le nombre de domaines servant les ressources
tag : [ Recommandation, FRONT-END]
---

## Limiter le nombre de domaines servant les ressources

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|   170   | 55  | 18  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Réseau | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 3 | 3 | 4 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Requêtes  |

### Description

Lorsqu’un site web ou un service en ligne héberge les composants d’une page web sur plusieurs domaines, 
le navigateur doit établir une connexion HTTP avec chacun de ces domaines. Une fois la page HTML récupérée, 
le navigateur appelle les ressources au fur et à mesure qu’il parcourt le DOM (Document Object Model). 
Certaines ressources sont indispensables au fonctionnement de la page. Si elles sont hébergées sur un autre domaine peu réactif,
cela peut rallonger le délai d’attente avant que la page soit opérationnelle. Dans la mesure du possible, il faut donc regrouper toutes les ressources sur un seul domaine.

Seule exception à cette règle, le fait d’héberger les ressources statiques (feuilles de styles, images, etc.) sur un domaine séparé,
pour éviter d’avoir à transporter un ou plusieurs cookies à chaque GET HTTP du navigateur. On réduit le temps de réponse ainsi que la bande passante consommée inutilement.

### Exemple

Pour un site web institutionnel à fort trafic, on privilégiera deux sous-domaines :
 - le serveur applicatif sur www.domain.tld ;
 - le serveur media « cookie-less » sur media.domain.tld.

On limite ainsi le nombre de domaines tout en évitant de transporter inutilement un cookie à chaque GET HTTP sur une ressource statique

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| Le nombre de domaines servant les ressources   |  5 |
