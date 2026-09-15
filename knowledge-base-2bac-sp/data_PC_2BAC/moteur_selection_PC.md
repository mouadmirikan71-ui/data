---
doc: "Moteur de sélection d'exercices PC — spécification"
poids: "poids_chapitres_PC.json (poids_moteur, somme 100)"
principe: "lacunes d'abord, poids examen en arbitrage"
date: "2026-09-15"
---

# Moteur de sélection — exercices PC 2BAC SP

## 1. Principe (ordre de priorité strict)

1. **Lacunes de l'élève d'abord** : on travaille ce qu'il ne maîtrise pas.
2. **Poids examen en arbitrage** : à lacunes égales (± 0,05), le chapitre qui
   rapporte le plus au national passe devant.
3. **Quota plancher** : les chapitres du **top-8 poids** (P21, P08, P15, P11,
   P04, P25, P07, P01) obtiennent au moins 1 exercice dès que la séance
   comporte ≥ 6 exercices, même à lacune faible — on ne sacrifie jamais un
   gros chapitre.
4. **Transverses gratuits** : P19/P20/P23 ne prennent jamais un slot à eux
   seuls ; ils sont injectés comme sous-questions (τ, Qr/K) dans les exos
   P21/P22/P24/P25.

## 2. Entrées / sorties

- **Entrée** : `lacune[P01..P28]` ∈ [0,1] (0 = maîtrisé, 1 = non maîtrisé),
  `N` = nombre d'exercices voulus, `duree_min` optionnelle.
- **Sortie** : liste ordonnée de `N` chapitres (+ type d'exercice conseillé :
  VRAIE si dispo, sinon TYPE-BAC), respectant §1.

## 3. Algorithme (déterministe)

```
score(ch) = 0.65 * lacune(ch) + 0.35 * (poids_moteur(ch) / 10.75)   # 10.75 = max (P21)
trier chapitres par (lacune arrondie à 0.05 près, puis poids_moteur) décroissants
allouer les N slots dans cet ordre (1 slot maxi par chapitre au 1er passage,
  puis 2e passage pour les N > 28, impossible en pratique)
appliquer le quota plancher §1.3 (échanger le slot le plus faible contre le
  chapitre top-8 manquant le plus pondéré, sauf lacune = 0 stricte)
remplacer tout slot P16/P02/P27 (poids < 0.5) par le chapitre non pourvu le
  plus pondéré, sauf si sa lacune ≥ 0.8 (vrai besoin élève)
```

Complexité O(28 log 28). Implémentation de référence : lire
`poids_chapitres_PC.json`, appliquer ci-dessus (≤ 30 lignes, tout langage).

## 4. Exemple travaillé (N = 6)

Lacunes : P21 0,9 · P08 0,9 · P15 0,4 · P11 0,4 · P04 0,2 · P25 0,7 ·
P07 0,1 · P01 0,1 · autres ≤ 0,1.

1. Tri : P21 (0,9 ; 10,75) → P08 (0,9 ; 7,89) → P25 (0,7 ; 5,02) →
   P15 (0,4 ; 5,92) → P11 (0,4 ; 5,68) → P04 (0,2 ; 5,44).
   - P21 devant P08 : lacunes égales → arbitrage par poids ✓.
   - P15 devant P11 : même logique ✓.
2. 6 slots : P21, P08, P25, P15, P11, P04 — top-8 couverts à 6/8
   (P07, P01 absents : lacunes 0,1, quota plancher §1.3 non déclenché car
   N = 6 < 6 ? N = 6 → déclenché : P04 (lacune 0,2, poids 5,44) est
   échangé contre P07 (poids 5,00) ? Non : P04 ∈ top-8 déjà ;
   manquants = P07, P01 ; le slot le plus faible est P04 (top-8, gardé).
   Quota : 6 slots pour 8 chapitres → on garde les 6 premiers, P07/P01
   signalés « à planifier séance suivante ».
3. Types : P21 VRAIE (2026N/2025R dispo en base ? sinon TYPE-BAC dosage) ;
   P08 VRAIE ; P25 TYPE-BAC (scaffold) ; P15 TYPE-BAC (V0 → priorité
   d'enrichissement, cf. ponderation §6) ; P11 TYPE-BAC ; P04 VRAIE.
4. Transverses : τ (P19) + Ka (P21) dans l'exo P21 ; Qr/K (P20) dans P25.

## 5. Garde-fous

- Ne jamais proposer 2 fois le même chapitre avant d'avoir couvert tous les
  chapitres à lacune ≥ 0,5.
- P16/P02/P27 : uniquement si lacune ≥ 0,8 ou demande explicite.
- Tracer chaque sélection : `(chapitre, lacune, poids_moteur, motif)` —
  motif ∈ {lacune, arbitrage-poids, quota-top8}.
```

## 6. Évolutions prévues (ne pas implémenter sans le §5 de ponderation)

- Refonte des poids après chaque session (2026R, 2027…) : relancer le codage
  §1 de `ponderation_PC.md`.
- Quand P11/P25 sortiront du scaffold et P01/P14/P15/P24 auront leurs VRAIE,
  retirer la mention « priorité d'enrichissement » du §4 sans changer l'algo.
