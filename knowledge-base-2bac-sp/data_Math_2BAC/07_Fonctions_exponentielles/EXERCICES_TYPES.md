---
chapitre: "07 - Fonctions exponentielles"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.3 Q1 (réel, SP confirmé) + 3 type-bac + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 1 vraie nationale + 3 type-bac + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 07 (Exponentielles)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **Q1 = VRAIE question** nationale : **2020 Rattrapage Ex.3 Q1a-Q1c** ($u'$, tableau, signe de $u$ —
> filière SP confirmée, RR 22F). **R1-R3 = type-bac** (étiquetées).
> Sources : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ (sujet SP + corrigé, session 2020R) + https://www.alloschool.com/element/109814 (barème, même papier 2020R).

## Données 2020R (Ex.3 Q1)
$u(x) = e^x-2x+2-3e^{-x}$ sur $\mathbb{R}$ ($u(0) = 0$).

## Question 1 — VRAIE (2020 R, Ex.3 Q1a+Q1b+Q1c, 1.25 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M7 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncés officiels :** « Montrer que $u'(x) = \frac{(e^x-1)^2+2}{e^x}$ » (0.5) ; « Dresser le tableau de variation
de $u$ (sans calculer de limite) » (0.25) ; « En déduire le signe de $u$ (remarquer $u(0) = 0$) » (0.5).

**Corrigé-type :**
1. $u'(x) = e^x-2+3e^{-x} = e^x-2+\frac{3}{e^x} = \frac{e^{2x}-2e^x+3}{e^x} = \frac{(e^x-1)^2+2}{e^x}$ ✔
   ($e^{2x}-2e^x+1 = (e^x-1)^2$ : forme canonique !).
2. $(e^x-1)^2+2 > 0$ ET $e^x > 0$ → $u' > 0$ → $\boxed{u\text{ strictement croissante sur }\mathbb{R}}$ (tableau sans limites, comme exigé !).
3. Croissante + $u(0) = 0$ → $\boxed{u < 0\text{ sur }]-\infty,0[}$ et $\boxed{u > 0\text{ sur }]0,+\infty[}$.
> بالدارجة: (1) اشتق ($-3e^{-x}$ مشتقتها $+3e^{-x}$ — إشارة $-x$!) ووحد المقام ($e^x$) ← البسط $e^{2x}-2e^x+3 = (e^x-1)^2+2$ (مربع كامل!)! (2) البسط (مربع+2!) والمقام ($e^x$!) موجبين ← **طالعة ديماً**! (3) طالعة + $u(0) = 0$ ← الإشارة باينة! (هاد $u$ هي اللي خدمات فالفصل 9: $v = e^xu$!)

## R1 — TYPE-BAC (l'arsenal limites)

🏷️ matière=Math · année=— · session=— · chapitre=M7 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** (a) $\lim_{x\to+\infty}\frac{e^x}{x^3}$ ? (b) $\lim_{x\to-\infty}xe^x$ ? (c) $\lim_{x\to 0}\frac{e^{2x}-1}{x}$ ?

**Corrigé :**
(a) CC : $e^x$ écrase $x^3$ → $\boxed{+\infty}$.
(b) CC : $e^x$ meurt en $-\infty$ → $\boxed{0}$.
(c) Taux : $\frac{e^{2x}-1}{x} = 2\cdot\frac{e^{2x}-1}{2x}\to 2\times 1 = \boxed{2}$ (dérivée de $e^{2x}$ en 0 !).
> بالدارجة: (a) الأسية ضد $x^3$ فـ $+\infty$ ← **الأسية كتربح**! (b) فـ $-\infty$ الأسية كتموت ($xe^x \to 0$)! (c) **وازن** ($2x$ فوق وتحت!) ← $2\times 1 = 2$! (معدل التغير — نفس حيلة $\sin$!)

## R2 — TYPE-BAC (étude $x^2e^{-x}$)

🏷️ matière=Math · année=— · session=— · chapitre=M7 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** $f(x) = x^2e^{-x}$ sur $\mathbb{R}$. (a) Limites. (b) Variations + extrema.

**Corrigé :**
(a) $\lim_{-\infty}f = +\infty$ ($x^2$ et $e^{-x}$ explosent !) ; $\lim_{+\infty}f = 0$ (CC : $X^2/e^X\to 0$) →
$\boxed{y = 0\text{ asymptote}}$.
(b) $f'(x) = 2xe^{-x}-x^2e^{-x} = xe^{-x}(2-x)$ ; signe $= x(2-x)$ : $-$ sur $]-\infty,0[$, $+$ sur $]0,2[$,
$-$ sur $]2,+\infty[$ → $\boxed{\text{min local } f(0) = 0}$, $\boxed{\text{max } f(2) = 4/e^2}$.
> بالدارجة: (a) فـ $-\infty$: $x^2$ و$e^{-x}$ بجوج كينفجرو ($+\infty$)! فـ $+\infty$: الأسية كتقتل ($X^2/e^X \to 0$ — مقارب أفقي)! (b) عمّل ($xe^{-x}(2-x)$) ← الإشارة = إشارة $x(2-x)$! قعر $f(0) = 0$ وقمة $f(2) = 4/e^2$!

## R3 — TYPE-BAC (équation, 2 méthodes !)
**Énoncé :** Résoudre dans $\mathbb{R}$ : $e^{2x}-3e^x+2 = 0$.

**Corrigé — Méthode 1 : substitution $X = e^x$.**
$X^2-3X+2 = 0$ → $X = 1$ ou $X = 2$ (les deux $> 0$ ✔) → $\boxed{x = 0\text{ ou }x = \ln 2}$.
**Corrigé — Méthode 2 : factorisation directe.**
$e^{2x}-3e^x+2 = (e^x-1)(e^x-2) = 0$ → $e^x = 1$ ou $e^x = 2$ → $\boxed{x = 0\text{ ou }x = \ln 2}$. ✅
> بالدارجة: جوج طرق! **التبديل** ($X = e^x$ ← تربيعية ← $X = 1, 2$ ← $x = 0, \ln 2$!) و**التعميل المباشر** ($(e^x-1)(e^x-2) = 0$)! التعميل أسرع إلا بنتي — والتبديل مضمون ديماً! (بجوج: تحقق $X > 0$!)

## 🪤 Pièges testés par question
- **Q1** : $(-3e^{-x})' = -3e^{-x}$ ($+3e^{-x}$ : dérivée de $-x$ !) ❌ ; $u'$ non factorisée par $1/e^x$ (signe illisible !) ❌ ; tableau AVEC limites (l'énoncé dit SANS !) ❌ ; signe sans $u(0) = 0$ ❌.
- **R1** : (a) FI non résolue par CC ❌ ; (b) $-\infty\times 0 = 0$ sans CC ❌ ; (c) $= 1$ (oublier le facteur 2 !) ❌.
- **R2** : $(e^{-x})' = e^{-x}$ ($-e^{-x}$ !) ❌ ; $f(0) = 0$ « pas un extremum » (min local !) ❌ ; $\lim_{-\infty} = 0$ (c'est $+\infty$ : $e^{-x}$ EXPLOSE !) ❌.
- **R3** : $X\le 0$ accepté ❌ ; $\ln 2$ « simplifié » (c'est la valeur exacte !) ❌ ; factorisation non vérifiée (redévelopper !) ❌.

---
*Q1 = nationale verbatim (2020 R, SP confirmé). R1-R3 = entraînement étiqueté. $u$ réutilisée : $v = e^xu$ (ch.09).*
