# DPIA - Traitement HealthMed

## 1. Contexte du traitement

- **Responsable de traitement** : X-Corp
- **Finalités** : Suivi des parcours médicaux pour les patients des établissements de santé clients. Prise de rendez-vous en ligne.
- **Données traitées** : 
    - Données d'identification : nom, prénom, date de naissance, numéro de sécurité sociale 
    - Données de santé : pathologie, historique des soins, comptes-rendus d'examens, ordonnances
- **Personnes concernées** : Patients des établissements de santé clients
- **Volume de données** : Élevé (ensemble des patients des établissements clients)
- **Durée de conservation** : 10 ans après la fin du traitement médical
- **Mesures existantes** : Pseudonymisation, chiffrement, authentification forte, contrôle d'accès, PRA/PCA

Ce traitement remplit plusieurs critères rendant la DPIA obligatoire selon la CNIL :

- Données sensibles (données de santé)
- Volume important de personnes concernées
- Données concernant des personnes vulnérables (patients)

## 2. Mesures de protection

| Mesure                       | Détail                                                                                                               | Évaluation                                                                      |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Pseudonymisation des données | Les données directement identifiantes sont stockées séparément des données médicales et remplacées par un pseudonyme | Conforme, limite le risque d'identification directe en cas de fuite             |
| Chiffrement des données      | Algorithme AES-256, chiffrement au repos et en transit                                                               | Conforme, protège la confidentialité des données même en cas d'accès illégitime |
| Authentification forte       | Accès à la plateforme avec 2FA                                                                                       | Conforme, réduit le risque d'accès frauduleux                                   |
| Contrôle d'accès             | Système de gestion des habilitations basé sur les rôles (RBAC), accès aux seules données nécessaires                 | Conforme, limite les accès aux données au strict besoin                         |
| PRA/PCA                      | Plan de reprise/continuité d'activité, sauvegardes régulières sur site distant                                       | Conforme, assure la disponibilité et l'intégrité des données                    |

Les mesures en place semblent conformes au RGPD et couvrent les principaux risques. Néanmoins, une analyse plus poussée des scénarios de risque est nécessaire.

## 3. Appréciation des risques

| Scénario de risque                   | Source                                                                                                      | Mesures                                                        | Impacts potentiels                                                                                                                                | Vraisemblance | Gravité |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ------- |
| Accès illégitime aux données         | - Piratage du SI<br>- Divulgation par un employé<br>- Accès abusif par un prestataire                       | - Chiffrement<br>- Contrôle d'accès<br>- Traçabilité des accès | - Divulgation de données médicales<br>- Préjudice pour les patients (discrimination, atteinte à la réputation...)<br>- Sanctions CNIL pour X-Corp | 2             | 4       |
| Modification non désirée des données | - Erreur humaine<br>- Acte malveillant<br>- Bug logiciel                                                    | - Traçabilité<br>- Sauvegarde<br>- Contrôle d'intégrité        | - Erreur médicale<br>- Perte de confiance des patients<br>- Plaintes                                                                              | 2             | 3       |
| Indisponibilité du service           | - Attaque par déni de service<br>- Panne matérielle<br>- Crise majeure (pandémie, catastrophe naturelle...) | - Sauvegardes<br>- PRA/PCA<br>- Réplication multi-sites        | - Retard de prise en charge<br>- Désorganisation des soins<br>- Surcharge des personnels soignants                                                | 3             | 3       |

Légende :
- Vraisemblance : 1 (très improbable) à 4 (très probable)
- Gravité : 1 (négligeable) à 4 (maximale)

Malgré les mesures en place, des risques résiduels subsistent, notamment en termes de divulgation de données sensibles et de continuité du service. Des actions complémentaires doivent être envisagées.

## 4. Validation de la DPIA

Au vu des éléments ci-dessus, les risques résiduels semblent acceptables au regard des bénéfices du traitement pour le suivi des patients. Néanmoins, le plan d'action suivant est recommandé pour les réduire encore :

1. Mettre en place une anonymisation irréversible des données dépassant la durée de conservation légale
2. Renforcer la politique "Privacy by Design" en intégrant des exigences de protection des données dès la conception
3. Mettre en place une validation humaine avant toute modification critique des données
4. Réaliser des tests réguliers de non-régression et du PRA/PCA
5. Monitorer en continu les vulnérabilités des serveurs exposés

**Avis du DPO** : Avis favorable sous réserve de la mise en œuvre effective du plan d'action. Une nouvelle DPIA devra être réalisée en cas d'évolution substantielle du traitement.

**Décision du responsable de traitement** : Traitement validé. Le plan d'action devra être mis en œuvre dans les 6 mois. Les risques résiduels sont acceptés.