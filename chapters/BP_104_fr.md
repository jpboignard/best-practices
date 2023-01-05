---
title :  Désactiver le DNS lookup d’Apache
GreenIT : 84 
id : 104
category : Production
tiers : Datacenter
responsable : Administrateur systèmes
priority: 2
difficulty: 2
impact: 3
ressources:
- Processeur
- Réseau
---

## Désactiver le DNS lookup d’Apache

### Identifiants

| GreenIT |  V2  |  V3  |  V4  |
|:-------:|:----:|:----:|:----:|
|  84    | 100  | 104  |      |

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
|  Processeur / Réseau  |

### Description

À chaque fois qu’un serveur web reçoit une requête HTTP, il enregistre cette information dans un log, en traduisant généralement l’adresse IP de l’internaute en nom de domaine. Cette conversion (DNS Lookup) constitue l’un des goulots d’étranglement du serveur HTTP Apache.

À désactiver donc.

### Exemple

Dans le fichier de configuration de votre serveur Apache, situé à l’adresse `/etc/apache/httpd.conf` ou à l’adresse `/etc/apache2/apache2.conf`, écrire :
```apacheconf
 HostnameLookups Off
```

### Principe de validation

| Le nombre ...     | est inférieur ou égal à   |  
|-------------------|:-------------------------:|
| de DNS lookup actif  |  0 |
