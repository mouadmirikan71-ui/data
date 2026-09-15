# SVT 2BAC Sciences Physiques (Maroc) — Knowledge Base pour AI Teacher (Gemini)

> Base de connaissances RAG-ready : cours + Darija + méthodologie + examens + glossaire.
> Filière : 2ème année Bac — Sciences Physiques (SP / PC) — BIOF.
> Langues : Français (académique) + Darija marocaine (explication prof, en alphabet arabe).

## 1. Arborescence (dossier racine imposé : `data_SVT_2BAC`)

```
data_SVT_2BAC/
├── README.md                      ← ce fichier (index + conventions)
├── PLAN_COLLECTE.md               ← organisation + planning + avancement
├── 00_Programme_officiel/         ← curriculum Ministère + cadre de référence examen
├── 01_Liberation_energie_matiere_organique/   ← U1-Ch1 Respiration / Fermentation
├── 02_Muscle_strie_conversion_energie/        ← U1-Ch2 Muscle strié squelettique
├── 03_Notion_information_genetique/           ← U2-Ch1 ADN, mitose, réplication
├── 04_Expression_information_genetique/       ← U2-Ch2 Transcription, traduction
├── 05_Transfert_information_reproduction_sexuee/ ← U2-Ch3 Méiose, fécondation
├── 06_Lois_transmission_caracteres_hereditaires/ ← U2-Ch4 Monohybridisme, dihybridisme, génétique humaine
├── 07_Ordures_menageres_matieres_organiques/  ← U3-Ch1 Déchets ménagers
├── 08_Pollutions_matieres_energetiques/       ← U3-Ch2 Pollutions énergétiques
├── 09_Matieres_radioactives_energie_nucleaire/← U3-Ch3 Radioactivité, nucléaire
├── 10_Chaines_montagnes_tectonique_plaques/   ← U4-Ch1 Chaînes récentes + tectonique
├── 11_Deformations_tectoniques/               ← U4-Ch2 Plis, failles, chevauchements
├── 12_Metamorphisme_tectonique/               ← U4-Ch3 Métamorphisme
├── 13_Granitisation_magmatisme/               ← U4-Ch4 Granitisation, magmatisme
├── 14_Methodologie/               ← méthode épreuve SVT (QROC, graphes, schémas, mots-clés)
├── 15_Examens_nationaux/          ← sujets + corrigés 2015-2025 indexés + analyses
└── 16_Glossaire_FAQ/              ← glossaire FR→Darija + FAQ transversale
```

Chaque dossier chapitre `01..13` contient (même gabarit partout) :

| Fichier | Contenu | Type (tag) |
|---|---|---|
| `COURS.md` | Résumé FR + شرح بالدارجة + définitions + processus en texte | `summary` |
| `COMPRENDRE_FACILEMENT.md` | **« How to understand this chapter the easy way »** — leçon parlée en Darija, étape par étape, analogies | `pedagogy` |
| `FAQ.md` | 6-10 questions fréquentes par chapitre, réponses FR + Darija | `faq` |
| `EXERCICES_TYPES.md` | Exercices types bac + corrigés rédigés façon prof (mots-clés soulignés) | `exercise` / `answer-key` |
| `SOURCES.md` | Sources utilisées : titre, URL, date d'accès, licence/usage | `meta` |

## 2. Convention de tags (en-tête de chaque fichier)

Chaque fichier commence par un bloc YAML :

```yaml
---
chapitre: "01 - Libération de l'énergie emmagasinée dans la matière organique"
unite: "U1 - Consommation de la matière organique et flux d'énergie"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "AlloSchool + Manuel Massar SVT 2BAC SP + synthèse prof"
date_collecte: "2026-09-14"
type: "summary"   # summary | pedagogy | faq | exercise | answer-key | methodology | exam | glossary | meta
langues: "FR + Darija"
---
```

Règles RAG :
- Texte brut (.md), pas de scans/images — les schémas sont **décrits en texte** (ex. « Schéma : mitochondrie → … »).
- Chunks visés : 300-800 tokens ; titres `##`/`###` comme points de découpe.
- Darija en alphabet arabe, termes scientifiques gardés en français entre parenthèses.
- Zéro contenu inventé sur les examens : sujets/corrigés = transcription ou lien + analyse, jamais de faux « officiel ».

## 3. Sources de référence

1. Ministère de l'Éducation Nationale (Maroc) — programme + **cadre de référence de l'examen national SVT-SP** (via AlloSchool section 4008, élément 48555).
2. AlloSchool — SVT 2BAC SP BIOF (cours, exercices, examens nationaux) : https://www.alloschool.com/course/sciences-de-la-vie-et-de-la-terre-svt-2eme-bac-sciences-physiques-biof
3. Manuels Fadaa / Massar SVT 2BAC SP (transcriptions originales, pas de copie brute).
4. NéoSVT / Biologie-Maroc — index des examens nationaux + corrigés (2015-2025).
5. Synthèses « prof » rédigées pour ce projet (pédagogie Darija) — marquées `source: synthèse prof`.

## 4. État d'avancement (mis à jour à chaque phase)

- [x] Arborescence `data_SVT_2BAC/` + gabarits
- [x] `00` Programme officiel (v1)
- [x] `14` Méthodologie épreuve (v1 complète)
- [x] `01` Chapitre 1 complet (modèle de qualité pour les 12 autres)
- [ ] `02..13` COURS + COMPRENDRE_FACILEMENT + FAQ (phase 2)
- [ ] `14` fiches méthodes par exercice-type (phase 2)
- [ ] `15` index sujets/corrigés 2015-2025 + 3 corrigés transcrits analysés (phase 3)
- [ ] `16` glossaire ~150 termes FR→Darija (phase 3)
- [ ] Relecture homogénéité + test RAG/Gemini (phase 4)

## 5. Comment utiliser avec Gemini (RAG / context window)

- **RAG** : ingérer tous les `.md`, chunker sur `##`, filtrer par `type`/`chapitre` dans le YAML.
- **System prompt suggéré** : « Tu es un prof marocain de SVT 2BAC SP. Tu expliques d'abord en français simple, puis tu reformules en Darija avec une image de la vie quotidienne et une analogie. Tu termines par les mots-clés du bac. »
- **Garde-fou examen** : les fichiers `type: exam`/`answer-key` sont les seuls à citer pour « d'après le national 20XX ».
