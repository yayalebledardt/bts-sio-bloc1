# BTS SIO — Portfolio E4 · Yanis Haddou

Dépôt de suivi des compétences pour l'**épreuve E4**, option SLAM,
2ᵉ année. Le Bloc 1 est le plus documenté, mais les blocs 2 et 3 sont
couverts aussi — la matrice de synthèse le montre.

Structure reprise du dépôt de suivi de la formation : une réalisation,
un dossier, une fiche de situation et ses preuves.

- **[`Excel_competences/Tableau_Synthese_E4.md`](Excel_competences/Tableau_Synthese_E4.md)**
  — la matrice compétences × réalisations, au format du fichier Excel
  officiel. C'est la vue d'ensemble : une ligne sans croix est un trou.
- **[`dashboard.md`](dashboard.md)** — les 18 savoirs du bloc, et où en
  est la preuve pour chacun.
- **[`Trame_Fiche_Situation_Professionnelle.md`](Trame_Fiche_Situation_Professionnelle.md)**
  — la trame vierge, pour les réalisations à venir.
- **`Realisations/`** — une fiche remplie par situation.

Le portfolio en ligne : **<https://yanis-haddou.vercel.app>**

---

## Les sept réalisations

| Réalisation | Compétences | État de la preuve |
| --- | --- | --- |
| [Production & variables d'environnement](Realisations/Stage_Production_Variables_Environnement/) | B1.1, B1.5, B2.2, B3.4 | ⚠️ à produire |
| [Parc & tickets GLPI](Realisations/Gestion_Parc_GLPI/) | B1.1, **B1.2** | ✅ deux PDF |
| [Agent de tri de courriels](Realisations/Agent_Tri_Mails/) | B1.5, **B2.1**, B2.3, **B3.1**, B3.3, B3.4 | ✅ 2 captures |
| [Site du podcast, légal & SEO](Realisations/Site_Podcast_Legal_SEO/) | **B1.3**, B2.2, B3.2, B3.4 | ✅ rapport + 3 captures |
| [KetaYaso / PrestaShop](Realisations/KetaYaso_PrestaShop/) | **B1.3**, B1.4 *sous condition*, B2.1, B2.3 | ⚠️ partielle |
| [Stripe, Vercel & passation](Realisations/Stripe_Vercel_Passation/) | **B1.4**, **B1.5**, B2.1, B2.2 | ✅ 3 captures |
| [Veille — IA & développement](Realisations/Veille_IA_Developpement/) | **B1.6** | ❌ aucune |

Les ✅ ont été vérifiés un par un : le document a été ouvert et répond en
ligne. Les ⚠️ et ❌ disent ce qui manque réellement — ce dépôt ne sert à
rien s'il enjolive.

---

## Les six compétences

| Code | Intitulé |
| --- | --- |
| B1.1 | Gérer le patrimoine informatique |
| B1.2 | Répondre aux incidents et aux demandes d'assistance et d'évolution |
| B1.3 | Développer la présence en ligne de l'organisation |
| B1.4 | Travailler en mode projet |
| B1.5 | Mettre à disposition des utilisateurs un service informatique |
| B1.6 | Organiser son développement professionnel |

---

## À produire avant la soutenance, par urgence

1. **Des entrées de veille.** Seul point à zéro. Trois entrées, une par
   semaine, trois paragraphes : ce que dit la source · ce que j'en
   retiens · ce que je vais essayer.
2. **Les preuves de la semaine 2 du stage** — `.env.example` anonymisé,
   extrait du contrôle au démarrage, et la capture de l'échec quand une
   variable manque. C'est la seule semaine sans capture, et c'est celle
   qui porte B1.1.
3. **Deux ou trois tickets GLPI reformatés** en symptôme → diagnostic →
   résolution → documentation.
4. **Les traces de suivi de KetaYaso** — Kanban ou Gantt, comptes rendus
   des points du lundi, composition de l'équipe. Sans elles, B1.4 ne
   tient pas.
5. **Trancher sur le dépôt KetaYaso** : public, ou confidentiel assumé
   avec extraits de code, schéma de base et diagramme de classes.

---

## Convention de commit

Un commit par savoir acquis ou par preuve ajoutée, pour que l'historique
raconte la progression :

```
docs: acquisition du savoir S6 — tickets GLPI reformatés
docs: preuve S15 — tableau de suivi KetaYaso
```
