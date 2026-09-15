# Audit final — Base RAG 2BAC SP (2026-09-15)

> Snapshot post-Part 19 + bonus. Généré par audit automatisé + vérifications manuelles.

## 1. Couverture structurelle : 55/55 ✅

| Matière | Chapitres | Fichiers/chap (5 attendus) | Sans VRAIE |
|---|---|---|---|
| PC (P01–P28) | 28 | 5/5 partout (COURS, EXERCICES_TYPES, FAQ, SOURCES, COMPRENDRE_FACILEMENT) | 0 |
| Math (M01–M14) | 14 | 5/5 partout | 0 |
| SVT (S01–S13) | 13 | 5/5 partout | 0 |

Chaque chapitre : §9 « pourquoi » profond, §10 confusions, §11 signaux adaptatifs,
corrigés FR + Darija, pièges testés, ≥1 exercice en 2 méthodes (standard élevé).

## 2. Exercices : 379 tagués

| Matière | VRAIE verbatim (Tier A) | VRAIE reconstituées (Tier B) | Entraînement | Total |
|---|---|---|---|---|
| PC | 44 | 14 | 131 | 189 |
| Math | 42 | 1 | 57 | 100 |
| SVT | 31 | 23 | 36 | 90 |
| **Total** | **117** | **38** | **224** | **379** |

Règle : 100 % des headers VRAIE portent `type=VRAIE · fidélité=…` ; 0 entraînement
présenté comme national (audit automatisé, Part 19 §1 + vérif finale).

## 3. Pondérations (Σ = 100 × 3)

- **PC** : 37 sessions codées 2008N–2026N (cases vagues réparties, §1) — top : P21 10,75 · P08 7,89 · P15 5,92.
- **Math** : 37 sessions — 3 Tier A exactes + 32 Tier C **ESTIMÉ** (écrit en toutes lettres) — top : M02 16,75 · M03 12,58 · M08 11,55.
- **SVT** : 4 Tier A + signaux B — invariant 4 domaines × 5 pts — top : S01 19,2 · S08 16,7 · S10 15,8 · S06 13,3 · S04 11,7.
- Moteurs de sélection + index examens + priorités croisées : un jeu par matière.

## 4. Glossaires P5 : 156 / 157 / 156 ✅ (cible 150 dépassée)

FR exact bac + Darija imagée + exemple d'usage, par matière.

## 5. Sources vivantes / mortes

- Vivantes : neosvt.com (SVT 2023N/R, 2022R, 2021R intégraux), scribd (corrections PC 2024R/2025R, sujet Math 2025N), revisio.ma (catalogue, descriptions), alloschool (2017N), adrarphysic.fr (liens Drive 2026N — illisibles sandbox).
- Mortes : bestcours.net (squatté), jimdo/moutamadris (blocages fetch), recueils scannés sans OCR.

## 6. Non-résolus assumés (rien de caché)

1. S13 : 0 VRAIE, 0 item Tier A confirmé (poids 0 = support via S12).
2. P14 : VRAIE 2026N non relue (Drive) → R4 entraînement ciblé.
3. M09/M08/M10 : 0 VRAIE-verbatim (volumes/linéarisation/ED absents 2020–2026 Tier A).
4. Sessions SVT 2022N/2021N/2020N/2019/2025N/2024N : domaines non documentés.
5. Tier C Math (32 sessions) : estimé pur — à remplacer par lecture réelle si sources.
6. AN « à recouper » : P09 (F, m), P26 (r), P17 (t1/2, v), P22 (concentrations), P12 (α).

## 7. Prochaine étape proposée

Intégration RAG/Gemini à planifier ensemble (chunking, injection context-window,
évaluation) — la base est gelée et taguée pour ça.
