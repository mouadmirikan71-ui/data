> **Pointer** : `13_Rotation_solide_axe_fixe` → P4 (4 type-bac : disque, treuil, patineuse, roulement) → corrigés-types + R2 en 2 méthodes.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Rotation d'un solide (P13)

## Méthode — rotation en 5 gestes 🧭

1. Convertir : tr/min → rad/s ($\times 2\pi/60$), tours → rad.
2. $J$ par cœur (cerceau $mR^2$ > disque $\tfrac{1}{2}mR^2$ > sphère $\tfrac{2}{5}mR^2$).
3. Moments : $M = F\cdot d_\perp$, force par l'axe = 0.
4. Dynamique : $\Sigma M = J\ddot{\theta}$ ; ou énergie $\tfrac{1}{2}J\omega^2$.
5. Roulement : $v = R\omega$, $E_c$ = translation + rotation.

## R1 — TYPE-BAC (disque : tr/min → joules)

🏷️ matière=PC · année=— · session=— · chapitre=P13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Disque $m = 2,0$ kg, $R = 0,30$ m, $\omega = 120$ tr/min. $E_c$ ?

**Corrigé-type.** $\omega = 120\times2\pi/60 = 12,6$ rad/s ; $J = \tfrac{1}{2}\times2,0\times0,09 = 0,090$ kg·m² ; $E_c = \tfrac{1}{2}\times0,090\times12,6^2 = \boxed{7,1\text{ J}}$.
🪤 *Piège testé : $\omega = 120$ dans $\tfrac{1}{2}J\omega^2$ (→ 648 J, ×91 !) — convertir en rad/s EN PREMIER, toujours.*

## R2 — TYPE-BAC (treuil, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Treuil $R = 0,20$ m soulève $m = 50$ kg à $v = 0,50$ m/s (permanent). a) Couple résistant ? b) $\omega$ ?

**Corrigé-type.** a) Équilibre des moments : $M = mgR = 50\times9,8\times0,20 = \boxed{98\text{ N·m}}$.
b) **Méthode 1 (cinématique)** : $\omega = v/R = 0,50/0,20 = \boxed{2,5\text{ rad/s}}$ ($\approx 24$ tr/min). **Méthode 2 (puissance)** : $P = mgv = M\omega$ → $\omega = 245/98 = \boxed{2,5\text{ rad/s}}$ ✓ (et $P = 245$ W gratis !).
🪤 *Piège testé : $\omega = v\times R$ — $v = R\omega$ donc $\omega = v/R$ : le petit treuil tourne VITE ($R$ petit → $\omega$ grand).*

## R3 — TYPE-BAC (la patineuse accélère)

🏷️ matière=PC · année=— · session=— · chapitre=P13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Patineuse : $J_1 = 4,0$ kg·m² bras ouverts ($\omega_1 = 1$ tr/2 s), $J_2 = 1,5$ kg·m² bras serrés. $\omega_2$ ? $E_c$ avant/après ?

**Corrigé-type.** $\omega_1 = \pi$ rad/s. $J_1\omega_1 = J_2\omega_2$ → $\omega_2 = 4,0\pi/1,5 = \boxed{8,4\text{ rad/s}}$ ($\times 2,7$ !). $E_c$ : $19,7$ J → $52,6$ J : l'énergie a $\times 2,7$ — c'est le TRAVAIL des bras qui l'a fournie (moment cinétique conservé, énergie NON !).
🪤 *Piège testé : « $E_c$ conservée » — $J\omega$ = cste mais $E_c = (J\omega)^2/2J$ AUGMENTE quand $J$ diminue : quelqu'un a travaillé (les muscles) !*

## R4 — TYPE-BAC (roulement : qui vole l'énergie ?)

🏷️ matière=PC · année=— · session=— · chapitre=P13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Cylindre plein $m = 1,0$ kg descend $h = 1,0$ m (roulement sans glissement). $v$ en bas ? Comparer au glissement pur.

**Corrigé-type.** $\tfrac{1}{2}mv^2 + \tfrac{1}{2}J\omega^2 = mgh$, $J = \tfrac{1}{2}mR^2$, $\omega = v/R$ → $\tfrac{3}{4}mv^2 = mgh$ → $v = \sqrt{4gh/3} = \boxed{3,6\text{ m/s}}$ vs $\sqrt{2gh} = 4,4$ m/s en glissement : $1/3$ de l'énergie part en rotation !
🪤 *Piège testé : $v = \sqrt{2gh}$ direct — en ROULEMENT, $E_c$ = translation + rotation : oublier le $\tfrac{1}{2}J\omega^2$ = +22% d'erreur.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | tr/min dans formules | rad/s en 1re ligne |
| R2 | $\omega = vR$ | $v = R\omega$ → $\omega = v/R$ |
| R3 | $E_c$ conservée | $J\omega$ cste, $E_c$ non ! |
| R4 | rotation oubliée | roulement = 2 $E_c$ |
