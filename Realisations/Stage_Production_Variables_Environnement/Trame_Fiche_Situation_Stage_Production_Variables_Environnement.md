# FICHE DE SITUATION PROFESSIONNELLE (ÉPREUVE E4)

## 1. IDENTIFICATION GÉNÉRALE
- **Titre de la réalisation :** Fiabilisation d'un environnement de production : contrôle des variables d'environnement et optimisation de la base
- **Cadre de réalisation :** [x] Stage 1  [ ] Stage 2  [ ] Atelier de professionnalisation  [ ] Projet de cours
- **Période de réalisation :** Juin 2026 — semaine 2 du stage
- **Modalité :** [x] Individuel  [ ] En équipe
- **Localisation / Organisation cliente :** Diginumia

## 2. CONTEXTE ET OBJECTIFS
- **Contexte organisationnel :** Diginumia développe des applications métier pour ses clients. J'y arrive sur une application de coach sportif déjà en service, conçue dès le départ pour être revendue à des entreprises.
- **Problématique / Besoin exprimé :** L'application démarrait même lorsqu'une variable d'environnement nécessaire était absente. La panne ne se déclarait alors qu'à l'usage, loin de sa cause, au moment où personne ne peut plus la relier à la configuration.
- **Objectifs fixés :** Faire échouer le démarrage tôt et explicitement plutôt que tard et silencieusement ; optimiser la base PostgreSQL ; ramener l'ensemble des développements sur la branche principale.

## 3. DÉMARCHE ET ENVIRONNEMENT TECHNIQUE
- **Environnement technologique mobilisé :**
  - PostgreSQL
  - Git (intégration sur la branche principale)
  - Variables d'environnement, gestion des secrets
- **Démarche suivie étape par étape :**
  1. Recensement des variables dont l'application dépend réellement.
  2. Ajout d'un contrôle au démarrage : si une variable manque, l'application refuse de démarrer et dit laquelle.
  3. Optimisation de la base PostgreSQL.
  4. Intégration de l'ensemble des développements sur la branche principale.
- **Gestion des imprévus / Incidents rencontrés :** À compléter depuis le rapport de stage.

## 4. RÔLE ET CONTRIBUTION PERSONNELLE
- **Responsabilité précise :** Sécurisation de l'environnement de production de l'application.
- **Actions menées individuellement :** Écriture du contrôle de démarrage, optimisation de la base, intégration Git.

## 5. LIVRABLES ET PREUVES ASSOCIÉES
⚠️ **C'est la seule semaine du stage sans aucune capture dans le portfolio** (semaine 1 : 9, semaine 3 : 2, semaine 4 : 4, semaine 5 : 8, semaine 2 : 0). À produire avant la soutenance :

- [ ] `.env.example` anonymisé, listant les variables attendues
- [ ] Extrait commenté du code de contrôle au démarrage
- [ ] **Capture du message d'erreur quand une variable manque** — la preuve la plus parlante : elle montre le comportement, pas l'intention
- [ ] Avant / après de l'optimisation de la base, si une mesure existe

## 6. COMPÉTENCES SLAM MOBILISÉES
- [x] **B1.1 — Gérer le patrimoine informatique :** Le service existait déjà et tournait. Recenser ses dépendances, vérifier leur présence et faire échouer tôt, c'est veiller à son bon fonctionnement et à sa pérennité — pas développer une nouvelle vitrine.
- [ ] **B1.2 — Répondre aux incidents et demandes d'assistance :** —
- [ ] **B1.3 — Développer la présence en ligne :** —
- [ ] **B1.4 — Travailler en mode projet :** —
- [x] **B1.5 — Mettre à disposition des utilisateurs un service informatique :** Le résultat est un service qui reste disponible pour ses utilisateurs au lieu de tomber en cours d'usage.
- [ ] **B1.6 — Organiser son développement professionnel :** —

## 7. BILAN RÉFLEXIF ET AUTO-ÉVALUATION
- **Points forts :** Le choix de l'échec explicite au démarrage : une panne qui se déclare au bon endroit coûte infiniment moins cher à diagnostiquer.
- **Axes d'amélioration :** Aucune trace visuelle n'a été conservée sur le moment. La leçon vaut pour la suite : capturer pendant, pas après.
- **Compétences professionnelles consolidées :** Comprendre qu'un service en production se juge autant sur sa façon d'échouer que sur son fonctionnement nominal.
