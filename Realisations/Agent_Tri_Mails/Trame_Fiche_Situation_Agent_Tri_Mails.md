# FICHE DE SITUATION PROFESSIONNELLE (ÉPREUVE E4)

## 1. IDENTIFICATION GÉNÉRALE
- **Titre de la réalisation :** Agent de tri automatique de courriels — base de données, règles de classement et chiffrement
- **Cadre de réalisation :** [x] Stage 1  [ ] Stage 2  [ ] Atelier de professionnalisation  [ ] Projet de cours
- **Période de réalisation :** Juillet 2026 — semaine 3 du stage
- **Modalité :** [x] Individuel  [ ] En équipe
- **Localisation / Organisation cliente :** Diginumia

## 2. CONTEXTE ET OBJECTIFS
- **Contexte organisationnel :** Une boîte de réception professionnelle recevant un volume de courriels qu'un classement manuel ne tient plus.
- **Problématique / Besoin exprimé :** Classer automatiquement les courriels entrants dans les bons dossiers métier, sans confier aveuglément la décision à un modèle d'intelligence artificielle.
- **Objectifs fixés :** Concevoir la base, développer l'interface et l'API, et établir une logique de tri dont chaque décision reste explicable.

## 3. DÉMARCHE ET ENVIRONNEMENT TECHNIQUE
- **Environnement technologique mobilisé :**
  - PostgreSQL — base de douze tables
  - Node.js / Express — API
  - Python, API OpenAI — classement en dernier recours
  - Chiffrement AES-256
- **Démarche suivie étape par étape :**
  1. Conception de la base : douze tables.
  2. Développement de l'interface et de l'API.
  3. **Tri en cascade** : d'abord les fiches clients (une adresse connue), puis les règles d'expéditeur (domaine, préfixe), et **l'IA seulement en dernier recours**.
  4. Chiffrement AES-256 des données sensibles.
  5. Gestion des rôles (RBAC) et espace RGPD d'export et de suppression.
- **Gestion des imprévus / Incidents rencontrés :** À compléter depuis le rapport de stage.

## 4. RÔLE ET CONTRIBUTION PERSONNELLE
- **Responsabilité précise :** Conception et développement complets de l'outil.
- **Actions menées individuellement :** Modélisation de la base, API, interface, logique de tri, chiffrement, habilitations.

## 5. LIVRABLES ET PREUVES ASSOCIÉES
Voir [`Preuves/Preuves_global.md`](Preuves/Preuves_global.md) — deux captures de l'outil en fonctionnement.

## 6. COMPÉTENCES SLAM MOBILISÉES
- [x] **B1.1 — Gérer le patrimoine informatique :** —
- [ ] **B1.2 — Répondre aux incidents et demandes d'assistance :** —
- [ ] **B1.3 — Développer la présence en ligne :** —
- [ ] **B1.4 — Travailler en mode projet :** —
- [x] **B1.5 — Mettre à disposition des utilisateurs un service informatique :** L'outil est mis à disposition avec ses rôles et son espace RGPD.
- [ ] **B1.6 — Organiser son développement professionnel :** —
- [x] **B2.1 — Concevoir et développer une solution applicative :** Interface, API Node/Express et logique de tri développées de bout en bout.
- [x] **B2.3 — Gérer les données :** Base de douze tables conçue pour l'usage, et non héritée.
- [x] **B3.1 — Protéger les données à caractère personnel :** Chiffrement AES-256 et espace RGPD d'export et de suppression.
- [x] **B3.3 — Sécuriser les équipements et les usages :** Gestion des rôles (RBAC).
- [x] **B3.4 — Garantir disponibilité, intégrité et confidentialité :** Chiffrement au repos et cloisonnement par rôle.

## 7. BILAN RÉFLEXIF ET AUTO-ÉVALUATION
- **Points forts :** L'ordre de la cascade. Mettre l'IA en dernier et non en premier est une décision d'architecture, pas un détail : chaque courriel classé par une règle l'est pour une raison qu'on peut montrer. L'IA ne tranche que ce que les règles n'ont pas su trancher.
- **Axes d'amélioration :** Le taux de classement correct n'a pas été mesuré. Sans chiffre, impossible de dire si la cascade fonctionne mieux qu'une IA seule — c'est pourtant l'argument central.
- **Compétences professionnelles consolidées :** Concevoir une base pour un usage précis, et placer un modèle probabiliste à l'endroit où son erreur coûte le moins cher.
