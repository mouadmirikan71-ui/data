---
chapitre: "09 - Calcul intégral"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.3 Q2-Q4 (réels, SP confirmé) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11), ancré 2020R"
---

# Chapitre 09 — Calcul intégral

> 📋 **Exigible au bac** : intégrale et aire ($\int_a^b f = F(b)-F(a)$), propriétés (linéarité, Chasles,
> positivité, ordre), intégration par parties (IPP), calculs usuels, aires ($f-g$, signe), valeur moyenne.

## 1. Accroche — l'aire sous la courbe, sans compter les carreaux 📐

**FR :** Aire sous $y = x^2$ entre 0 et 2 ? Compter les carreaux ≈ 2,66... mais la valeur EXACTE ?
Newton a trouvé le raccourci magique : l'aire = $F(2)-F(0)$ où $F' = f$ (ici $x^3/3$ → $8/3$ !). L'intégrale =
l'ANTI-dérivée évaluée aux bornes : dériver casse, intégrer reconstruit (l'aire !). Le national 2020R l'utilise :
$W$ primitive de $v$ → $\int_0^2 v = W(2)-W(0) = \frac{1}{2}e^4-\frac{21}{2}$. Tout le chapitre = transformer des
aires en calculs de primitives.

**بالدارجة:** المساحة تحت $y = x^2$ بين 0 و2؟ حساب المربعات ≈ 2,66... ولكن القيمة **المضبوطة**؟ نيوتن لقى الاختصار السحري: المساحة = $F(2)-F(0)$ حيث $F' = f$ (هنا $x^3/3$ ← $8/3$)! التكامل = **عكس الاشتقاق** محسوب فالأطراف: الاشتقاق كيكسر، والتكامل كيبني (المساحة)! الوطني 2020R استعملو: $W$ أصلية ديال $v$ ← $\int_0^2 v = W(2)-W(0)$! هاد الفصل = تحويل المساحات لحسابات الأصليات!

## 2. Résumé du cours (exigible au bac)

### 2.1 Primitive → intégrale (le pont fondamental)
- $F$ primitive de $f$ sur $I$ ⟺ $F' = f$ (il y en a une INFINITÉ : $F+C$ !).
- $\boxed{\int_a^b f(x)\,dx = [F(x)]_a^b = F(b)-F(a)}$ (le $C$ s'élimine !). Sens : aire ALGÉBRIQUE sous la courbe
  (comptée $+$ au-dessus de $Ox$, $-$ en dessous !).

### 2.2 Primitives usuelles (tableau cœur)

| $f$ | $F$ | $f$ | $F$ |
|---|---|---|---|
| $x^n$ ($n\ne-1$) | $\frac{x^{n+1}}{n+1}$ | $\frac{1}{x}$ | $\ln\|x\|$ |
| $e^x$ | $e^x$ | $\frac{1}{x^2}$ | $-\frac{1}{x}$ |
| $\cos x$ | $\sin x$ | $\sin x$ | $-\cos x$ |
| $u'\cdot u^n$ | $\frac{u^{n+1}}{n+1}$ | $\frac{u'}{u}$ | $\ln\|u\|$ |
| $u'e^u$ | $e^u$ | $f(ax+b)$ | $\frac{1}{a}F(ax+b)$ |

### 2.3 Propriétés (l'algèbre des intégrales)
- Linéarité : $\int (f+g) = \int f+\int g$, $\int kf = k\int f$.
- Chasles : $\int_a^b + \int_b^c = \int_a^c$ ; $\int_a^a = 0$ ; $\int_b^a = -\int_a^b$.
- Positivité : $f\ge 0$ sur $[a,b]$ ($a\le b$) ⟹ $\int_a^b f\ge 0$. Ordre : $f\le g$ ⟹ $\int f\le\int g$.
- Inégalité triangulaire : $|\int f|\le\int|f|$.

