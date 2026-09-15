> **Pointer** : `05_Noyaux_masse_energie` → P4 (3 type-bac : EL hélium 2 méthodes, fission, stabilité) + VRAIE 2023N (QCM fission) → corrigés-types + pièges testés.
> Désintégrations (Soddy, $N(t)$, datation) → `04_Decroissance_radioactive`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Noyaux, masse et énergie (P05)

## Méthode — énergie nucléaire en 5 gestes 🧭

1. Équation : $A$/$Z$ des 2 côtés (Soddy — P04).
2. Masses en **u** (données !), $\Delta m$ = avant − après.
3. $\times 931{,}5$ = **MeV** (kg/joules UNIQUEMENT si demandé !).
4. Stabilité = $E_L/A$, jamais $E_L$ brute.
5. Ordre de grandeur : fission ~200, fusion ~18, $\alpha$ ~5 MeV.

## R1 — TYPE-BAC ($E_L$ de $^4He$, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P5 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $m_H = 1{,}00783$ u, $m_n = 1{,}00866$ u, $m_{He} = 4{,}00260$ u (atomiques) ; $m_p = 1{,}00728$ u, $m_e = 0{,}00055$ u. Calculer $E_L(^4He)$ et $E_L/A$.

**Corrigé-type — Méthode 1 (masses nucléaires).** $m_{noyau} = 4{,}00260 - 2(0{,}00055) = 4{,}00150$ u (retrancher les 2 électrons !). $\Delta m = 2(1{,}00728)+2(1{,}00866)-4{,}00150 = 4{,}03188-4{,}00150 = 0{,}03038$ u → $E_L = 0{,}03038\times931{,}5 = \boxed{28{,}3\text{ MeV}}$, $E_L/A = \boxed{7{,}07\text{ MeV/nucléon}}$.

**Corrigé-type — Méthode 2 (masses atomiques).** $\Delta m = 2m_H+2m_n-m_{He} = 2{,}01566+2{,}01732-4{,}00260 = 0{,}03038$ u (électrons : $2-2 = 0$, annulés !) → $\boxed{28{,}3\text{ MeV}}$, $\boxed{7{,}07\text{ MeV/nucléon}}$. Même résultat, zéro correction.
🪤 *Piège testé : M1 sans retrancher les électrons ($\Delta m = 0{,}02928$ → $27{,}3$ MeV, FAUX de 1 MeV !) — M2 (atomiques) évite ce piège : à préférer !*

## R2 — TYPE-BAC (fission : 200 MeV en main)

🏷️ matière=PC · année=— · session=— · chapitre=P5 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Fission $^{235}$U : $\Delta m = 0{,}21$ u/fission. a) $E$ en MeV puis en J. b) Énergie libérée par 1,0 g d'$^{235}$U ($N_A = 6{,}02\times10^{23}$) ?

**Corrigé-type.** a) $E = 0{,}21\times931{,}5 = \boxed{196\text{ MeV} \approx 200}$ ; $\times1{,}60\times10^{-13}$ → $\boxed{3{,}1\times10^{-11}\text{ J}}$. b) $N = (1/235)N_A = 2{,}56\times10^{21}$ → $E = 2{,}56\times10^{21}\times3{,}1\times10^{-11} = \boxed{8{,}0\times10^{10}\text{ J} \approx 22\text{ MWh}}$ (1 g = une ville !).
🪤 *Piège testé : $\Delta m$ en kg ($0{,}21\times1{,}66\times10^{-27}\times c^2$) — 3 conversions = 3 risques : rester en u ($\times931{,}5$) !*

## R3 — TYPE-BAC (stabilité : $E_L/A$ tranche)

🏷️ matière=PC · année=— · session=— · chapitre=P5 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $E_L(^{238}U) = 1800$ MeV, $E_L(^{56}Fe) = 492$ MeV. Quel est le noyau le plus stable ? Justifier.

**Corrigé-type.** $E_L/A$ : U : $1800/238 = 7{,}56$ MeV/nucléon ; Fe : $492/56 = 8{,}79$ MeV/nucléon. $\boxed{^{56}Fe}$ plus stable ($8{,}79 > 7{,}56$ — le fer est au sommet d'Aston !).
🪤 *Piège testé : « U (1800 > 492) » — comparer $E_L$ brute = comparer des pommes et des pastèques : TOUJOURS $/A$ !*

## VRAIE — 2023N Ex2-P1 (QCM fission)

🏷️ matière=PC · année=2023 · session=N · chapitre=P5 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

QCM : proposition E VRAIE (fission : la masse perdue → énergie libérée, $E = \Delta mc^2$).
🪤 *vraie : masse « perdue » = CONVERTIE (cinétique + $\gamma$) — l'énergie totale se conserve, c'est la forme qui change.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | électrons oubliés (M1) | M2 atomiques : annulation auto |
| R2 | calcul via kg | u → $\times931{,}5$ = MeV |
| R3 | stabilité sur $E_L$ brute | TOUJOURS $/A$ ! |
| 2023N | masse « disparue » | convertie ($E_{tot}$ conservée) |
