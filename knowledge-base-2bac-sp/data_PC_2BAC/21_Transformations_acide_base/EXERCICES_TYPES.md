> **Pointer** : `21_Transformations_acide_base` → P4 (2 type-bac : 4 pH 2 méthodes, Henderson) + 2 VRAIES (2021N τ/Ka, 2023N double Henderson) → corrigés-types + pièges testés.
> Dosages (équivalence, $pH_{éq}$, indicateurs) → `22_Dosages_acido_basiques`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Acide-base (P21)

## Méthode — acide-base en 4 gestes 🧭

1. FORT ou faible ? (ouvre chaque exo !)
2. Fort : $pH = -\log C$ / $14+\log C$ ; faible : $\sqrt{}$ ($C/K_a > 100$ !) / Henderson.
3. Henderson : $[B]/[A]$ → $pH$ (et inverse !).
4. $\tau = 10^{-pH}/C$ → $K_a = C\tau^2/(1-\tau)$ → identité !

## R1 — TYPE-BAC (4 solutions : 2 méthodes de contrôle !)

🏷️ matière=PC · année=— · session=— · chapitre=P21 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $pH$ de 4 solutions $0{,}10$ M : HCl, $NaOH$, $CH_3COOH$ ($K_a = 1{,}8\times10^{-5}$), $NH_3$ ($K_b = 1{,}8\times10^{-5}$) ?

**Corrigé-type — Méthode 1 (formules directes).** HCl (fort) : $\boxed{1{,}0}$ ; $NaOH$ (forte) : $\boxed{13{,}0}$ ; acétique : $\sqrt{1{,}8\times10^{-6}} = 1{,}34\times10^{-3}$ → $\boxed{2{,}87}$ ; $NH_3$ : $[OH^-] = 1{,}34\times10^{-3}$ → $\boxed{11{,}13}$.

**Corrigé-type — Méthode 2 (contrôle via $\tau$ : cas acétique).** $\tau = 10^{-2{,}87}/0{,}10 = 1{,}35$ % → $K_a = C\tau^2/(1-\tau) = 0{,}10\times(0{,}0135)^2/0{,}9865 = \boxed{1{,}8\times10^{-5}}$ ✓ (retour au $K_a$ donné — le $pH$ est cohérent !).
🪤 *Piège testé : acétique « $pH = 1{,}0$ » — $-\log C$ = FORTS seulement : un faible à $0{,}10$ M a $pH = 2{,}87$ !*

## R2 — TYPE-BAC (Henderson : 2 sens !)

🏷️ matière=PC · année=— · session=— · chapitre=P21 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Couple acétique ($pK_a = 4{,}75$). a) $[AH]/[A^-] = 2{,}24$ : $pH$ ? b) $pH = 5{,}23$ : rapport $[B]/[A]$ ?

**Corrigé-type.** a) $[B]/[A] = 1/2{,}24$ → $pH = 4{,}75 + \log(1/2{,}24) = 4{,}75 - 0{,}35 = \boxed{4{,}40}$. b) $\log([B]/[A]) = 5{,}23 - 4{,}75 = 0{,}48$ → $[B]/[A] = 10^{0{,}48} = \boxed{3{,}0}$.
🪤 *Piège testé : a) $pH = 4{,}75 - \log(2{,}24)$ avec $[B]/[A] = 2{,}24$ (rapport INVERSÉ !) — $[AH]/[A^-] = 2{,}24$ → $[B]/[A] = 1/2{,}24$ : identifier $B$ ($A^-$) et $A$ ($AH$) AVANT !*

## VRAIE — 2021N Ex1-P2 ($\tau$ → $K_a$ → identité + Henderson)

🏷️ matière=PC · année=2021 · session=N · chapitre=P21 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

$AH + H_2O \rightleftharpoons A^- + H_3O^+$ : $\tau = 10^{-2{,}88}/0{,}1 = 1{,}32\%$ ($pH_0 = 2{,}88$). $Q_{r,éq} = C_a\tau^2/(1-\tau) = 1{,}77\times10^{-5} = K_a$ → $pK_a = 4{,}75$ → acide $= CH_3COOH$ (tableau). Henderson ($[AH]/[A^-] = 2{,}24$) : $pH = 4{,}75 - \log 2{,}24 = 4{,}4$.
🪤 *vraie : $\tau$ via $pH_0$ ($x_f = [H_3O^+]V$) ; $K_a = Q_{r,éq}$ ; $[AH]/[A^-]$ = rapport INVERSÉ !*
> Dosage associé ($V_{bE}$, $C_a$, $V_{b1}$) → P22 (VRAIE 2021N Ex1-P2).

## VRAIE — 2023N Ex1-P1/P2 (acétique + double Henderson !)

🏷️ matière=PC · année=2023 · session=N · chapitre=P21 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

$CH_3COOH$ ($C_A = 0{,}05$, $pH = 3{,}05$) : $\alpha = 1-\tau = 1-10^{-3{,}05}/0{,}05 = 98{,}2\%$ (quasi non dissocié !) ; $K_{A1} = 10^{-2pH}/(C_A-10^{-pH})$ → $pK_{A1} = 4{,}79}$. Réaction $CH_3COOH + HCOO^- \rightleftharpoons CH_3COO^- + HCOOH$ : $Q_{r,éq} = K_{A1}/K_{A2} = 10^{3{,}75-4{,}79} = 9{,}1\times10^{-2}$. Double Henderson (rapports inverses, logs annulés !) : $pH = (4{,}79+3{,}75)/2 = 4{,}27$.
🪤 *vraie : $Q_r = K_{A1}/K_{A2}$ (diviser les 2 Ka !) ; $pH$ moyen quand les rapports se compensent.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $-\log C$ partout | fort ou faible ? (M2 : contrôle $\tau$ !) |
| R2 | rapport inversé | $B = A^-$, $A = AH$ d'abord ! |
| 2021N | $K_a \neq Q_{r,éq}$ | $K_a = C\tau^2/(1-\tau)$ |
| 2023N | 2 Henderson séparés | rapports inverses → moyenne ! |
