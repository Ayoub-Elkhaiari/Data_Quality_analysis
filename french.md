# Qualité des Données

La **qualité des données** signifie que les données sont fiables, précises, et sans erreurs. Une bonne qualité des données est importante car elle aide dans de nombreux domaines comme les opérations, la gestion client, le marketing, l’analyse, et la prise de décision. En revanche, une **mauvaise qualité des données** peut faire perdre du temps, causer de mauvaises décisions, et créer de la frustration.

## Problèmes Courants de Qualité des Données

1. **Incomplétude** : Certaines données manquent, comme des informations clients incomplètes, ce qui peut compliquer les services et réduire la satisfaction.
2. **Inexactitude** : Les données avec des fautes de frappe, des valeurs inutiles ou erronées rendent difficile la confiance dans les informations. Par exemple, un mauvais numéro de série pour une pièce peut fausser le suivi de l’inventaire.
3. **Incohérence** : Les données incohérentes, comme des montants dans différentes devises sans conversion, compliquent les analyses.
4. **Invalidité** : Des données incorrectes et illogiques, comme un nombre négatif pour des unités de produit (ex. : -10 pour un stock), peuvent causer des erreurs.
5. **Redondance** : Les doublons dans les données peuvent fausser l’analyse et consommer plus d’espace.
6. **Format non standard** : Des différences dans les nombres décimaux, comme "13,99" vs "14,777709", peuvent créer des erreurs de calcul et de rapport.

## Importance de l'Assurance Qualité des Données

L’**assurance qualité des données (AQD)** regroupe des processus pour garantir que les données restent précises, cohérentes, et utiles.

### Principales Activités de l'Assurance Qualité des Données

1. **Profilage des Données** : Explorer et analyser les données pour trouver des problèmes. Par exemple, on vérifie combien de lignes sont vides, en double, ou hors norme. Si 2% des lignes d’une table clients manquent, c’est acceptable ; mais si 20% manquent, c’est un gros problème.

2. **Indicateurs de Qualité des Données** : On peut mesurer la qualité des données avec des indicateurs pour savoir si elles sont fiables :
   - **% de Complétude** : Indique combien de données sont manquantes. Par exemple, si 98 % des dossiers de maintenance sont remplis, les données sont plus fiables.
   - **% de Précision** : Mesure combien de données reflètent la réalité, comme des descriptions de pièces correctes.
   - **% de Conformité** : Vérifie si les données respectent des règles. Par exemple, chaque incident qualité doit être lié à un ordre de maintenance.

### Outils et Méthodes pour le Profilage des Données

On peut utiliser des requêtes SQL pour explorer les données et repérer des valeurs manquantes, des doublons ou vérifier les formats. Par exemple :
   - **Exemple de requête SQL** : `SELECT COUNT(*) FROM Clients WHERE Email IS NULL;` – pour trouver les adresses e-mail manquantes.
   - **SQL Server Data Quality Services (DQS)** : Cet outil aide à automatiser le profilage sans avoir besoin de code SQL personnalisé.

Pour de plus grands ensembles de données, des outils comme la bibliothèque **pandas de Python** permettent de voir facilement les données manquantes ou incorrectes, de visualiser les données et de les corriger.

### Maintenir une Bonne Qualité des Données

La gestion de la qualité des données est un processus continu. C’est particulièrement vrai dans des environnements comme le **système de gestion de la qualité d’Airbus**. Lorsque de nouvelles données sont ajoutées ou mises à jour, il est important de les vérifier régulièrement pour éviter les problèmes. Un profilage et une validation constants aident à garantir que les décideurs peuvent faire confiance aux données qu'ils utilisent.

Dans l’**industrie aéronautique**, une bonne qualité des données permet d'éviter des erreurs dans des domaines comme le suivi des pièces ou la planification de la maintenance, ce qui pourrait sinon entraîner des retards, des coûts supplémentaires, ou des risques de sécurité.

### Exemple : Travail sur la Qualité des Données chez Airbus

En tant qu’analyste de qualité des données chez Airbus, vous vous concentrerez sur l’amélioration de la fiabilité des données dans le département **Quality for Airframe Services (QBSR)**. En assurant l’exactitude des rapports de non-conformité et des mesures de performance, vous aiderez le département à prendre de meilleures décisions.

Par exemple, si les données de maintenance ont des formats de date incohérents, il serait utile de les standardiser et de mettre en place des vérifications régulières pour permettre aux équipes d’Airbus d’analyser avec confiance les tendances de maintenance pour anticiper et prévenir les problèmes.

### Résumé

Dans ce rôle, vos principales tâches seraient :
- **Profilage des Données** : Utiliser des outils comme SQL ou DQS pour explorer et vérifier la qualité des données.
- **Mise en Place d'Indicateurs de Qualité** : Mesurer la complétude, l’exactitude et la conformité des données pour s’assurer qu'elles répondent aux normes d’Airbus.
- **Vérifications Régulières** : Maintenir la qualité des données pour qu'elles restent fiables dans des environnements en évolution rapide comme l’aéronautique.
- **Communication** : Travailler avec les utilisateurs pour comprendre leurs besoins et les aider à prendre des décisions basées sur des données de bonne qualité.
