> **Pointer** : `18_Suivi_temporel_vitesse_reaction` → P4 (3 type-bac : vitesse 2 méthodes, spectro, titrage+trempe) + VRAIE 2021N Ex1-P1 → corrigés-types + pièges testés.
> Socle (tableau, $t_{1/2}$, facteurs) → `17_Transformations_lentes_et_rapides`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Suivi temporel et vitesse (P18)

## Méthode — suivi+vitesse en 5 gestes 🧭

1. Grandeur $= f(x)$ (tableau P17 !) puis inverser.
2. Vitesse = pente TANGENTE ÷ $V$.
3. Via espèce : ÷ $\nu$ !
4. $t_{1/2}$ : $x_{max}/2$ → grandeur → projeter.
5. $A = \varepsilon lC$ ($l$ en cm !).

## R1 — TYPE-BAC (vitesse, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P18 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $2H_2O_2 \to 2H_2O + O_2$ ($V = 0{,}10$ L). $x$ (mmol) : $t = 120$ s → $2{,}5$ ; $t = 240$ s → $3{,}8$. Vitesse moyenne sur $[120, 240]$ ?

**Corrigé-type — Méthode 1 (via $x$).** $v = \Delta x/(\Delta t\cdot V) = 1{,}3\times10^{-3}/(120\times0{,}10) = \boxed{1{,}1\times10^{-4}\text{ mol·L}^{-1}\text{·s}^{-1}}$.
**Corrigé-type — Méthode 2 (via $[H_2O_2]$).** $[]_{120} = 0{,}050$ M, $[]_{240} = 0{,}024$ M → $v = -(\Delta C/2)/\Delta t = 0{,}026/(2\times120) = \boxed{1{,}1\times10^{-4}}$ ✓ (÷2 = coefficient !).
🪤 *Piège testé : M2 sans ÷2 ($2{,}2\times10^{-4}$) — $v = v_{disp}/\nu$ : via une ESPÈCE, diviser par son coefficient ; via $x$, rien !*

## R2 — TYPE-BAC (suivi spectro : $A = A_\infty/2$ !)

🏷️ matière=PC · année=— · session=— · chapitre=P18 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $S_2O_8^{2-} + 2I^- \to 2SO_4^{2-} + I_2$, $n(S_2O_8)_0 = 0{,}20$ mmol, $n(I^-)_0 = 1{,}0$ mmol, $V = 0{,}20$ L, $\varepsilon(I_2) = 2000$, $l = 1$ cm. a) $x_{max}$ ? b) $A_\infty$ ? c) $A = 1{,}0$ : où en est-on ?

**Corrigé-type.** a) $x_{max} = \min(0{,}20/1 ; 1{,}0/2) = \boxed{0{,}20\text{ mmol}}$ ($S_2O_8$ limitant). b) $[I_2]_\infty = 0{,}20\times10^{-3}/0{,}20 = 1{,}0\times10^{-3}$ M → $A_\infty = 2000\times1\times10^{-3} = \boxed{2{,}0}$. c) $A = 1{,}0 = A_\infty/2$ → $[I_2] = 5{,}0\times10^{-4}$ → $x = 0{,}10$ mmol $= x_{max}/2$ → $\boxed{t = t_{1/2}}$ !
🪤 *Piège testé : $x_{max} = 1{,}0/2$ « $I^-$ limitant » — comparer $n_0/\nu$ des DEUX : $0{,}20 < 0{,}50$ → $S_2O_8$ !*

## R3 — TYPE-BAC (suivi par titrage + trempe)

🏷️ matière=PC · année=— · session=— · chapitre=P18 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $2H_2O_2 \to 2H_2O + O_2$ ($n_0 = 0{,}010$ mol, $V = 0{,}10$ L). À $t = 5$ min, on prélève $10$ mL (trempe !) : le titrage donne $n(H_2O_2) = 0{,}80$ mmol dans le prélèvement. $x$ à $t = 5$ min ? Pourquoi la trempe ?

**Corrigé-type.** $C = 0{,}80\times10^{-3}/0{,}010 = 0{,}080$ M → $n_{restant} = 0{,}080\times0{,}10 = 8{,}0$ mmol → $x = (10{,}0-8{,}0)/2 = \boxed{1{,}0\text{ mmol}}$ (÷2 = $\nu$ !). Trempe : figer $x$ (froid → $v \approx 0$) — sans elle, la réaction continue pendant le dosage → $x$ faux !
🪤 *Piège testé : $x = 10{,}0 - 8{,}0 = 2{,}0$ (÷$\nu$ oublié !) — $n = n_0 - \nu x$ → $x = (n_0-n)/\nu$ : diviser par 2 !*

## VRAIE — 2021N Ex1-P1 (saponification conductimétrique)

🏷️ matière=PC · année=2021 · session=N · chapitre=P18 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

Saponification $CH_3COOC_2H_5 + HO^-$ (ester en excès), $\sigma = 0{,}25 - 160x$ ($V_0 = 100$ mL). $x_{max} = n_0(HO^-) = 1{,}0\times10^{-3}$ mol ($HO^-$ limitant). $t_{1/2}$ : $x = x_{max}/2 = 5\times10^{-4}$ → $\sigma_{1/2} = 0{,}17$ S/m → lecture graphe $t_{1/2} = 4$ min. Vitesse : $v = -(1/160V_0)(d\sigma/dt)$ ; à $t_1$ : pente $(0{,}17-0{,}22)/4$ → $V_1 = 0{,}781$ mol·m⁻³·min⁻¹.
🪤 *vraie : unités mol·m⁻³·min⁻¹ ($V_0$ en m³ !) ; $t_{1/2}$ via $\sigma$ (convertir $x \to \sigma$ d'abord !).*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $\nu$ oublié via $[]$ | $v = v_{esp}/\nu$ |
| R2 | limitant au hasard | $\min(n_0/\nu)$ |
| R3 | $x = n_0 - n$ (÷$\nu$ !) | $x = (n_0-n)/\nu$ |
| 2021N | $\sigma_{1/2} = \sigma_{max}/2$ | convertir $x \to \sigma$ d'abord ! |
