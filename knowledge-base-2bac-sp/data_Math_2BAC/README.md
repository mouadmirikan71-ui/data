# Mathématiques 2BAC Sciences Physiques (Maroc) — Knowledge Base pour AI Teacher (Gemini)

> Base de connaissances RAG-ready : cours + Darija + méthodologie + examens + glossaire.
> Filière : 2ème année Bac — Sciences Physiques (SP / PC) — BIOF.
> Langues : Français (académique) + Darija marocaine (explication prof, alphabet arabe).
> Formules : **LaTeX** (`$...$` inline, `$$...$$` blocs) — parsable tel quel par Gemini/RAG.

## 1. Arborescence (dossier racine imposé : `data_Math_2BAC`)

```
data_Math_2BAC/
├── README.md + PLAN_COLLECTE.md   ← index, conventions, roadmap
├── 00_Programme_officiel/         ← curriculum Ministère + cadre de référence examen
├── 01_Limites_continuite/                     ← S1 : limites, FI, continuité, TVI
├── 02_Derivation_etude_fonctions/             ← S1 : dérivabilité, variations, branches infinies
├── 03_Suites_numeriques/                      ← S1 : convergence, monotonie, suites adjacentes
├── 04_Fonctions_primitives/                   ← S1 : primitives usuelles
├── 05_Fonction_logarithme_neperien/           ← S1 : ln, étude, équations
├── 06_Nombres_complexes_partie1/              ← S1 : forme algébrique, module, conjugué
├── 07_Fonctions_exponentielles/               ← S2 : exp, puissances, croissances comparées
├── 08_Nombres_complexes_partie2/              ← S2 : forme trigo/expo, équations, géométrie
├── 09_Calcul_integral/                        ← S2 : intégrales, IPP, aires
├── 10_Equations_differentielles/              ← S2 : y' = ay + b, y'' + ... (cadre SP)
├── 11_Produit_scalaire_espace/                ← S2 : orthogonalité, plans, sphères
├── 12_Produit_vectoriel_espace/               ← S2 : déterminant, plans, distances
├── 13_Denombrement/                           ← S2 : arrangements, combinaisons
├── 14_Probabilites/                           ← S2 : conditionnelles, indépendance, variable aléatoire, loi binomiale
├── 15_Methodologie/               ← rédaction de preuves, réflexes par question-type, pièges, gestion 3h
├── 16_Examens_nationaux/          ← sujets + corrigés 2015-2025 indexés + analyses
└── 17_Glossaire_FAQ/              ← glossaire FR→Darija + FAQ transversale
```

Chaque dossier chapitre `01..14` suit le **même gabarit** (copié de `data_SVT_2BAC`, adapté aux maths) :

| Fichier | Contenu | Type (tag) |
|---|---|---|
| `COURS.md` | Théorèmes + formules LaTeX + **intuition avant preuve** + شرح بالدارجة | `summary` |
| `COMPRENDRE_FACILEMENT.md` | **« How to understand this chapter the easy way »** — construction pas à pas en Darija + erreurs à éviter | `pedagogy` |
| `FAQ.md` | 6-10 questions d'élèves par chapitre, réponses FR + Darija | `faq` |
| `EXERCICES_TYPES.md` | Classiques bac + corrigés rédigés (étapes numérotées, justifications) | `exercise` / `answer-key` |
| `SOURCES.md` | Titre, URL, date d'accès | `meta` |

## 2. Convention de tags (en-tête YAML de chaque fichier)

```yaml
---
chapitre: "01 - Limites et continuité"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "AlloSchool + Manuel Massar Maths 2BAC SP + synthèse prof"
date_collecte: "2026-09-14"
type: "summary"   # summary | pedagogy | faq | exercise | answer-key | methodology | exam | glossary | meta
langues: "FR + Darija + LaTeX"
---
```

Règles RAG : texte brut `.md`, formules en LaTeX (jamais en images), chunks 300-800 tokens sur `##`,
Darija en alphabet arabe, termes FR gardés tels quels. Aucun faux « sujet officiel » inventé.

## 3. Sources de référence

1. Ministère EN — programme + **cadre de référence examen national Maths-SP** (via AlloSchool).
2. AlloSchool — Maths 2BAC SP BIOF : https://www.alloschool.com/course/mathematiques-2eme-bac-sciences-physiques-biof
3. Manuels Massar / Fadaa Maths 2BAC SP (transcriptions originales).
4. Annales corrigées (AlloSchool examens nationaux, sites profs marocains).
5. Synthèses « prof » (pédagogie Darija) — `source: synthèse prof`.

## 4. État d'avancement

- [x] Arborescence `data_Math_2BAC/` + gabarits
- [x] `00` Programme officiel (v1)
- [x] `15` Méthodologie épreuve (v1 complète)
- [x] `01` Chapitre modèle (limites & continuité, LaTeX + Darija + easy-way + FAQ)
- [ ] `02..14` COURS + COMPRENDRE_FACILEMENT + FAQ (phase 2)
- [ ] `16` index sujets/corrigés 2015-2025 + 3 corrigés transcrits analysés (phase 3)
- [ ] `17` glossaire ~150 termes FR→Darija (phase 3)
- [ ] Relecture + test RAG/Gemini (phase 4)

## 5. Utilisation avec Gemini (RAG / context window)

- Ingérer les `.md`, chunker sur `##`, filtrer via le YAML (`type`, `chapitre`).
- System prompt suggéré : « Tu es un prof marocain de maths 2BAC SP. Pour chaque notion : intuition + exemple simple d'abord (FR), puis théorème/formule en LaTeX, puis explication en Darija avec analogie, puis un piège classique et comment l'éviter. »
