---
chapitre: "03 - Suites numériques"
unite: "S1 - Analyse de base"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.1 (suites, réel) + 1 type-bac + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 vraies nationales + 1 type-bac + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 03 (Suites)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **Q1-Q4 = VRAI exercice national** : **2020 Rattrapage Ex.1 (2 pts)** — suite récurrente homographique +
> auxiliaire arithmétique. **R1 = type-bac** (géométrique). Corrigés étape par étape + 🪤.
> Source : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ — ✅ filière confirmée SP :
> en-tête officiel du corrigé (RR 22F) = « شعبة العلوم التجريبية » (SVT + Sciences Physiques), papier commun PC+SVT.
> Barème officiel Ex.1 : Q1 0.5 pt, Q2a 0.5 pt, Q2b 0.75 pt (0.25 $v_n$ + 0.5 $u_n$), Q2c 0.25 pt.

## Données 2020R (communes à Q1-Q4)
$(u_n)$ définie par $u_0 = 1$ et $u_{n+1} = \frac{3u_n-8}{2u_n-5}$ pour tout $n\in\mathbb{N}$.
On pose $v_n = \frac{u_n-3}{u_n-2}$.

## Question 1 — VRAIE (2020 R, Ex.1 Q1)

🏷️ matière=Math · année=2020 · session=R · chapitre=M3 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Montrer que pour tout $n$ de $\mathbb{N}$, $u_n < 2$. »

**Corrigé-type (récurrence) :**
1. **Initialisation** : $u_0 = 1 < 2$ ✔.
2. **Hérédité** : supposer $u_n < 2$. Alors $2u_n-5 < -1 < 0$ (donc $u_{n+1}$ bien défini !) et :
$$u_{n+1}-2 = \frac{3u_n-8}{2u_n-5}-2 = \frac{-u_n+2}{2u_n-5} = \frac{\overbrace{2-u_n}^{>0}}{\underbrace{2u_n-5}_{<0}} < 0$$
donc $u_{n+1} < 2$ ✔.
3. $\boxed{\forall n\,,\, u_n < 2}$ par récurrence.
> بالدارجة: الترجع الكلاسيكي! الحيلة: حسب $u_{n+1}-2$ وبيّن أنو سالب — البسط موجب ($2-u_n$) والمقام سالب ($2u_n-5$) ← الكسر سالب! ولاحظ: نفس الحساب كيثبت أن المقام ما كيتصفرش (المقام $< 0$ ديماً) ← المتتالية معرّفة مزيان!

## Question 2 — VRAIE (2020 R, Ex.1 Q2a)

🏷️ matière=Math · année=2020 · session=R · chapitre=M3 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Montrer que $(v_n)$ est une suite arithmétique de raison $2$. »

**Corrigé-type :**
$$v_{n+1}-v_n = \frac{u_{n+1}-3}{u_{n+1}-2}-\frac{u_n-3}{u_n-2} = \frac{3u_n-7}{u_n-2}-\frac{u_n-3}{u_n-2} = \frac{2u_n-4}{u_n-2} = \boxed{2}$$
($u_n\ne 2$ grâce à Q1, donc simplification légitime !). $\boxed{(v_n)\text{ arithmétique de raison }2}$.
> بالدارجة: حسب $v_{n+1}-v_n$ وعوّض $u_{n+1}$ بالصيغة — التبسيط كيعطي 2 بالضبط! والقسمة على $(u_n-2)$ مشروعة حيت Q1 قالت $u_n < 2$ (ما كيساويش 2)! شفتي كيفاش الأسئلة مربوطين؟ Q1 كتحمي Q2!

## Question 3 — VRAIE (2020 R, Ex.1 Q2b)

🏷️ matière=Math · année=2020 · session=R · chapitre=M3 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Écrire $v_n$ en fonction de $n$ et en déduire $u_n$ en fonction de $n$. »

**Corrigé-type :**
1. $v_0 = \frac{1-3}{1-2} = 2$ → $\boxed{v_n = 2+2n}$.
2. $v_n = \frac{u_n-3}{u_n-2} \iff v_n(u_n-2) = u_n-3 \iff u_n(v_n-1) = 2v_n-3 \iff u_n = \frac{2v_n-3}{v_n-1}$.
3. Injecter $v_n = 2+2n$ : $\boxed{u_n = \frac{4n+1}{2n+1}}$. (Vérifier : $n = 0 \to 1 = u_0$ ✔ !)
> بالدارجة: $v_0 = 2$ ← $v_n = 2+2n$ (صيغة الحسابية!). ومن بعد **قلب العلاقة**: $v_n(u_n-2) = u_n-3$ ← جمع حدود $u_n$ ← $u_n = \frac{2v_n-3}{v_n-1}$! وتحقق بـ $n=0$: إلا ما عطاتكش $u_0 = 1$ راه غلطتي!

