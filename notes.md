# Notes

## PC Localisation - Problématique

Trois utilisateurs :
- Le **gestionnaire de la flotte** : Close the Gap. Il reçoit des PC puis les redistribue à des gestionnaires locaux.
- Le **gestionnaire local** : il s'agit du partenaire qui reçoit les ordinateurs, les gère sur place, renseigne pour quelle utilisation les PC vont être occupés.
- L'**utilisateur final** : la personne qui va utiliser l'ordinateur.

### Le gestionnaire de la flotte

## Notes

- Les PC offerts ont en moyenne 2-5 ans de durée de vie après au reconditionnement (recyclés a posteriori localement),
- Les utilisateurs (personnes ou organisations) doivent avoir confiance dans les PC utilisés, notre système de localisation/monitoring est une garantie de qualité.
- Le gestionnaire local ne DEMANDE pas un remplacement (il signale/communique qu'un pc du réseau est out), Close The Gap est informé et procéde au remplacement logistique. 
- Les gestionnaires locaux & Close The Gap devraient avoir un système de suivi : en plus d'un avantage logistique sur l'état/statut (! fonctionne/ne fonctionne pas) du PC, ils veulent savoir où ils vont et à quel but, quels projets (!) ils auront servi.
- Il faut mettre en place un système de monitoring géolocalisé du statut de PC et son utilisation (projet + infos users de base)

## Fonctionnalités

### Schéma Shipping (changement localisation physique)
Même système que pour DHL, TNT,... Doit pouvoir fonctionner pour un ET plusieurs laptops.
#### ENVOI
1. set **origine** et destination
2. scan du QR Code
3. envoi physique
#### RECEPTION
1. réception physique
2. set **destination**
3. scan du QR code pour confirmer les réception
4. Le(s) machine(s) sont automatiquement ajoutée(s) au listing des machines présentes sur le site du gestionnaire local.

### Schéma Attribution de laptops (un ou plusieurs)
- vérifier le statut
- changer le statut.

#### Pour changer le statut pour Close the Gap
1. Définir le pays
2. Définir la région
3. Définir la ville
4. Définir le partenaire

#### POur changer le statut pour gestionnaire local
1. Définir la localité/projet
2. Définir si pour un ou plusieurs utilisateurs
- Si un utilisateur => L'utilisateur final, en scannant le QR code, pourra se créer un compte sur la plateforme pour renseigner l'état de son ordinateur depuis son smartphone.
- Si plusieurs utilisateurs, cela signifie que c'est pour un usage occasionnel et non personnel. Pas de compte d'utilisateur à créer mais le gestionnaire local peut attribuer un tag pour savoir pour quelles raisons l'ordinateur va être utiliser.


## Interfaces

### INTERFACE Close The Gap : 
- Localisation au scan du QR Code,
- statut d'ordinateur 
    - Localisation
        - pays, 
        - région, 
        - ville, 
        - nom du partenaire
    - (premier encodage), 
    - utilisation (y/n), 
    - état 
        - OK
        - cassé à réparer
            - hardware, 
            - software, 
            - panne non identifée 
        - cassé à recycler
    - disparu/volé
- traçage
    - numéro de série de la machine
    - ID Close The Gap
    - QR CODE
- toutes les infos qui suivent seront dispos pour Close The Gap

=> tout cela crée un historique et donc un rapport sur la vie du PC

### INTERFACE Gestionnaire local :
Au scan du QR code :
- Localisation
    - pays, 
    - région, 
    - ville, 
    - tag pour projet/classe
- statut d'ordinateur, 
    - En stock
        - yes
        - no
    - état
        - OK
        - cassé à réparer 
            - hardware 
            - software 
            - panne non identifiée
        - cassé à recycler 
        - disparu/volé, 
- type activité (éducation/choix multiples)
- type d'utilisateur : 
    - unique (si unique, alors possibilité pour l'utilisateur d'avoir un profil user dans l'application)
    - multiple
- fréquence 
    - full time
    - occasionnel

### INTERFACE Utilisateur Final (si type user unique) : 
- nom, 
- prénom, 
- sexe, 
- tag/keyword. Pour renseigner le nom de la classe ou du projet auquel la machine va servir.
- tranche age,
- activité (choix multiples), 