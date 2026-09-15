> **Pointer** : `19_Transformations_non_totales_equilibre` → P4 (2 type-bac : xéq 2 méthodes, FeSCN) + VRAIE 2023N Ex1-P3 → corrigés-types + pièges testés.
> Quotient $Q_r$ + sens d'évolution → `20_Quotient_de_reaction_sens_evolution`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Non totales et équilibre (P19)

## Méthode — équilibre en 4 gestes 🧭

1. Tableau en $x$ (P17 !) → chaque $[\,](x)$.
2. $Q_r(x_{éq}) = K$ → équation (racine carrée si carrés !).
3. REJETER $x > x_{max}$ (parasite !).
4. $\tau = x_{éq}/x_{max}$ (total ≠ rapide !).

## R1 — TYPE-BAC ($x_{éq}$, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P19 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $1{,}0$ mol acide + $1{,}0$ mol alcool ($V = 1$ L), $K = 4$ (estérification). $x_{éq}$ ? $\tau$ ?

**Corrigé-type — Méthode 1 (racine).** $x^2/(1-x)^2 = 4$ → $x/(1-x) = 2$ → $x_{éq} = \boxed{0{,}67}$ → $\tau = \boxed{67\%}$.
**Corrigé-type — Méthode 2 (discriminant).** $3x^2-8x+4 = 0$ → $\Delta = 16$ → $x = 2$ (REJETÉ : $> x_{max} = 1$ !) ou $x = \boxed{0{,}67}$ ✓.
🪤 *Piège testé : garder $x = 2$ — TOUJOURS vérifier $x_{éq} \leq x_{max}$ : la racine parasite se fait piéger à chaque bac !*

## R2 — TYPE-BAC ($FeSCN^{2+}$ : limitée à 11 %)

🏷️ matière=PC · année=— · session=— · chapitre=P19 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $Fe^{3+} + SCN^- \rightleftharpoons FeSCN^{2+}$, $K = 140$, $[]_0 = 10^{-3}$ M chacun. a) Sens initial ? b) $x_{éq}$ ? c) $\tau$ ?

**Corrigé-type.** a) $Q_{r,i} = 0 < K$ → DIRECT. b) $140 = x/(10^{-3}-x)^2$ → $140u^2+u-10^{-3} = 0$ ($u = 10^{-3}-x$) → $u = 8{,}9\times10^{-4}$ → $x_{éq} = \boxed{1{,}1\times10^{-4}\text{ mol/L}}$. c) $\tau = \boxed{11\%}$ (limitée !).
🪤 *Piège testé : « $K = 140$ grand → totale » — $140 \ll 10^4$ : à ces DILUTIONS, même $K = 140$ donne $\tau = 11\%$ — $\tau$ dépend de $[]_0$ !*

## VRAIE — 2023N Ex1-P3 (estérification : 66,7 % → 70 %)

🏷️ matière=PC · année=2023 · session=N · chapitre=P19 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

Acide + méthanol ($n_0 = 0{,}9$) : $n_{af} = 0{,}3$ (graphe) → $x_f = 0{,}6$ → $r = 0{,}6/0{,}9 = 66{,}7\%$. Après ajout ($K = 4$) : $K = (0{,}6+x_{éq})^2/((0{,}4-x_{éq})(0{,}3-x_{éq}))$ → $3x^2-4x+0{,}12 = 0$ ($\Delta = 14{,}56$) → $x_{éq} = 0{,}031$ ($1{,}3$ REJETÉE : $> x_{max} = 0{,}3$ !) → $r' = 0{,}63/0{,}9 = 70\%$.
🪤 *vraie : $x_f$ via $n_{af}$ (lecture !) ; racine $> x_{max}$ rejetée (encore !).*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | racine $> x_{max}$ | vérifier $\leq x_{max}$ |
| R2 | $K$ « grand » = totale | $\tau$ dépend de $[]_0$ |
| 2023N | racine $1{,}3$ gardée | $x_{max} = 0{,}3$ = plafond ! |
