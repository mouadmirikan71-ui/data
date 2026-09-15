# Plan de collecte — data_Math_2BAC (Maths 2BAC SP, Maroc)

## A. Organisation des données

**1 dossier racine** : `data_Math_2BAC/` (18 sous-dossiers, voir README.md) — miroir de `data_SVT_2BAC/` pour une maintenance uniforme.

- **14 dossiers chapitres** (`01`→`14`) calqués sur le programme officiel SP :
  - S1 : limites/continuité, dérivation/étude de fonctions, suites, primitives, ln, complexes (partie 1).
  - S2 : exp, complexes (partie 2), intégrales, équations différentielles, produit scalaire/vectoriel dans l'espace, dénombrement, probabilités.
- **3 dossiers transverses** : `15_Methodologie` (rédaction de preuves, réflexes, pièges), `16_Examens_nationaux` (2015-2025), `17_Glossaire_FAQ` (FR→Darija).
- **1 dossier cadre** : `00_Programme_officiel`.
- **5 fichiers par chapitre** : `COURS.md` / `COMPRENDRE_FACILEMENT.md` (« How to understand this chapter the easy way » + erreurs à éviter) / `FAQ.md` / `EXERCICES_TYPES.md` / `SOURCES.md`.
- **Tags uniformes** : YAML `chapitre, source, date_collecte, type` → filtrable par le RAG.
- **Style prof imposé** : chaque notion = 1) intuition/exemple simple → 2) théorème/formule LaTeX → 3) « pourquoi ce théorème existe » → 4) Darija + analogie (ex. dérivée = vitesse) → 5) piège classique + comment l'éviter.

## B. Durée estimée (4 phases, sessions agent ~1-2 h)

| Phase | Contenu | Durée | Livrable |
|---|---|---|---|
| **Phase 1 — EN COURS** | Arborescence, README, programme v1, méthodologie complète, **chapitre 01 modèle**, gabarits | **Cette session (1-2 h)** | Dossiers + 5 fichiers de référence |
| **Phase 2 — Cœur (13 chapitres)** | Pour `02`→`14` : COURS (LaTeX) + COMPRENDRE_FACILEMENT + FAQ (FR+Darija) | **3-4 sessions (~5-8 h)** — les chapitres analyse (02, 03, 09) sont les plus lourds | 39 fichiers |
| **Phase 3 — Examens + glossaire** | Index sujets/corrigés 2015-2025, transcription+analyse de 3-5 nationaux récents (corrigés détaillés), glossaire ~150 termes | **1-2 sessions (~3-5 h)** — les corrigés maths détaillés sont longs à rédiger proprement | `16/` + `17/` |
| **Phase 4 — Finition RAG** | EXERCICES_TYPES par chapitre, SOURCES partout, relecture homogénéité LaTeX, test Gemini | **1 session (~1-2 h)** | Base complète testée |

**Total estimé : 6-8 sessions, ~10-17 h**, étalées selon ta dispo (ex. 1 session/jour → ~une semaine).
> Les maths coûtent un peu plus cher que la SVT : chaque corrigé national = 4-5 exercices avec preuves complètes en LaTeX propre. C'est précisément ce qui fera la différence « vrai prof » vs « IA sèche ».

## C. Fait dans cette session (Phase 1)

1. ✅ Arborescence complète `data_Math_2BAC/` (18 dossiers).
2. ✅ `README.md` + ce plan.
3. ✅ `00_Programme_officiel/programme_officiel.md` (v1).
4. ✅ `15_Methodologie/methodologie_epreuve_maths.md` (méthode complète).
5. ✅ `01_Limites_continuite/COURS.md` — chapitre modèle (LaTeX + Darija + easy-way + FAQ + pièges).

## D. Ordre conseillé pour la Phase 2

1. `03` Suites + `02` Dérivation/étude de fonctions (le gros du problème d'analyse au national).
2. `06` + `08` Complexes (exercice quasi-systématique, très rentable).
3. `05` ln + `07` exp + `09` intégrales + `04` primitives (bloc fonctions).
4. `13` + `14` Dénombrement/probas, `11` + `12` géométrie espace, `10` équa. diff.

## E. Points à confirmer

1. **Darija** : alphabet arabe (actuel, recommandé) vs arabizi ? — modifiable globalement.
2. **LaTeX** : `$...$`/`$$...$$` (actuel, standard) vs autre format ?
3. **Examens** : transcriptions intégrales de quelques sujets (top RAG, lourd) vs liens + analyses (léger) ? Recommandation : liens + analyses + 3 transcriptions (voir SVT).
4. Faut-il traiter aussi la **branche arabe (مسلك عربي)** ou rester BIOF ?
