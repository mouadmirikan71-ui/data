---
chapitre: "06 - Nombres complexes (partie 1 : forme algébrique)"
unite: "S2 - Algèbre"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.2 Q1 (réel, SP confirmé) + 3 type-bac + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 1 vraie nationale + 3 type-bac + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 06 (Complexes P1)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **Q1 = VRAIE question** nationale : **2020 Rattrapage Ex.2 Q1 (0.75 pt)** — 2nd degré dans $\mathbb{C}$
> (filière SP confirmée, RR 22F). **R1-R3 = type-bac** (étiquetées). (Trigo/Moivre → ch.08.)
> Sources : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ (sujet SP + corrigé, session 2020R) + https://www.alloschool.com/element/109814 (barème, même papier 2020R).

## Question 1 — VRAIE (2020 R, Ex.2 Q1, 0.75 pt, 2 méthodes !)

🏷️ matière=Math · année=2020 · session=R · chapitre=M6 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Résoudre dans l'ensemble $\mathbb{C}$ des nombres complexes l'équation : $z^2-\sqrt{2}z+1 = 0$. »

**Corrigé — Méthode 1 : discriminant.**
1. $\Delta = (\sqrt{2})^2-4 = -2 < 0$ → 2 solutions conjuguées.
2. $\boxed{z_1 = \frac{\sqrt{2}+i\sqrt{2}}{2}\,,\, z_2 = \frac{\sqrt{2}-i\sqrt{2}}{2}}$.
3. Vérifier (Vieta) : somme $= \sqrt{2}$ ✔, produit $= \frac{2+2}{4} = 1$ ✔.

**Corrigé — Méthode 2 : forme canonique (sans $\Delta$ !).**
1. $z^2-\sqrt{2}z+1 = \left(z-\frac{\sqrt{2}}{2}\right)^2-\frac{1}{2}+1 = \left(z-\frac{\sqrt{2}}{2}\right)^2+\frac{1}{2} = 0$.
2. $\left(z-\frac{\sqrt{2}}{2}\right)^2 = -\frac{1}{2} = \left(i\frac{\sqrt{2}}{2}\right)^2$ → $\boxed{z = \frac{\sqrt{2}}{2}\pm i\frac{\sqrt{2}}{2}}$. ✅
> بالدارجة: جوج طرق! **المميز** ($\Delta = -2$ ← الصيغة مباشرة) ولا **الشكل القانوني** (مربع كامل ← $X^2 = -1/2$ ← $X = \pm i\sqrt{2}/2$)! القانوني أناقة: كيبين منين جا الـ $i$! وتحقق بـ Vieta ديماً (المجموع والجداء)!

## R1 — TYPE-BAC (opérations + inverse + puissances de $i$)

🏷️ matière=Math · année=— · session=— · chapitre=M6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** (a) $(2+3i)(1-i)$ ? (b) $\frac{1}{2+i}$ sous forme $a+ib$ ? (c) $i^{27}$ ?

**Corrigé :**
(a) Distribuer : $2-2i+3i-3i^2 = 2+i+3 = \boxed{5+i}$.
(b) Conjugué : $\frac{1}{2+i} = \frac{2-i}{(2+i)(2-i)} = \frac{2-i}{5} = \boxed{\frac{2}{5}-\frac{1}{5}i}$.
(c) $27 = 4\times 6+3$ → $\boxed{i^{27} = i^3 = -i}$.
> بالدارجة: (a) وزع وعوض $i^2 = -1$! (b) **المقام العقدي ← ضرب بالمرافق** ($5 = 2^2+1^2$)! (c) قسم الأس على 4 والباقي هو اللي كيحكم ($i^0 = 1, i^1 = i, i^2 = -1, i^3 = -i$ — الدورة!).

## R2 — TYPE-BAC (2nd degré : l'autre classique)

🏷️ matière=Math · année=— · session=— · chapitre=M6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Résoudre dans $\mathbb{C}$ : $z^2+2z+5 = 0$.

**Corrigé :**
1. $\Delta = 4-20 = -16 < 0$ → $\boxed{z = \frac{-2\pm i\sqrt{16}}{2} = -1\pm 2i}$.
2. Vérifier : somme $= -2$ ✔, produit $= (-1)^2+2^2 = 5$ ✔.
> بالدارجة: نفس القالب ديال Q1! $\Delta = -16$ ← $\pm i\sqrt{16} = \pm 4i$ ← قسم على 2: $-1\pm 2i$! والتحقق: $(-1)^2+2^2 = 5$ (الجداء = مجموع المربعات للمترافقين — تحقق سريع!).

## R3 — TYPE-BAC (géométrie : cercle + médiatrice)

🏷️ matière=Math · année=— · session=— · chapitre=M6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** (a) Nature de $\{M(z) : |z-(1+i)| = 2\}$ ? (b) Nature de $\{M(z) : |z| = |z-2|\}$ ?

**Corrigé :**
(a) $|z_M-z_A| = 2$ avec $A(1+i)$ : $\boxed{\text{cercle de centre } A(1,1)\text{, rayon } 2}$.
(b) $MA = MB$ avec $O(0)$ et $B(2,0)$ : $\boxed{\text{médiatrice de } [OB]\text{ (droite } x = 1\text{)}}$.
> بالدارجة: المعيار كيهضر هندسة! $|z-a| = r$ = **دائرة** (المركز $a$ والشعاع $r$)! $|z-a| = |z-b|$ = **واسط** (المتساوية البعد)! ترجم كل معادلة معيار لجملة هندسية قبل ما تحسب والو!

## 🪤 Pièges testés par question
- **Q1** : $\Delta < 0$ → « pas de solution » (réflexe périmé !) ❌ ; $\pm\sqrt{2}$ sans $i$ ❌ ; dénominateur $2a = 2$ oublié ❌.
- **R1** : $i^2 = +1$ ❌ ; $1/(2+i) = 1/2+i$ ❌ ; $i^{27} = i^{3} = 1$ ($i^3 = -i$ !) ❌.
- **R2** : $\sqrt{-16} = -4$ ❌ ($\pm 4i$ !) ; solutions non conjuguées (erreur de signe) ❌.
- **R3** : centre lu $(-1,-1)$ ($z-(1+i)$ : centre $+1+i$ !) ❌ ; médiatrice confondue avec le segment ❌ ; $|z|$ lu « $z = 0$ » au lieu de « $M$ variable, $O$ fixe » ❌.

---
*Q1 = nationale verbatim (2020 R, SP confirmé). R1-R3 = entraînement étiqueté. Suite (trigo/Moivre/rotations) : ch.08, questions 2020R Ex.2 Q2-Q5 en banque.*
