# Challenge récupération de données EC2 2025

Lors de l'european cyber cub 2025, une nouvelle épreuve à été ajoutée. Il s'agit d'une épreuve de forensic de récupération de données créée par l'entreprise Databack, d'une durée de ~8h. 
Avec l'équipe de l'ESNA `ESNArcotrafiquants` nous sommes arrivés en tête de l'épreuve. 

**Vous trouverez notre rapport dans le dossier `rapport`.**

## Résumé du Scénario – Challenge Forensic « Kiki-Vendéen »

### Contexte
La PME du Kiki-Vendéen, spécialisée à l’origine dans la fabrication de verre régional, s’est diversifiée dans la vente en ligne. Elle a subi une attaque paralysant l’ensemble de ses services (production, logistique, commandes, paie), car tous dépendent d’une seule base de données.

### Situation actuelle

Le SI de l’entreprise est désorganisé : absence de cartographie, maintenance délaissée depuis 2 ans.
L’entreprise utilise la virtualisation et des backups, mais ne suit pas les bonnes pratiques 3-2-1+.
Une image disque (.dd) du serveur compromis a été collectée et vous est remise pour analyse.

### Objectif principal
Assurer la remédiation en récupérant les données critiques, tout en documentant toutes vos étapes dans un rapport forensic complet.
À partir de l’image disque fournie, vous devez retrouver et valider les éléments suivants :

    - Base de données Microsoft SQL Server (ou son backup)
    - Factures réparties dans 3 répertoires distincts
    - Répertoire de partage de documents (avec divers formats de fichiers)

### Validation des données
Vous devez prouver que les fichiers sont fonctionnels (contenu valide, ouvert sans erreur).
Enjeux Techniques

    - Le pirate est inexpérimenté (noob), laissant des traces, erreurs et plusieurs chemins possibles.
    - Certaines données peuvent avoir des extensions incorrectes.
    - La compétition couvre : reverse engineering, cryptographie, systèmes de fichiers et containers.

### Consignes de Compétition

Toute réponse doit être justifiée (textes, captures, outils utilisés…).
Un template de rapport PDF est fourni sur le disque.
Vous pouvez utiliser tous les outils que vous souhaitez.
Le rapport final doit être enregistré sur le disque fourni.

`Rappel : Certains fichiers seront utiles pour les épreuves suivantes (EC2), pensez à tout extraire du disque externe.`