### 2.4 Intégration par parties — IPP (l'arme des produits)
- $\boxed{\int_a^b u'v = [uv]_a^b-\int_a^b uv'}$ (dériver $v$, primitiver $u'$ !).
- Choix : $v$ = ce qui se SIMPLIFIE en dérivant ($x^n$, $\ln x$ !), $u'$ = ce qui s'intègre ($e^x$, $\sin x$... 2020R :
  $\int_0^2-2xe^x\,dx$ : $v = -2x$ ($v' = -2$ !), $u' = e^x$.

### 2.5 Aires géométriques (le signe !)
- Si $f\ge 0$ : aire $= \int_a^b f$. Si $f\le 0$ : aire $= -\int_a^b f$. Si signe variable : DÉCOUPER (Chasles !)
  aux zéros et additionner les $|\cdot|$ !
- Entre 2 courbes : $\int_a^b|f-g|$ (la borne = intersections !).
- Valeur moyenne : $\mu = \frac{1}{b-a}\int_a^b f$ (hauteur du rectangle de même aire !).

### 2.6 Volumes de révolution (exigible, rare au national 2020-2026)
- La courbe de $f \ge 0$ sur $[a,b]$ tourne autour de $(Ox)$ : chaque tranche en $x$ = DISQUE de rayon $f(x)$, d'aire $\pi[f(x)]^2$.
- $\boxed{V = \pi\int_a^b [f(x)]^2\,dx}$ (unités de volume u.v. !). Méthode : (1) vérifier $f \ge 0$ (sinon $|f|$ : le rayon est positif !) ; (2) développer $[f]^2$ ; (3) primitiver terme à terme ; (4) $\times\pi$ À LA FIN.
- Classique de contrôle : demi-cercle $f(x) = \sqrt{r^2-x^2}$ sur $[-r,r]$ → $V = \pi\int_{-r}^r (r^2-x^2)dx = \boxed{\frac{4}{3}\pi r^3}$ (la sphère !).
- ⚠️ Ne JAMAIS intégrer $f$ puis mettre au carré : $V = \pi\int f^2 \ne \pi\left(\int f\right)^2$ !

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** التكامل = **المساحة بالحساب**! بدل ما تحسب المربعات، قلب على الأصلية ($F' = f$) وحسب $F(b)-F(a)$! الاشتقاق والتكامل عكس بعض (نيوتن)!

1. **الأصلية:** $F$ اللي مشتقتها $f$! كاينين بزاف ($F+C$) ولكن فالتكامل المحدود $C$ كتمشي ($F(b)+C-F(a)-C$)! $\int_a^b f = F(b)-F(a)$ — **الصيغة الأم**!
2. **الجدول:** $x^n \to \frac{x^{n+1}}{n+1}$، $e^x \to e^x$ (ما كتتبدلش!)، $1/x \to \ln|x|$! والحالات الخاصة: $u'u^n$، $u'/u$ (← $\ln$!)، $u'e^u$ (← $e^u$)! و$f(ax+b) \to F(ax+b)/a$ (القسم على $a$ إجباري!)!
3. **الخواص:** الخطية (فرق التكامل!)، شال (قطع وجمع!)، الإيجابية ($f \ge 0$ ← التكامل $\ge 0$)! هادو هما أدوات التلاعب!
4. **التكامل بالأجزاء (IPP):** $\int u'v = [uv]-\int uv'$ — للجداءات ($x\times e^x$، $x\times\ln x$)! القاعدة: $v$ = اللي **كيتبسط** بالاشتقاق ($x$، $\ln x$)! 2020R: $\int-2xe^x$: $v = -2x$ ← $v' = -2$ (ثابت — تبسط!)!
5. **المساحات:** $f$ موجبة ← التكامل مباشرة! سالبة ← **ناقص** التكامل! متغيرة الإشارة ← **قطع** فالأصفار وجمع القيم المطلقة! (التكامل الجبري كيلغي الموجب بالسالب — المساحة ما كتلغيش!)!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — أي تكامل: قلب على الأصلية أولاً!** $F' = f$؟ (جدول + $u'$, $1/a$...) إلا لقيتيها ← $F(b)-F(a)$ وسالات! إلا جداء ($x\cdot e^x$) ← IPP! إلا كسر ($u'/u$) ← $\ln$!

**الخطوة 2 — IPP: الاختيار الصحيح.** $v$ = اللي كيتبسط ($x^n \to$ درجة أقل، $\ln x \to 1/x$)! $u'$ = اللي كيتكامل ساهل ($e^x$, $\sin x$)! إلا خربقتي ($v = e^x$) التكامل كيتعقد بدل ما يتبسط — عاود من اللول!

**الخطوة 3 — الإشارة قبل المساحة!** «احسب المساحة» ← أولاً: إشارة $f$ على $[a,b]$! موجبة ← تكامل! سالبة ← ناقص تكامل! متغيرة ← قطع فالأصفار ($x_0$) + $|\int_a^{x_0}|+|\int_{x_0}^b|$! اللي كامل مباشرة بلا إشارة خسر!

**الخطوة 4 — تحقق بالاشتقاق!** لقيتي $F$؟ اشتقها: إلا عطاتك $f$ راه صحيحة! (2020R: $W' = v$ — التحقق جزء من التمرين!) هاد العادة كتكشف 90 % ديال الأغلاط!

**الخطوة 5 — الأخطاء القاتلة:** $F(b)-F(a)$ معكوسة ($F(a)-F(b)$!)؛ $C$ فالتكامل المحدود (ما كايناش!)؛ IPP باختيار معكوس (تعقيد!)؛ المساحة = التكامل الجبري مع تغير الإشارة (التعويض!)؛ $[uv]$ محسوب فطرف واحد (طرفين!)؛ $1/a$ منسية فـ $f(ax+b)$!

## 5. Définitions clés (FR + Darija)

| Notion | FR | بالدارجة |
|---|---|---|
| Primitive $F' = f$ | Anti-dérivée ($+C$ !) | الأصلية — عكس المشتقة |
| $\int_a^b f = F(b)-F(a)$ | Intégrale = aire algébrique | التكامل = المساحة الجبرية |
| Chasles | $\int_a^b+\int_b^c = \int_a^c$ | التقطيع والجمع |
| IPP : $\int u'v = [uv]-\int uv'$ | Dériver $v$, primitiver $u'$ | بالأجزاء: بسط $v$! |
| Aire $= \int\|f\|$ (découpée) | Géométrique (toujours $\ge 0$ !) | المساحة الحقيقية موجبة! |
| $\mu = \frac{1}{b-a}\int_a^b f$ | Valeur moyenne | القيمة المتوسطة |

## 6. FAQ du chapitre

**Q1. Pourquoi $F(b)-F(a)$ donne l'aire ?**
Parce que $F$ accumule : $F(x)$ = aire de $a$ à $x$ (sa dérivée $= f$ = « débit d'aire » !). Donc aire de $a$ à $b$
$= F(b)-F(a)$ (tout jusqu'à $b$, moins tout jusqu'à $a$). C'est le théorème fondamental (Newton-Leibniz, admis) !
بالدارجة: حيت $F(x)$ = المساحة من $a$ لـ $x$ (المشتقة = «صبيب المساحة»)! المساحة من $a$ لـ $b$ = اللي حتى $b$ ناقص اللي حتى $a$! (مبرهنة نيوتن-لايبنتز!)

**Q2. $+C$ : quand ?**
Primitive GÉNÉRALE ($F+C$) : oui, $C$ obligatoire ! Intégrale DÉFINIE ($\int_a^b$) : NON ($C$ s'élimine) !
« $\int_0^2 x\,dx = [x^2/2+C]_0^2$ » = faute (le $C$ ne doit pas apparaître).
بالدارجة: الأصلية العامة: $C$ إجباري! المحدود: لا ($C$ كتمشي)! اللي كتب $C$ فالمحدود غلط!

**Q3. IPP : comment choisir $u'$ et $v$ ?**
$v$ = ce qui se SIMPLIFIE en dérivant : $x^n$ (degré ↓), $\ln x$ (→ $1/x$ !). $u'$ = le reste intégrable ($e^x$,
$\sin x$... Si après IPP c'est PIRE → mauvais choix, inverser ! (ILATE : Inverse-log, Log, Algébrique, Trigo, Expo —
priorité à $v$ !)
بالدارجة: $v$ = اللي كيتبسط ($x$، $\ln x$)! $u'$ = الباقي اللي كيتكامل! إلا تعقد ← قلب الاختيار! (قاعدة ILATE للأولوية!)

**Q4. Aire ou intégrale : quelle différence ?**
Intégrale = aire ALGÉBRIQUE (signée : $-$ sous $Ox$ !). Aire GÉOMÉTRIQUE = toujours $+$ : découper aux zéros !
$\int_{-\pi}^{\pi}\sin = 0$ mais aire $= 4$ ! Le national adore ce contraste !
بالدارجة: التكامل = مساحة **موقعة** (سالب تحت المحور)! المساحة الحقيقية = موجبة ديماً: قطع فالأصفار! $\int\sin = 0$ ولكن المساحة $= 4$! الوطني كيبغي هاد الفرق!

**Q5. $\int u'/u$ : pourquoi $\ln$ ?**
Parce que $(\ln|u|)' = u'/u$ (dérivée de composée, ch.02 !). Dès que le numérateur = (k ×) la dérivée du
dénominateur → $\ln$ ! $\int_0^1\frac{2x}{x^2+1}dx = [\ln(x^2+1)]_0^1 = \ln 2$.
بالدارجة: حيت $(\ln|u|)' = u'/u$! ملي البسط = مشتقة المقام ← **لوغاريتم**! المنعكس الذهبي للكسور!

**Q6. Volume de révolution : la formule et le piège ?**
$V = \pi\int_a^b [f(x)]^2\,dx$ : on met au CARRÉ d'abord, on intègre ensuite, $\times\pi$ à la fin. Le piège : $\pi\left(\int f\right)^2$ (carré après intégration — FAUX !). Et si $f$ change de signe : $|f|$ (un rayon est positif !).
بالدارجة: الحجم = $\pi$ فالتكامل ديال **المربع**! ربع أولاً، كامل من بعد، ضرب فـ$\pi$ فاللخر! الفخ: التربيع من بعد التكامل (غالط!)، وإلا $f$ كتبدل الإشارة: القيمة المطلقة!

**Q7. Valeur moyenne : c'est quoi physiquement ?**
La hauteur CONSTANTE qui donnerait la même aire (même « effet total ») : vitesse moyenne, tension moyenne...
$\mu = \frac{1}{b-a}\int_a^b f$. (En PC : $v_{moy} = \Delta x/\Delta t$ = moyenne de $v(t)$ !)
بالدارجة: العلو **الثابت** اللي كيعطي نفس المساحة (نفس «الأثر الكلي»): السرعة المتوسطة...! (فالفيزياء: $v_{moy} = \Delta x/\Delta t$!)

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : $F$ nommée + vérifiée ($F' = f$) ; crochets $[F]_a^b$ ; $F(b)-F(a)$ dans L'ORDRE ;
IPP : $u',v$ déclarés + $[uv]$ aux 2 bornes ; signe de $f$ AVANT toute aire ; $\boxed{\text{résultats}}$.
**Erreurs fréquentes** : $F(a)-F(b)$ ❌ ; $C$ dans le défini ❌ ; IPP inversée ❌ ; aire sans découpage ❌ ;
$1/a$ oublié ❌ ; $[uv]$ à une borne ❌ ; $\ln$ sans $|\cdot|$ ❌ ;
volumes : $\pi(\int f)^2$ au lieu de $\pi\int f^2$ ❌ ; $\pi$ oublié ❌ ; $f$ non vérifiée $\ge 0$ ❌ ; unités (u.v.) absentes ❌.

## 8. Sources de ce chapitre
- National Maths SX 2020 Rattrapage Ex.3 Q2-Q4 ($v = e^xu$, $W$ primitive, $\int_0^2v$, minimum $9/2$) —
  filière SP confirmée (RR 22F). https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ +
  corrigé officiel https://www.alloschool.com/element/109814.
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-15.

## 9. Le « pourquoi » profond — dériver ⇄ intégrer 🔬

**Pourquoi $F(b)-F(a)$ = aire ? (l'accumulation)**
Imagine $F(x)$ = « aire accumulée de $a$ à $x$ » : quand $x$ avance de $dx$, l'aire gagne $f(x)\,dx$ (tranche !) →
$F'(x) = f(x)$ : $F$ EST une primitive ! Réciproquement, TOUTE primitive accumule pareil (à $C$ près, qui s'élimine
par différence !). L'intégrale n'est pas « définie » comme $F(b)-F(a)$ par hasard : c'est le THÉORÈME (l'aire
accumulée se dérive en $f$ !). Dériver = « trancher », intégrer = « accumuler les tranches » : inverses naturels !

**Pourquoi IPP ? (la distributivité de la dérivée, à l'envers)**
$(uv)' = u'v+uv'$ → $u'v = (uv)'-uv'$ → $\int u'v = [uv]-\int uv'$ : IPP = la formule du produit LUE À L'ENVERS !
On échange un produit dur ($\int u'v$) contre un produit + un produit FACILE ($\int uv'$) — SI $v$ se simplifie en
dérivant. Sans cette simplification, IPP tourne en rond : le choix $u'$/$v$ EST la méthode (ILATE !).

**Pourquoi découper aux zéros pour les aires ? (l'algébrique compense)**
$\int_a^b f$ compte $+$ au-dessus, $-$ en dessous : une bosse $+5$ et un creux $-5$ donnent $0$ (algébrique !) mais
l'aire GÉOMÉTRIQUE vaut $10$ (deux morceaux de $5$ !). L'intégrale mesure un BILAN (comme un compte bancaire :
+5-5 = 0 !), l'aire mesure une SURFACE (toujours $+$ !). D'où Chasles + $|\cdot|$ : on convertit le bilan en surface.

**Ponts :** ch.02 (dérivées : VÉRIFIER $F$ en dérivant ! $u'/u$, $u'e^u$ : les formes à reconnaître !) ; ch.04
(primitives : le chapitre jumeau — ici on les ÉVALUE !) ; ch.05/07 (ln/exp : les $F$ usuelles !) ; PC cinématique
($x = \int v$, $v = \int a$ : TOUTE la méca ch.08-10 !) ; PC RC/RL ($q = \int i$ !) ; proba ch.14 (densités :
$P = \int f$ !).

> بالدارجة: علاش $F(b)-F(a)$ = المساحة؟ حيت $F(x)$ = «المساحة المتراكمة» (المشتقة = $f$ = «صبيب المساحة»)! والمساحة من $a$ لـ $b$ = المتراكم حتى $b$ ناقص حتى $a$! الاشتقاق = «التقطيع»، والتكامل = «تجميع الشرائح» — عكس طبيعي! وIPP = صيغة الجداء **مقروءة بالمقلوب** ($(uv)' = u'v+uv'$)! وعلاش التقطيع فالأصفار؟ حيت التكامل **حصيلة** (+5-5 = 0!) والمساحة **سطح** (10!) — شال + القيمة المطلقة كيحولو الحصيلة لسطح!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $\int_{-\pi}^{\pi}\sin = 0$ vs aire $= 4$ — le bilan n'est pas la surface.**
*Le clic :* l'intégrale COMPENSE (bosse $+2$, creux $-2$ : bilan $0$ !) mais l'aire ADDITIONNE ($2+2 = 4$ !).
Question « calculer $\int$ » → bilan (Chasles inutile). Question « aire » → découper + $|\cdot|$ ! Lire le VERBE !
بالدارجة: التكامل **كيعوض** (+2-2 = 0!) ولكن المساحة **كتجمع** (2+2 = 4)! «احسب التكامل» ← حصيلة! «احسب المساحة» ← قطع + قيمة مطلقة! قرا الفعل!

**C2. IPP : $u' = x$, $v = e^x$ — le choix qui empire.**
*Le clic :* $\int xe^x$ : $v = x$ ($v' = 1$ : SIMPLIFIÉ !) + $u' = e^x$ ✔. Inversé ($u' = x$, $v = e^x$) : $\int\frac{x^2}{2}e^x$ :
PIRE ! Règle ILATE ($v$ prioritaire : Log > Algébrique > Trigo > Expo) : $x$ (algébrique) bat $e^x$ (expo) pour $v$.
بالدارجة: $\int xe^x$: $v = x$ (كيتبسط!) + $u' = e^x$! المقلوب كيعطي $\int x^2e^x$ — **أسوأ**! قاعدة ILATE ($v$ بالأولوية)! إلا تعقد ← قلب!

**C3. $[uv]_a^b$ à moitié — le crochet borgne.**
*Le clic :* $[uv]_a^b = u(b)v(b)-u(a)v(a)$ : DEUX bornes ! Écrire $[uv]_a^b = u(b)v(b)$ (oublier $a$) = la moitié des
points envolée. Pire : $u(a)v(a)$ est souvent NON nul (2020R : $[−2xe^x]_0^2 = -4e^2-0$ : le $0$ se calcule, il ne
se devine pas !). Les deux bornes, TOUJOURS.
بالدارجة: $[uv]_a^b = u(b)v(b)-u(a)v(a)$: **جوج أطراف**! اللي كتب غير $b$ طير نص النقط! والطرف $a$ غالباً ماشي صفر — **حسبو** ما تخمنوش!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Dérivées (ch.02) : $u^n$, $e^u$, $\ln u$, $u'v+uv'$ — reconnaître ET vérifier !
2. Primitives usuelles (tableau §2.2 par cœur !) — sans lui, rien ne démarre.
3. Limites (ch.01) : $\ln$, $e^x$ aux bornes (les $F(b)$ à évaluer !).
4. Équations/inéquations : zéros de $f$ (découpage des aires !).

**Si l'intégrale bloque — plan B :**
Le mur : $F$ introuvable (ni tableau, ni IPP évidente). **Fallback** : (1) DÉRIVER pour deviner : si l'énoncé DONNE
$W$ (2020R !), VÉRIFIER $W' = v$ (toujours faisable : c'est le ch.02 !) puis $W(b)-W(a)$ ; (2) produit $x^ne^x$ ou
$x^n\ln x$ → IPP répétée ($n$ fois : degré ↓↓) ; (3) fraction : tenter $u'/u$ (dériver le dénominateur !) ; (4) si
vraiment bloqué : écrire Chasles/linéarité + ce qu'on sait (points partiels : le national note les étapes !).
بالدارجة: إلا ما لقيتيش $F$: إلا عطاوك $W$ ← **تحقق** ($W' = v$ — الفصل 2!) ومن بعد $W(b)-W(a)$! الجداءات ← IPP مكررة! الكسور ← جرب $u'/u$ (اشتق المقام)! وإلا بقات حابسة: كتب شال والخطية واللي عرفتي (التنقيط على المراحل)!
