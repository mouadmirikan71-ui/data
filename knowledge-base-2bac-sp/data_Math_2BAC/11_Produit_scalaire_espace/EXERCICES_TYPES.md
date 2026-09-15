> **Pointer** : `11_Produit_scalaire_espace` → P4 (2 vraies 2025N Ex.1 + 4 type-bac) → corrigés-types + R2 en 2 méthodes.

# Exercices types — Produit scalaire dans l'espace (M11)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Données 2025N (Ex.1, 3 pts — espace + sphère)

$A(0,0,2)$, $B(2,0,0)$, sphère $S$ centre $O$ rayon $R = 2$ ; $I$ milieu de $[AB]$ ; $M(0,m,0)$, $m \in \mathbb{R}$. Source : etude-generale (2025 Normale SP, énoncés réels ; corrigés-types prof recoupés par calcul).

## Q1 — VRAIE (2025 N, Ex.1 Q1+Q2)

🏷️ matière=Math · année=2025 · session=N · chapitre=M11 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « Équation de $S$ » ; « $A, B \in S$ ? » ; « Intersection du plan $(OAB)$ avec $S$ » ; « $\overrightarrow{OI} \perp \overrightarrow{AB}$ + $d(O,(AB)) = \sqrt{2}$ ».

**Corrigé-type.** $S$ : $(x-0)^2+(y-0)^2+(z-0)^2 = 4$, $\boxed{x^2+y^2+z^2 = 4}$. $A$ : $0+0+4 = 4$ ✓ ; $B$ : $4+0+0 = 4$ ✓ → $\boxed{A, B \in S}$. Plan $(OAB)$ : $O, A, B$ ont $y = 0$ → plan $y = 0$ → $\cap S$ : $x^2+z^2 = 4$, $y = 0$ = **cercle centre $O$ rayon 2** (grand cercle). $I(1,0,1)$ : $\overrightarrow{OI}\cdot\overrightarrow{AB} = (1,0,1)\cdot(2,0,-2) = 2-2 = 0$ → $\boxed{\perp}$ ; $I \in (AB)$ + $OI \perp (AB)$ → $d = OI = \sqrt{1+0+1} = \boxed{\sqrt{2}}$.
🪤 *Piège testé : intersection plan-sphère « deux points » — non, un PLAN coupe une sphère en CERCLE (c'est une DROITE qui donne 0/1/2 points).*

## Q2 — VRAIE (2025 N, Ex.1 Q4 : section plane)

🏷️ matière=Math · année=2025 · session=N · chapitre=M11 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « Le plan $(ABM)$ : $mx+2y+mz-2m = 0$ (voir M12-Q1) coupe $S$ en un cercle de rayon $r$ : montrer $r = \sqrt{2+4/(m^2+2)}$ ; déduire $\sqrt{2} < r \leq 2$ ».

**Corrigé-type.** $d = d(O, P) = \frac{|-2m|}{\sqrt{m^2+4+m^2}} = \frac{2|m|}{\sqrt{2m^2+4}}$. Pythagore : $r^2 = R^2-d^2 = 4-\frac{4m^2}{2m^2+4} = \frac{8+2m^2}{m^2+2}\cdot\frac{1}{1}$… précisément $4 - \frac{2m^2}{m^2+2} = \frac{4m^2+8-2m^2}{m^2+2} = \frac{2m^2+8}{m^2+2} = 2+\frac{4}{m^2+2}$ → $\boxed{r = \sqrt{2+4/(m^2+2)}}$. Or $m^2+2 \geq 2$ → $0 < \frac{4}{m^2+2} \leq 2$ → $2 < r^2 \leq 4$ → $\boxed{\sqrt{2} < r \leq 2}$ ($r = 2 \iff m = 0$ : grand cercle).
🪤 *Piège testé : $r = R - d$ (soustraire au lieu de Pythagore) — $r^2+d^2 = R^2$ : le triangle $\Omega$-projeté-point est RECTANGLE.*

## R1 — TYPE-BAC (normal + point = équation)

🏷️ matière=Math · année=— · session=— · chapitre=M11 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** $P$ : normal $\vec{n}(1,2,-1)$, passe par $A(0,1,3)$. a) Équation ? b) $B(1,0,-1) \in P$ ?

**Corrigé-type.** a) $x+2y-z+d = 0$, $A$ → $d = 1$ → $\boxed{x+2y-z+1 = 0}$. b) $1+0+1+1 = 3 \neq 0$ → $\boxed{B \notin P}$.
🪤 *Piège testé : signe de $d$ — revérifier que $A$ satisfait l'équation finale.*

## R2 — TYPE-BAC (distance point-plan, 2 méthodes !)

**Énoncé.** $P : 2x-y+3z-5 = 0$, $A(1,2,0)$. Calculer $d(A,P)$.

**Corrigé-type — M1 (formule).** $\frac{|2-2+0-5|}{\sqrt{14}} = \boxed{5/\sqrt{14}}$. **M2 (projeté).** Droite $(1+2t,2-t,3t)$ dans $P$ → $t = 5/14$ → $AH = |t|\|\vec{n}\| = \boxed{5/\sqrt{14}}$.
🪤 *Piège testé : $5/14$ ou $-5/\sqrt{14}$ — $|inj|/\|n\|$ : $|~|$ et $\sqrt{}$ obligatoires.*

## R3 — TYPE-BAC (sphère + plan tangent)

🏷️ matière=Math · année=— · session=— · chapitre=M11 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** $S : x^2+y^2+z^2-4x+2y-4 = 0$. a) Centre, rayon ? b) $T(2,-1,3) \in S$ ? Plan tangent en $T$ ?

**Corrigé-type.** a) $(x-2)^2+(y+1)^2+z^2 = 9$ → $\boxed{\Omega(2,-1,0), R = 3}$. b) $0+0+9 = 9$ ✓ ; normal $(0,0,3)$ → $\boxed{z = 3}$ (contrôle : $d = 3 = R$ ✓).
🪤 *Piège testé : centre $(-2,1,0)$ — $(x-2)^2$ donne $+2$.*

## R4 — TYPE-BAC (positions relatives)

🏷️ matière=Math · année=— · session=— · chapitre=M11 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** $P_1 : x+2y-z+1 = 0$, $P_2 : 2x+4y-2z+3 = 0$, $P_3 : y+2z = 0$. a) $P_1$ vs $P_2$ ? b) $P_1$ vs $P_3$ ?

**Corrigé-type.** a) $\vec{n}_2 = 2\vec{n}_1$ → $\parallel$ ; $A(0,1,3) \in P_1$, $\notin P_2$ ($1 \neq 0$) → $\boxed{\text{strictement }\parallel}$. b) $\vec{n}_1\cdot\vec{n}_3 = 0$ → $\boxed{\perp}$.
🪤 *Piège testé : parallélisme lu sur $d$ — il se lit sur les NORMAUX.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| Q1 | plan∩sphère = « 2 points » | plan → CERCLE ; droite → 0/1/2 pts |
| Q2 | $r = R-d$ | Pythagore : $r^2+d^2 = R^2$ |
| R1 | signe de $d$ | revérifier $A$ dans l'équation |
| R2 | $5/14$ | $|inj|/\|n\|$ |
| R3 | centre $(-2,1,0)$ | flipper le signe |
| R4 | $\parallel$ lu sur $d$ | colinéarité des normaux |
