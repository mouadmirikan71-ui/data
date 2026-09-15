---
chapitre: "09 - Calcul intégral"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.3 Q2-Q4 (réels, SP confirmé) + 1 type-bac + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 vraies nationales + 1 type-bac + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 09 (Intégrales)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **Q1-Q4 = VRAIES questions** nationales : **2020 Rattrapage Ex.3 Q2-Q4** ($v = e^xu$, primitive $W$,
> $\int_0^2v$, minimum — filière SP confirmée, RR 22F). **R1 = type-bac** (aire avec signe).
> Sources : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ (sujet SP + corrigé, session 2020R) + https://www.alloschool.com/element/109814 (barème, même papier 2020R).

## Données 2020R (Ex.3 — admis de Q1/étude de $u$)
$u(x) = e^x-2x+2-3e^{-x}$ ; $u'(x) = \frac{(e^x-1)^2+2}{e^x} > 0$ ; $u$ strictement croissante, $u(0) = 0$ ;
donc $u < 0$ sur $]-\infty,0[$, $u > 0$ sur $]0,+\infty[$. (Étude complète → ch.07.)
$v(x) = e^{2x}-2xe^x+2e^x-3$ ; $W(x) = \frac{1}{2}e^{2x}+(4-2x)e^x-3x$.

## Question 1 — VRAIE (2020 R, Ex.3 Q2a+Q2b, 1 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M9 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncés officiels :** « Vérifier que pour tout $x$, $v(x) = e^xu(x)$ » (0.5) ; « En déduire le signe de $v$ » (0.5).

**Corrigé-type :**
1. $e^xu(x) = e^x(e^x-2x+2-3e^{-x}) = e^{2x}-2xe^x+2e^x-3 = \boxed{v(x)}$ ✔.
2. $e^x > 0$ toujours → signe$(v)$ = signe$(u)$ : $\boxed{v < 0\text{ sur }]-\infty,0[}$, $\boxed{v > 0\text{ sur }]0,+\infty[}$, $v(0) = 0$.
> بالدارجة: وزع $e^x$ على $u$ — كتخرج $v$ بالضبط! ومن بعد: $e^x$ موجبة ديماً ← إشارة $v$ = إشارة $u$ (اللي درستيها فـ Q1)! السؤال كيبني على اللي قبلو — **استعمل النتائج السابقة**!

## Question 2 — VRAIE (2020 R, Ex.3 Q3a, 0.5 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M9 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Montrer que $W$ définie par $W(x) = \frac{1}{2}e^{2x}+(4-2x)e^x-3x$ est une primitive de $v$. »

**Corrigé-type :**
$W'(x) = e^{2x}+(-2)e^x+(4-2x)e^x-3 = e^{2x}+(2-2x)e^x-3 = e^{2x}-2xe^x+2e^x-3 = \boxed{v(x)}$ ✔.
Donc $W$ est UNE primitive de $v$ (à $C$ près — inutile ici !).
> بالدارجة: عطاوك $W$ — **اشتق وتحقق**! ($u'v+uv'$ للحد الأوسط!) إلا خرجات $v$ راه أصلية! هاد السؤال هدية (الفصل 2!) — واللي حاول يلقى $W$ من راسو ضيع الوقت!

## Question 3 — VRAIE (2020 R, Ex.3 Q3b, 0.5 pt, 2 méthodes !)

🏷️ matière=Math · année=2020 · session=R · chapitre=M9 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Calculer l'intégrale $\int_0^2 v(x)\,dx$. »

**Corrigé — Méthode 1 : via $W$ (donnée !).**
$\int_0^2v = W(2)-W(0) = \left(\frac{1}{2}e^4-6\right)-\left(\frac{1}{2}+4\right) = \boxed{\frac{1}{2}e^4-\frac{21}{2}}$
($\approx 16,8$). ($W(0) = \frac{1}{2}+4 = \frac{9}{2}$ — resservira en Q4 !)
**Corrigé — Méthode 2 : IPP directe (sans $W$ !).**
$\int_0^2e^{2x} = \frac{e^4-1}{2}$ ; $\int_0^2-2xe^x\overset{IPP}{=}[-2xe^x]_0^2+\int_0^22e^x = -4e^2+(2e^2-2)$ ;
$\int_0^22e^x = 2e^2-2$ ; $\int_0^2-3 = -6$. Total : $\frac{e^4-1}{2}-2e^2-2+2e^2-2-6 = \frac{e^4-1}{2}-10 = \boxed{\frac{1}{2}e^4-\frac{21}{2}}$. ✅
> بالدارجة: جوج طرق! **$W$ المعطاة** ($W(2)-W(0)$ — سريعة، استعمل الهدية!) و**IPP المباشرة** (حد بحد: $e^{2x}$ مباشر، $-2xe^x$ بالأجزاء $v = -2x$!) — بجوج عطاو $\frac{1}{2}e^4-\frac{21}{2}$! M1 للذكاء (استغلال المعطيات)، M2 للقوة (تقنية خالصة)!

## Question 4 — VRAIE (2020 R, Ex.3 Q3c, 0.75 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M9 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Montrer que $\frac{9}{2}$ est le minimum absolu de $W$ sur $\mathbb{R}$. »

**Corrigé-type :**
1. $W' = v$ (Q2 !) ; signe$(v)$ = signe$(u)$ (Q1 !) : $W$ décroît sur $]-\infty,0]$, croît sur $[0,+\infty[$.
2. Minimum absolu en $0$ : $W(0) = \frac{1}{2}+4-0 = \boxed{\frac{9}{2}}$ ✔.
> بالدارجة: السلسلة الكاملة: $W' = v$ (Q2!) وإشارة $v$ (Q1!) ← $W$ هابطة من بعد طالعة ← **القعر فـ $0$** ← $W(0) = 9/2$! التمرين كامل مربوط: Q1 ← Q2 ← Q3 ← Q4! اللي حل كل سؤال بوحدو ضيع الخيط!

## R1 — TYPE-BAC (aire avec changement de signe)

🏷️ matière=Math · année=— · session=— · chapitre=M9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Aire entre la courbe de $f(x) = x^2-1$ et $Ox$ sur $[-1,2]$ ?

**Corrigé :**
1. Signe : $f\le 0$ sur $[-1,1]$, $f\ge 0$ sur $[1,2]$ → DÉCOUPER en $1$ !
2. $A = -\int_{-1}^1(x^2-1)dx+\int_1^2(x^2-1)dx = -\left[\frac{x^3}{3}-x\right]_{-1}^1+\left[\frac{x^3}{3}-x\right]_1^2$
$= -(-\frac{4}{3})+\frac{4}{3} = \boxed{\frac{8}{3}}$ (unités d'aire).
($\int_{-1}^2$ direct $= 0$ : le bilan compense — PAS l'aire !)
> بالدارجة: الإشارة أولاً: سالبة $[-1,1]$ وموجبة $[1,2]$ ← **قطع فـ $1$**! المساحة $= \frac{4}{3}+\frac{4}{3} = \frac{8}{3}$! والتكامل المباشر $= 0$ (الحصيلة!) — **ماشي المساحة**! هاد الفرق (0 ضد 8/3) هو أشهر فخ فالتكامل!

## R2 — ENTRAÎNEMENT (volume : la sphère retrouvée)

🏷️ matière=Math · année=— · session=— · chapitre=M9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★ · barème=—

**Énoncé :** En tournant autour de $(Ox)$, le demi-disque $y = \sqrt{4-x^2}$ ($-2 \le x \le 2$) engendre une boule de rayon $2$. Retrouver son volume par le calcul intégral.
**Corrigé :**
1. $f \ge 0$ ✔ (racine !). $V = \pi\int_{-2}^{2}(\sqrt{4-x^2})^2\,dx = \pi\int_{-2}^{2}(4-x^2)\,dx$.
2. $V = \pi\left[4x-\frac{x^3}{3}\right]_{-2}^{2} = \pi\left[\left(8-\frac{8}{3}\right)-\left(-8+\frac{8}{3}\right)\right] = \pi\cdot\frac{32}{3} = \boxed{\frac{32\pi}{3}\text{ u.v.}}$
3. Contrôle : $\frac{4}{3}\pi r^3 = \frac{4}{3}\pi\cdot 8 = \frac{32\pi}{3}$ ✔ (la formule de la sphère !).
> بالدارجة: نصف القرص كيدور ← كرة! $V = \pi\int(4-x^2)$ ($(\sqrt{\cdot})^2$ كتحيد الجذر — هدية!) ← $[4x-x^3/3]_{-2}^{2}$ ← $\frac{32\pi}{3}$! والتحقق: $\frac{4}{3}\pi r^3$ ($r = 2$) نفس النتيجة — الصيغة خدامة!

## R3 — ENTRAÎNEMENT (volume style national : $e^x$ + contrôle)

🏷️ matière=Math · année=— · session=— · chapitre=M9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★★ · barème=—

**Énoncé :** $f(x) = e^x$ sur $[0,1]$. (a) Volume $V$ engendré par rotation de $C_f$ autour de $(Ox)$. (b) On admet $V' = \pi(e-1)$ = volume du « tronc » sous la tangente en $0$ ($y = x+1$). Comparer $V$ et $V'$ : lequel est le plus grand ? Justifier sans calculer $V'$.
**Corrigé :** (a) $V = \pi\int_0^1 e^{2x}\,dx = \pi\left[\frac{e^{2x}}{2}\right]_0^1 = \boxed{\frac{\pi}{2}(e^2-1)\text{ u.v.}}$ ($\approx 10,0$). (b) Sur $[0,1]$ : $e^x \ge x+1$ (convexité : courbe au-dessus de sa tangente !) → $[f]^2 \ge (x+1)^2$ → en intégrant : $\boxed{V \ge V'}$ (ordre + positivité, §2.3 !).
> بالدارجة: $V = \pi\int e^{2x} = \frac{\pi}{2}(e^2-1)$ ($e^{2x}$ أصلية $e^{2x}/2$ — القسم على 2 إجباري!)! والمقارنة بلا حساب: $e^x \ge x+1$ (التحدب: المنحنى فوق المماس!) ← المربع كيحفظ الترتيب (موجبين!) ← التكامل كيحفظو ← $V \ge V'$! الوطني كيبغي هاد الربط (تكامل + ترتيب)!

> ⚠️ Volumes : **aucune VRAIE identifiée** (sessions 2020–2026 Tier A : 0 occurrence ; recueils Fayssal/scribd non lisibles en texte). R2/R3 = entraînement pur. Si un volume tombe au national, signaler pour upgrade en VRAIE.

## 🪤 Pièges testés par question
- **Q1** : $e^x\cdot(-3e^{-x}) = -3e^{-2x}$ ($= -3$ !) ❌ ; signe de $v$ sans citer $e^x > 0$ ni Q1 ❌.
- **Q2** : dérivée de $(4-2x)e^x$ sans $u'v+uv'$ ❌ ; « $W$ est LA primitive » (UNE primitive, $+C$ !) ❌.
- **Q3** : $W(0)-W(2)$ (ordre !) ❌ ; $W(0) = \frac{1}{2}$ (oublier $+4$ !) ❌ ; IPP avec $v = e^x$ (empire !) ❌.
- **Q4** : minimum « en $9/2$ » (c'est $W(0) = 9/2$, minimum EN $0$ !) ❌ ; variations sans Q1+Q2 ❌ ; « minimum local » (ABSOLU : monotone de chaque côté sur $\mathbb{R}$ !) ❌.
- **R1** : $\int_{-1}^2 = 0$ présenté comme l'aire ❌ ; découpage au mauvais point ❌ ; unités d'aire oubliées ❌.
- **R2** : $(\sqrt{4-x^2})^2$ « simplifié » en $\sqrt{(4-x^2)^2}$ (tourner en rond !) ❌ ; bornes $0$ à $2$ (demi-volume !) ❌ ; $\pi$ oublié ❌.
- **R3** : primitive de $e^{2x}$ = $e^{2x}$ (oublier $/2$ !) ❌ ; comparaison par calcul décimal sans justification ❌ ; ordre inversé ($e^x \le x+1$ !) ❌.

---
*Q1-Q4 = exercice national réel (2020 R, Ex.3, SP confirmé). R1 = entraînement étiqueté. Ex.3 Q1 (étude de $u$) → ch.07 (exp).*
