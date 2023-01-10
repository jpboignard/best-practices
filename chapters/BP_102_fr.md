---
title :  Mettre en cache les réponses Ajax
GreenIT : 91
Weight : 102
activity : Production
tiers : Utilisateur/Terminal
responsable : Architecte Logiciel/Développeur
priority: 3
difficulty: 2
impact: 4
ressources:
- Réseau
- Requêtes
gr491Recommandation : "FRONT-END  3. Utiliser les environnements et outils qui permettent de limiter les impacts"
gr491Critere : https://gr491.isit-europe.org/crit.php?id=3-5015-frontend-la-reduction-des-volumes-dechanges-des-operations
gr491Search : https://gr491.isit-europe.org/search.php?search=cache&go=Rechercher&famille=&inc=
tag : [ Cache, FRONT-END ]
---

## Mettre en cache les réponses Ajax

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|   91   | 107  | 102  |      |

### Catégories

| Cycle de vie |  Tiers  |  Responsable  |
|:---------:|:----:|:----:|
| 4. Production | Utilisateur/Terminal | Architecte Logiciel/Développeur |

### Indications

| Degré de priorité |      Mise en oeuvre       |  Impact écologique    |
|:-------------------:|:-------------------------:|:---------------------:|
| 3 | 2 | 4 |

|Ressources Economisées                                      |
|:----------------------------------------------------------:|
|  Réseau / Requêtes  |

### Description

Les réponses Ajax qui seront inchangées dans un futur proche ne doivent pas être redemandées au serveur. Par conséquent, les mettre en cache pour économiser de la bande passante.

### Exemple

Si une requête Ajax retourne une liste de noms de villes, de noms de contacts ou tout élément non calculé, il faut mettre ces réponses en cache du côté client pour ne pas générer à nouveau une requête vers le serveur.

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de réponses AJAX non mises en cache  | 10%  |
