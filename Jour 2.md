# Registre des traitements — X-Corp

## Préambule méthodologique

Ce registre est établi exclusivement à partir de la fiche `Entreprise Fictive X-corp.md`.
Les informations non renseignées dans cette fiche sont explicitement marquées
`[Non précisé dans la fiche X-Corp]` et font l'objet de recommandations, plutôt que
d'être complétées par hypothèse.

**Qualification du rôle de X-Corp** : la fiche ne qualifie explicitement le rôle de
X-Corp pour aucun des trois traitements. L'analyse des finalités (déterminées par
les clients RetailCo, HealthMed et EduLearn) conduit à retenir l'hypothèse d'une
qualification de **sous-traitant** au sens de l'article 4-8 du RGPD, à confirmer
par la revue des contrats. Cette qualification conditionne le régime applicable
(article 28 et article 30.2).

---

## Traitement n°1 — Gestion des clients pour RetailCo

| Champ | Valeur |
|---|---|
| Responsable de traitement | RetailCo (hypothèse d'analyse — non qualifié dans la fiche) |
| Rôle de X-Corp | Sous-traitant (hypothèse d'analyse — à confirmer par les contrats) |
| DPO | Un DPO a été nommé chez X-Corp. Identité et coordonnées : `[Non précisé dans la fiche X-Corp]` |
| Finalité | Personnalisation des offres et des promotions, amélioration de l'expérience client |
| Catégories de personnes concernées | Clients de RetailCo — 800 000 personnes |
| Catégories de données | Noms, adresses, emails, numéros de téléphone, historique d'achats, préférences de produits |
| Base légale | Consentement des clients |
| Destinataires | `[Non précisé dans la fiche X-Corp]` — la fiche cite deux partenaires technologiques (CloudSecure, stockage cloud sécurisé ; AdBoost, publicité digitale ciblée) sans préciser leur rattachement à ce traitement |
| Transferts hors UE | `[Non précisé dans la fiche X-Corp]` |
| Durée de conservation | 5 ans après le dernier contact |
| Mesures de sécurité | Mesures globales X-Corp : pseudonymisation des données sensibles, chiffrement AES-256 en transit et au repos, authentification à deux facteurs pour l'accès aux systèmes internes, contrôle d'accès basé sur les rôles (RBAC). La fiche ne précise pas leur déclinaison par traitement. |
| Points de vigilance | • La fiche signale des difficultés à gérer et documenter les consentements marketing, notamment pour les campagnes via AutoMail — ce qui affecte directement la base légale de ce traitement.<br>• Absence de contrat de sous-traitance documenté (article 28).<br>• Destinataires non identifiés : incompatible avec l'exigence de l'article 30. |

---

## Traitement n°2 — Suivi des patients pour HealthMed

| Champ | Valeur |
|---|---|
| Responsable de traitement | HealthMed (hypothèse d'analyse — non qualifié dans la fiche) |
| Rôle de X-Corp | Sous-traitant (hypothèse d'analyse — à confirmer par les contrats) |
| DPO | Un DPO a été nommé chez X-Corp. Identité et coordonnées : `[Non précisé dans la fiche X-Corp]` |
| Finalité | Suivi des traitements, rappel des rendez-vous, personnalisation des conseils de santé |
| Catégories de personnes concernées | Patients de HealthMed — 500 000 personnes |
| Catégories de données | Noms, adresses, emails, numéros de téléphone, historique médical, prescriptions |
| | ⚠️ Données de santé = catégorie particulière au sens de l'article 9 |
| Base légale | Consentement explicite des patients (article 9.2.a) |
| Destinataires | `[Non précisé dans la fiche X-Corp]` |
| Transferts hors UE | `[Non précisé dans la fiche X-Corp]` |
| Durée de conservation | 10 ans après la fin du traitement médical |
| Mesures de sécurité | Mesures globales X-Corp (voir traitement n°1). La fiche ne précise aucune mesure renforcée spécifique aux données de santé. |
| Points de vigilance | • Traitement à grande échelle de données de santé : justifie à lui seul l'obligation de désigner un DPO (article 37.1.c) et rend une AIPD très probablement obligatoire (article 35.3.b).<br>• Le consentement explicite est une base valable (article 9.2.a) mais fragile : son retrait doit être aussi simple que son recueil, or la fiche signale des difficultés de gestion des consentements.<br>• Aucun hébergeur de données de santé (HDS) mentionné.<br>• Aucune mesure de sécurité différenciée pour ces données malgré leur sensibilité. |

---

## Traitement n°3 — Analyse de l'usage pour EduLearn

| Champ | Valeur |
|---|---|
| Responsable de traitement | EduLearn (hypothèse d'analyse — non qualifié dans la fiche) |
| Rôle de X-Corp | Sous-traitant (hypothèse d'analyse — à confirmer par les contrats) |
| DPO | Un DPO a été nommé chez X-Corp. Identité et coordonnées : `[Non précisé dans la fiche X-Corp]` |
| Finalité | Amélioration des parcours d'apprentissage, recommandations de cours, suivi des progrès |
| Catégories de personnes concernées | Utilisateurs de la plateforme EduLearn — 300 000 personnes |
| Catégories de données | Identifiants utilisateurs, adresses email, parcours d'apprentissage, résultats d'examen |
| Base légale | Consentement des utilisateurs |
| Destinataires | `[Non précisé dans la fiche X-Corp]` |
| Transferts hors UE | `[Non précisé dans la fiche X-Corp]` |
| Durée de conservation | 2 ans après la fin de l'utilisation de la plateforme |
| Mesures de sécurité | Mesures globales X-Corp (voir traitement n°1) |
| Points de vigilance | • La finalité de recommandation de cours implique un profilage des apprenants (article 4-4).<br>• L'âge des utilisateurs n'est pas précisé : si la plateforme accueille des mineurs, le régime de l'article 8 s'applique (consentement du titulaire de la responsabilité parentale).<br>• Les résultats d'examen sont des données à impact potentiel sur le parcours des personnes : leur exactitude relève de l'article 5.1.d. |
