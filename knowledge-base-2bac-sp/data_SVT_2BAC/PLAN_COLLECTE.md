# Plan de collecte — data_SVT_2BAC (SVT 2BAC SP, Maroc)

## A. Comment les données seront organisées

**1 dossier racine imposé** : `data_SVT_2BAC/` (17 sous-dossiers, voir README.md).

- **13 dossiers chapitres** (`01`→`13`) calqués sur le programme officiel (4 unités) :
  - U1 Consommation de la matière organique : Ch1 libération d'énergie (respiration/fermentation), Ch2 muscle strié.
  - U2 Génétique : Ch3 notion d'information génétique, Ch4 expression (transcription/traduction), Ch5 méiose/fécondation, Ch6 lois de Mendel + génétique humaine.
  - U3 Matières organiques/inorganiques : Ch7 déchets, Ch8 pollutions énergétiques, Ch9 radioactivité/nucléaire.
  - U4 Géologie : Ch10 chaînes de montagnes/tectonique, Ch11 déformations, Ch12 métamorphisme, Ch13 granitisation.
- **3 dossiers transverses** : `14_Methodologie` (LA pièce qui fait la différence au bac), `15_Examens_nationaux` (2015-2025 + corrigés), `16_Glossaire_FAQ` (FR→Darija).
- **1 dossier cadre** : `00_Programme_officiel` (ce qui est exigible, barème, format d'épreuve).
- **5 fichiers par chapitre** : `COURS.md` / `COMPRENDRE_FACILEMENT.md` (« How to understand this chapter the easy way ») / `FAQ.md` / `EXERCICES_TYPES.md` / `SOURCES.md`.
- **Tags uniformes** : chaque fichier = bloc YAML `chapitre, source, date_collecte, type` → filtrable par le RAG, traçable jusqu'à la source.

**Style prof imposé** (différence vs « IA sèche ») : chaque notion = 1) image de la vie réelle → 2) concept FR simple → 3) « pourquoi » (le mécanisme, pas juste le « quoi ») → 4) reformulation en Darija avec analogie → 5) mots-clés bac. C'est écrit dans le gabarit, donc Gemini hérite du style en citant la base.

## B. Combien de temps ça prendra

Travail en **4 phases**. Base : sessions agent de ~1-2 h. Entre crochets = livrable vérifiable dans le repo.

| Phase | Contenu | Durée estimée | Livrable |
|---|---|---|---|
| **Phase 1 — Squelette + modèle qualité** (EN COURS) | Arborescence, README, programme officiel v1, méthodologie complète, **chapitre 01 exemplaire**, gabarits | **Cette session (1-2 h)** | Dossiers + 5 fichiers de référence |
| **Phase 2 — Les 12 chapitres restants** | Pour `02`→`13` : COURS + COMPRENDRE_FACILEMENT + FAQ (FR+Darija, style prof) | **2-3 sessions (~4-6 h)** — ~30-45 min par chapitre en qualité prof | 36 fichiers |
| **Phase 3 — Examens + glossaire** | Index sujets/corrigés 2015-2025 (liens + métadonnées), transcription+analyse de 3-5 nationaux récents, glossaire ~150 termes FR→Darija, FAQ transversale | **1-2 sessions (~2-4 h)** | `15/` + `16/` complets |
| **Phase 4 — Finition RAG** | EXERCICES_TYPES par chapitre, SOURCES partout, relecture homogénéité, test d'injection Gemini (chunking, prompt système) | **1 session (~1-2 h)** | Base complète, testée |

**Total estimé : 5-7 sessions, soit ~8-14 h de travail agent**, étalées selon ta disponibilité (ex. 1 session/jour → base complète en une semaine).

> Pourquoi pas « tout en 1 heure » ? La valeur = la pédagogie Darija + les corrigés rédigés façon prof + la vérification anti-hallucination sur les examens. Un scrape brut d'AlloSchool prendrait 20 minutes mais donnerait une IA sèche — l'inverse de ton objectif.

## C. Ce qui est déjà fait dans cette session (Phase 1)

1. ✅ Arborescence complète `data_SVT_2BAC/` (17 dossiers).
2. ✅ `README.md` (index + convention RAG) + ce plan.
3. ✅ `00_Programme_officiel/programme_officiel.md` (v1 : unités, chapitres, format d'épreuve, cadre de référence).
4. ✅ `14_Methodologie/methodologie_epreuve_SVT.md` (méthode complète : QROC, graphes, schémas, génétique, gestion temps).
5. ✅ `01_Liberation_energie_matiere_organique/COURS.md` — le chapitre-modèle (FR + Darija + easy-way + FAQ + mots-clés).

## D. Prochaines étapes proposées (ordre conseillé)

1. Valider le **style du chapitre 01** (Darija en alphabet arabe ? niveau de détail ?).
2. Lancer Phase 2 : chapitres `02, 03, 04` (bioénergétique + génétique moléculaire = le cœur du national).
3. Puis `05, 06` (méiose + Mendel), `10-13` (géologie), `07-09` (environnement).
4. Phase 3 (examens + glossaire), Phase 4 (finition + test Gemini).

## E. Points à confirmer avec toi

1. **Darija** : alphabet arabe (الحالي, recommandé pour le RAG) vs arabizi (latin) ? — modifiable globalement.
2. Faut-il inclure aussi la **version arabe (مسلك عربي)** ou rester 100 % BIOF (français) ?
3. Pour les examens : transcription intégrale de quelques sujets (lourd mais top pour RAG) vs liens + analyses détaillées (léger, pas de risque copyright) ? Recommandation : liens + analyses + 3 transcriptions.
