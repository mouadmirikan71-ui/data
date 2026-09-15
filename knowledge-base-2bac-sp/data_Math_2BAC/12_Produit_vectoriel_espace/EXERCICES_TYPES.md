> **Pointer** : `12_Produit_vectoriel_espace` → P4 (1 vraie 2025N Ex.1-Q3 + 4 type-bac) → corrigés-types + R2 en 2 méthodes.

# Exercices types — Produit vectoriel dans l'espace (M12)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Données 2025N (Ex.1 Q3 — $\wedge$ → plan)

$A(0,0,2)$, $B(2,0,0)$, $M(0,m,0)$. Source : etude-generale (2025 Normale SP, énoncé réel ; corrigé-type prof recoupé).

## Q1 — VRAIE (2025 N, Ex.1 Q3a+Q3b)

🏷️ matière=Math · année=2025 · session=N · chapitre=M12 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « Vérifier $\overrightarrow{AB} \wedge \overrightarrow{AM} = 2m\vec{i} + 4\vec{j} + 2m\vec{k}$ » ; « Déduire que $mx+2y+mz-2m = 0$ est une équation de $(ABM)$ ».

**Corrigé-type.** $\overrightarrow{AB}(2,0,-2)$, $\overrightarrow{AM}(0,m,-2)$ : $\wedge = (0\times(-2)-(-2)m,\; (-2)\times0-2\times(-2),\; 2m-0\times0) = \boxed{(2m,4,2m)}$ ✓. Test : $(2m,4,2m)\cdot(2,0,-2) = 4m-4m = 0$ ✓. Normal $\parallel (m,2,m)$ → $mx+2y+mz+d = 0$ ; $A(0,0,2)$ → $2m+d = 0$ → $\boxed{mx+2y+mz-2m = 0}$ (valable aussi pour $m = 0$ : $y = 0$ = plan $(OAB)$ ✓).
🪤 *Piège testé : diviser par $m$ (« simplifier » le normal) — $m$ peut être NUL : garder $(2m,4,2m)$, la composante 4 ne s'annule jamais.*

## R1 — TYPE-BAC (calcul + vérification)

🏷️ matière=Math · année=— · session=— · chapitre=M12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** $\vec{u}(1,2,3)$, $\vec{v}(4,5,6)$. Calculer $\vec{u} \wedge \vec{v}$ + vérifier.

**Corrigé-type.** $(2\times6-3\times5,\; 3\times4-1\times6,\; 1\times5-2\times4) = \boxed{(-3,6,-3)}$. Tests : $\cdot\vec{u} = -3+12-9 = 0$ ✓ ; $\cdot\vec{v} = -12+30-18 = 0$ ✓.
🪤 *Piège testé : 2ᵉ composante $-6$ — $+,-,+$ puis test scalaire.*

## R2 — TYPE-BAC (plan par 3 points, 2 méthodes !)

**Énoncé.** $A(1,0,0)$, $B(0,1,0)$, $C(0,0,1)$. Équation de $(ABC)$ ?

**Corrigé-type — M1 ($\wedge$).** $\overrightarrow{AB} \wedge \overrightarrow{AC} = (1,1,1)$ → $x+y+z+d = 0$, $A$ → $\boxed{x+y+z-1 = 0}$. **M2 (intercepts).** Coupe les axes en 1 : $\boxed{x/1+y/1+z/1 = 1}$.
🪤 *Piège testé : normal $(-1,-1,-1)$ « différent » — opposé = même plan.*

## R3 — TYPE-BAC (aire d'un triangle)

🏷️ matière=Math · année=— · session=— · chapitre=M12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Mêmes points : aire de $ABC$ ?

**Corrigé-type.** $\frac{1}{2}\|(1,1,1)\| = \boxed{\sqrt{3}/2}$.
🪤 *Piège testé : $\sqrt{3}$ sans $1/2$ — triangle = moitié.*

## R4 — TYPE-BAC (test de colinéarité)

🏷️ matière=Math · année=— · session=— · chapitre=M12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** $\vec{u}(2,-1,3)$, $\vec{v}(4,-2,6)$, $\vec{w}(1,0,0)$. a) $\vec{u} \parallel \vec{v}$ ? b) $\vec{u} \parallel \vec{w}$ ?

**Corrigé-type.** a) $\vec{u} \wedge \vec{v} = (0,0,0)$ → $\boxed{\text{oui}}$ ($\vec{v} = 2\vec{u}$). b) $\vec{u} \wedge \vec{w} = (0,3,1) \neq \vec{0}$ → $\boxed{\text{non}}$.
🪤 *Piège testé : proportionnalité à l'œil — le $\wedge$ tranche.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| Q1 | simplifier par $m$ | $m = 0$ possible : garder $(2m,4,2m)$ |
| R1 | 2ᵉ composante : signe | $+,-,+$ puis test |
| R2 | normal opposé « faux » | $-\vec{n}$ = même plan |
| R3 | $\sqrt{3}$ sans $1/2$ | triangle = moitié |
| R4 | proportionnalité à l'œil | $\vec{u} \wedge \vec{v} = \vec{0}$ |

## VRAIE — 2023N Ex1 (espace : A(0,1,4), sphère tangente en D)

🏷️ matière=Math · année=2023 · session=N · chapitre=M12 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
$AB \wedge AC = 4(2i+j+2k)$ → $S_{ABC} = \frac{1}{2}\|\cdot\| = 2\sqrt{9} = 6$ ; $d(B,(AC)) = \|AB\wedge AC\|/\|AC\| = 12/6 = 2$. $D$ milieu $[AC]$ : $D(1,3,2)$, $D\Omega = \frac{1}{4}(AB\wedge AC)$ → $D\Omega \perp (ABC)$ → $d(\Omega,(ABC)) = \|D\Omega\| = 3$. Sphère $x^2+y^2+z^2-6x-8y-8z+32=0$ : centre $\Omega(3,4,4)$, $R = \sqrt{9+16+16-32} = 3$ → $d = R$ : plan tangent en $D$ ! Plans $\parallel (ABC)$ coupant selon cercle $r=\sqrt{5}$ : $d(\Omega,Q) = \sqrt{9-5} = 2$ → $|18+d|/3 = 2$ → $Q_1 : 2x+y+2z-12=0$, $Q_2 : 2x+y+2z-24=0$.
🪤 *vraie : $D\Omega \parallel$ normal → $D$ = projeté (pas de calcul !) ; $d(\Omega,Q)$ via $r^2 = R^2-d^2$.*
