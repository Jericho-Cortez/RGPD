# Rapport de Synthèse RGPD - X-Corp

## Introduction

Le RGPD, entré en application en 2018, a profondément changé les règles en matière de protection des données personnelles. Il responsabilise les entreprises en leur imposant de nouvelles obligations, et renforce les droits des individus sur leurs données. **Son non-respect expose à des sanctions pouvant aller jusqu'à 4% du CA mondial**.

Les grands principes du RGPD sont : licéité, loyauté, transparence, limitation des finalités, minimisation des données, exactitude, limitation de la conservation, intégrité et confidentialité, et responsabilité. 

Ce rapport a pour but d'illustrer ces concepts clés avec des exemples concrets tirés du cas de l'entreprise X-Corp.

## Les acteurs du RGPD chez X-Corp

- **Responsable de Traitement (RT)** : X-Corp agit en tant que RT pour la plupart de ses traitements, car elle détermine les finalités et les moyens. *Exemple : pour son produit DataManage, X-Corp est RT car elle définit à quelles fins les données clients sont utilisées (prospection...) et par quels moyens (son logiciel).*

- **Sous-Traitants (ST)** : X-Corp fait appel à plusieurs ST, notamment pour l'hébergement et certaines prestations analytiques. *Exemple : AWS est un ST de X-Corp car il agit uniquement sur instruction de X-Corp pour stocker les données sur ses serveurs. Il n'en détermine pas l'usage.*

- **Délégué à la Protection des Données (DPO)** : X-Corp a nommé un DPO, obligatoire vu son activité de profilage à grande échelle. Le DPO veille à la conformité RGPD de l'entreprise. *Il a par exemple réalisé des DPIA sur chaque nouveau produit.*

## Les bases légales utilisées par X-Corp

Le RGPD impose que **chaque traitement repose sur une base légale valable**. X-Corp utilise principalement :

- Le **consentement** pour ses opérations marketing. *Ex : envoi de newsletters aux utilisateurs de EduLearn ayant explicitement accepté.*

- L'**exécution du contrat** pour les traitements nécessaires à la fourniture des services. *Ex : stockage des données médicales des patients pour assurer le bon fonctionnement d'HealthMed.*

- L'**intérêt légitime** pour certains traitements analytiques. *Ex : analyses d'usage d'EduLearn pour améliorer la plateforme.*

## Les données sensibles traitées par X-Corp

Le RGPD interdit de traiter certaines données sensibles sauf exceptions strictes. Or X-Corp traite des **données médicales** pour son produit HealthMed. Cela n'est possible que sous certaines conditions :

- **Consentement explicite des patients** ou nécessité pour la médecine préventive/les diagnostics médicaux. *X-Corp recueille le consentement spécifique des utilisateurs d'HealthMed.*

- **Mesures de sécurité renforcées**. *X-Corp pseudonymise les données médicales et les chiffre en AES-256.*

- **Accès restreint**. *Seuls certains employés habilités peuvent accéder aux données d'HealthMed, selon le principe du moindre privilège.*

## Les droits des personnes 

Le RGPD accorde aux individus des droits renforcés sur leurs données, que X-Corp doit respecter :

- **Droit d'accès** : les utilisateurs peuvent récupérer une copie de leurs données. *X-Corp reçoit 50 à 100 demandes d'accès par mois, auxquelles elle doit répondre sous 1 mois.*

- **Droit à l'effacement** : les utilisateurs peuvent demander la suppression de leurs données. *Sur EduLearn, le bouton "Supprimer mon compte" permet d'exercer ce droit.*

- **Droit à la portabilité** : les utilisateurs peuvent récupérer leurs données dans un format standard pour les transférer ailleurs. *Sur HealthMed, une fonctionnalité permet d'exporter son dossier médical au format HL7.*

## Les mesures de sécurité

Le RGPD impose de protéger les données avec des mesures appropriées. X-Corp a déployé :

- **Pseudonymisation** des données sensibles pour limiter l'impact en cas de fuite. 
- **Chiffrement AES-256** des données stockées et transmises.
- **Authentification forte** par 2FA pour les accès sensibles.
- **Gestion des habilitations** avec un système de contrôle d'accès basé sur les rôles (RBAC).

## Accountability : prouver la conformité

X-Corp ne doit pas seulement être conforme, elle doit pouvoir le démontrer :

- **Registre des traitements** listant les caractéristiques de chaque traitement (données, finalités, mesures de sécurité...). *X-Corp a cartographié ses 3 principaux traitements : RetailCo, HealthMed et EduLearn.*

- **DPIA** pour les traitements à risque (données sensibles, profilage...). *X-Corp réalise une DPIA avant chaque nouveau produit.*

- **Notifications des incidents** à la CNIL. *X-Corp a identifié des lacunes dans ses procédures de gestion des violations suite à une fuite de données de 2000 clients.*

## Conclusion 

Ce rapport montre que le RGPD impacte tous les aspects des traitements de données chez X-Corp : finalités, données collectées, sécurité, droits des utilisateurs, documentation de conformité... 

Des efforts importants ont été faits (nomination d'un DPO, DPIA, mesures de chiffrement et pseudonymisation...) mais des chantiers restent à mener, notamment sur la gestion des consentements et des violations de données.

L'audit complet permettra de dresser un état des lieux exhaustif et de construire un plan d'action conforme et adapté aux enjeux de X-Corp.