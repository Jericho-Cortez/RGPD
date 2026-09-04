# Gestion d'une violation de données - HealthMed

## 1. Description du scénario

- Service impacté : HealthMed 
- Date et heure de détection de l'incident : 12/05/2023 à 10h15
- Origine de l'incident : erreur humaine dans la configuration d'un serveur
- Détail des faits : Un technicien a mal configuré les droits d'accès à un serveur hébergeant des données HealthMed lors d'une opération de maintenance. Des comptes-rendus médicaux avec des données sensibles (pathologies, traitements, historique médical…) se sont retrouvés exposés sur Internet sans authentification pendant 6 heures, de 4h du matin à 10h. L'erreur a été détectée suite à une alerte sur un forum spécialisé.

## 2. Qualification de la violation

- Type de violation : Confidentialité 
- Catégories de données impactées :
    - Données d'identification : nom, prénom, date de naissance, numéro de sécurité sociale
    - Données de santé : pathologies, traitements, historique médical, comptes-rendus d'examens
- Nombre de personnes concernées : 5000 patients
- Conséquences potentielles : 
    - Divulgation de données médicales très sensibles
    - Risque de discrimination ou de chantage envers les patients
    - Atteinte à la réputation de X-Corp
    - Possibles sanctions de la CNIL

## 3. Évaluation des risques

Au vu de la sensibilité des données et du nombre de personnes impactées, cette violation présente vraisemblablement un risque élevé pour les droits et libertés des personnes physiques :
- Risque de discrimination si des données sur des pathologies stigmatisantes (VIH, troubles psychiatriques...) sont divulguées
- Risque de préjudice moral et psychologique lié à l'exposition de données très intimes 
- Risque d'usurpation d'identité ou de fraude avec les données d'identification
- Risque de chantage ou d'intimidation si des données compromettantes sont révélées

## 4. Notification et communication

La violation doit être notifiée à la CNIL dans les 72 heures, car :
- Elle est susceptible d'engendrer un risque élevé pour les droits et libertés des personnes
- Elle concerne des catégories particulières de données (données de santé)

Une communication doit également être adressée individuellement aux personnes concernées dans les meilleurs délais, pour leur permettre de prendre des mesures pour se protéger des conséquences (vigilance sur leurs comptes, support psychologique...).

## 5. Mesures correctrices

Actions immédiates :
- Fermeture de l'accès web au serveur concerné
- Changement des mots de passe des comptes techniques  
- Vérification des journaux pour identifier les données exposées
- Information de la direction et du DPO

Actions correctives : 
- Revue de la politique de gestion des accès
- Sensibilisation et formation des équipes techniques
- Mise en place d'une procédure de validation des changements
- Audit de sécurité des systèmes hébergeant des données sensibles

Actions préventives :
- Réalisation d'un exercice de gestion de crise cyber
- Mise à jour de l'analyse de risques et de la DPIA HealthMed

## 6. Documentation interne

La violation est consignée dans le registre interne des violations de X-Corp, avec l'ensemble des éléments collectés :
- Circonstances et nature de la violation 
- Catégories de données et nombre de personnes impactées
- Conséquences potentielles de la violation
- Mesures prises pour remédier à la violation et atténuer ses éventuelles conséquences négatives
- Preuve de la notification à la CNIL
- Preuve de la communication aux personnes concernées