## Question 4 — VRAIE (2020 R, Ex.1 Q2c, 2 méthodes !)

🏷️ matière=Math · année=2020 · session=R · chapitre=M3 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncé officiel :** « Calculer la limite de la suite $(u_n)$. »

**Corrigé — Méthode 1 : forme explicite (rigoureuse).**
$\lim u_n = \lim\frac{4n+1}{2n+1} = \frac{4}{2} = \boxed{2}$ (terme dominant). La forme explicite PROUVE la convergence.
**Corrigé — Méthode 2 : point fixe (vérification).** Si $u_n\to\ell$ ($\ell\ne 5/2$), $f$ continue en $\ell$ :
$\ell = \frac{3\ell-8}{2\ell-5} \iff 2\ell^2-8\ell+8 = 0 \iff (\ell-2)^2 = 0 \iff \boxed{\ell = 2}$. ✅ Cohérent —
mais M2 seule ne prouve pas la convergence (M1 oui !).
> بالدارجة: جوج طرق! **الصريحة** ($\frac{4n+1}{2n+1} \to 2$ — هادي هي البرهان!) و**النقطة الثابتة** ($\ell = f(\ell) \to \ell = 2$ — تحقق!). القاعدة: النقطة الثابتة كتعطي **المرشح**، والصريحة (ولا رتيبة+محدودة) كتثبت **التقارب**. بجوج مع بعض = إجابة كاملة!

## R1 — TYPE-BAC (géométrique : somme + limite infinie)

🏷️ matière=Math · année=— · session=— · chapitre=M3 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** $(w_n)$ géométrique, $w_0 = 3$, raison $q = \frac{1}{2}$. (a) $w_n$ ? (b) $S_n = \sum_{k=0}^{n}w_k$ ?
(c) $\lim S_n$ ?

**Corrigé :**
(a) $\boxed{w_n = 3\left(\frac{1}{2}\right)^n}$.
(b) $\boxed{S_n = 3\frac{1-(1/2)^{n+1}}{1-1/2} = 6\left(1-\left(\frac{1}{2}\right)^{n+1}\right)}$.
(c) $(1/2)^{n+1}\to 0$ → $\boxed{\lim S_n = 6}$ (retrouver : $\frac{a}{1-q} = \frac{3}{1/2} = 6$ ✔).
> بالدارجة: الهندسية: الحد $= u_0q^n$، والمجموع $= a\frac{1-q^{n+1}}{1-q}$ — **الأس $n+1$** ($n+1$ حد من 0 لـ $n$)! والنهاية: $(1/2)^{n+1} \to 0$ ← المجموع اللانهائي $= \frac{a}{1-q} = 6$. تحقق بالصيغة المباشرة!

## 🪤 Pièges testés par question
- **Q1** : hérédité sans initialisation ❌ ; signe du quotient faux (num $> 0$ + dén $< 0$ → $< 0$ !) ❌ ; oublier que le calcul prouve aussi $2u_n-5\ne 0$ (bien-défini) ❌.
- **Q2** : erreur algébrique dans $v_{n+1}$ (tout s'écroule !) — vérifier avec $v_0 = 2$, $v_1 = 4$ ❌ ; simplifier par $(u_n-2)$ sans citer Q1 ❌.
- **Q3** : $v_0$ mal calculé ($= 2$, pas $-2$ !) ❌ ; inversion $v_n \leftrightarrow u_n$ bâclée ❌ ; pas de vérification $u_0 = 1$ ❌.
- **Q4** : limite « devinée » sans forme explicite ni théorème ❌ ; point fixe présenté comme preuve de convergence ❌ ; $\ell = 2$ rejeté car « $u_n < 2$ » (la limite peut ÉGALER la borne !) ❌.
- **R1** : exposant $n$ au lieu de $n+1$ dans $S_n$ ❌ ; $S_n$ confondu avec $u_n$ ❌ ; $\lim S_n = +\infty$ (« somme infinie = infini » — faux si $|q|<1$ !) ❌.

---
*Q1-Q4 = exercice national réel (2020 R, SX). R1 = entraînement étiqueté. Même source : Ex.2 (complexes → Math-06/08), Ex.3 + Problème (études → Math-01/02/05/07, intégrale → Math-09).*
