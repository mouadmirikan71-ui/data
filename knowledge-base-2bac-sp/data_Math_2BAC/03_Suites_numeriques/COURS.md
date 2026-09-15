---
chapitre: "03 - Suites numériques"
unite: "S1 - Analyse de base"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.1 (suites, réel) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11), ancré 2020R"
---

# Chapitre 03 — Suites numériques

> 📋 **Exigible au bac** : monotonie, suites bornées, limites (théorèmes), $q^n$, suites arithmétiques/géométriques
> + sommes, récurrence, suites récurrentes $u_{n+1} = f(u_n)$ + point fixe, suites adjacentes.

## 1. Accroche — ton épargne est une suite 🏦

**FR :** Tu places 10 000 DH à 2 % par an : année 0 → 10 000 ; année 1 → 10 200 ; année 2 → 10 404... Chaque terme
se calcule depuis le précédent ($u_{n+1} = 1,02\,u_n$) — c'est une SUITE. Questions naturelles : combien dans
20 ans ? ($u_{20} = 10000\times1,02^{20}$ — forme explicite !) Ça plafonne ou ça explose ? (limite !) Tout le
chapitre = décrire l'avenir d'une grandeur qui évolue par étapes : lundi, mardi... $n$, $n+1$...

**بالدارجة:** حطيتي 10 000 درهم بفائدة 2 %: العام 0 ← 10 000، العام 1 ← 10 200، العام 2 ← 10 404... كل حد كيتحسب من اللي قبلو ($u_{n+1} = 1,02u_n$) — هادي هي **المتتالية**! الأسئلة الطبيعية: شحال من بعد 20 عام؟ واش كتستقر ولا كتنفجر؟ هاد الفصل كامل = توقع المستقبل ديال حاجة كتطور خطوة بخطوة!

## 2. Résumé du cours (exigible au bac)

### 2.1 Définitions & modes de génération
- Suite = fonction de $\mathbb{N}$ vers $\mathbb{R}$ : $u_0, u_1, \ldots, u_n, \ldots$
- **Explicite** : $u_n = f(n)$ (ex : $u_n = \frac{4n+1}{2n+1}$ — cf. 2020R !). **Récurrente** : $u_{n+1} = f(u_n)$
  + $u_0$ (ex : $u_{n+1} = \frac{3u_n-8}{2u_n-5}$ — cf. 2020R !).

### 2.2 Monotonie (3 méthodes)
- **Différence** : signe de $u_{n+1}-u_n$ ($> 0$ → croissante).
- **Quotient** (si $u_n > 0$) : comparer $\frac{u_{n+1}}{u_n}$ à 1.
- **Via $f$** : si $u_{n+1} = f(u_n)$ avec $f$ croissante : comparer $u_0, u_1$ puis **récurrence**
  ($u_n \le u_{n+1} \Rightarrow f(u_n) \le f(u_{n+1})$).

### 2.3 Suites bornées
- Majorée ($u_n \le M$), minorée ($u_n \ge m$), **bornée** (= les deux). ⚠️ bornée ⇏ convergente : $(-1)^n$ !

### 2.4 Limites — l'arsenal
- **Opérations** : comme les fonctions (tableau ch.01). **Comparaison** : $u_n \ge v_n\to+\infty \Rightarrow u_n\to+\infty$.
- **Gendarmes** : $v_n \le u_n \le w_n$, $v_n, w_n \to \ell \Rightarrow u_n \to \ell$.
- **$q^n$** : $|q|<1 \to 0$ ; $q = 1 \to 1$ ; $q>1 \to +\infty$ ; $q\le-1$ : PAS de limite (diverge).
- **Monotone bornée** : croissante + majorée ⟹ CONVERGE (vers $\ell \le M$). LE théorème d'existence !
- **Point fixe** : si $u_{n+1} = f(u_n)$, $u_n\to\ell$ et $f$ continue en $\ell$ ⟹ $\boxed{\ell = f(\ell)}$.

### 2.5 Arithmétiques & géométriques (formules cœur)
- Arithmétique ($+r$) : $u_n = u_0+nr$ ; somme : $\boxed{S = \text{nb}\times\frac{1^{er}+dernier}{2}}$.
- Géométrique ($\times q$) : $u_n = u_0q^n$ ; somme : $\boxed{S = a\frac{1-q^{n+1}}{1-q}}$ ($q\ne 1$).
- Somme INFINIE ($|q|<1$) : $\boxed{\frac{a}{1-q}}$ (la limite de $S_n$ !).

### 2.6 Récurrence (le rituel en 3 temps)
1. **Initialisation** : vérifier $P(n_0)$. 2. **Hérédité** : supposer $P(n)$, PROUVER $P(n+1)$.
3. **Conclusion** : « par récurrence, $P(n)$ vraie $\forall n\ge n_0$ ». Sans (1), (2) ne prouve RIEN !

### 2.7 Suites adjacentes (complément)
- $(u_n)$ croissante, $(v_n)$ décroissante, $v_n-u_n\to 0$ ⟹ les deux convergent vers la MÊME limite.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** المتتالية = **فيلم بالصور**: الصورة $n$ كتولد الصورة $n+1$. السؤال: الفيلم كيستقر على مشهد (نهاية) ولا كيهرب للانهاية؟

1. **الصريحة ضد التراجعية:** الصريحة ($u_n = f(n)$) = آلة حاسبة مباشرة (عطيني $n$ نعطيك $u_n$). التراجعية ($u_{n+1} = f(u_n)$) = سلسلة (خاصك اللي قبل باش تحسب اللي من بعد). الوطني كيعطي التراجعية وكيطلب توصّل للصريحة (عبر متتالية مساعدة $v_n$ — تمرين 2020R بالضبط!).
2. **الرتابة:** الفرق ($u_{n+1}-u_n$) هو الطريقة العامة. الخارج ($u_{n+1}/u_n$) للجداءات والأسس. والدالة $f$ للتراجعية مع البرهان بالترجع!
3. **النهايات:** نفس قوانين الدوال + 3 أسلحة جديدة: المقارنة، الشرطة (gendarmes)، و**الرتيبة المحدودة تتقارب** — هادي هي اللي كتثبت الوجود بلا ما تحسب النهاية!
4. **النقطة الثابتة:** إلا $u_{n+1} = f(u_n)$ وتقاربت لـ $\ell$ ← $\ell = f(\ell)$! علاش؟ حيت بجوج الجهات كيمشيو لـ $\ell$ والاتصال كيخلي $f$ تتبع. حل المعادلة = النهاية المرشحة!
5. **الترجع:** الدومينو! (1) طيّح الأولى (initialisation)، (2) برهن أن أي وحدة كتطيّح اللي وراها (hérédité)، (3) النتيجة: كلشي طايح!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — حسب الحدود الأولى ديماً!** $u_0, u_1, u_2, u_3$ بالآلة (مسموحة فالوطني!) ← كتخمن الرتابة والنهاية قبل البرهان. التخمين ماشي الجواب، ولكن كيوجهك!

**الخطوة 2 — رتيبة + محدودة = تقارب (مضمون!).** إلا بغيتي تثبت التقارب بلا حساب النهاية: برهن الرتابة (فرق ولا ترجع) + القيد المناسب (majorée إلا طالعة، minorée إلا هابطة) ← **تقاربت!** هاد الزوج هو الإجابة ديال 80 % ديال أسئلة «montrer que $(u_n)$ converge»!

**الخطوة 3 — التراجعية: المساعدة $v_n$ هي المفتاح.** ملي كيعطيوك $u_{n+1} = f(u_n)$ وكيعرّفو $v_n$ بدلالة $u_n$ ← حسب $v_{n+1}$ بدلالة $v_n$ (غالباً حسابية ولا هندسية!) ← الصيغة الصريحة ديال $v_n$ ← رجّع $u_n$ ← النهاية! تمرين 2020R هو القالب: حفظ المراحل!

**الخطوة 4 — النقطة الثابتة للتحقق.** لقيتي النهاية $\ell$؟ عوّضها فـ $f$: إلا $\ell = f(\ell)$ راه متوافقة! (2020R: $\ell = 2$: $f(2) = (6-8)/(4-5) = 2$ ✔). إلا ما تحققاتش ← غلطة فالحساب!

**الخطوة 5 — الأخطاء القاتلة:** الخلط بين $u_n$ و$S_n$ (الحد ضد المجموع!)؛ «محدودة إذن متقاربة» ($(-1)^n$ كتكذب!)؛ نهاية $q^n$ مع $q \le -1$ (ما كايناش!)؛ الترجع بلا تأسيس (قصر فالهواء!)؛ $v_n$ محسوبة غلط (خطأ جبري = كلشي غالط — تحقق بـ $v_0$!).

## 5. Définitions clés (FR + Darija)

| Notion | FR | بالدارجة |
|---|---|---|
| Suite récurrente | $u_{n+1} = f(u_n)$ + $u_0$ | كل حد من اللي قبلو |
| Croissante | $u_{n+1}-u_n \ge 0$ (ou quotient $\ge 1$) | طالعة |
| Bornée | Majorée ET minorée | محدودة من الفوق والتحت |
| Convergence | $u_n \to \ell$ finie | الاستقرار على عدد |
| Point fixe | $\ell = f(\ell)$ (si $u_{n+1} = f(u_n)\to\ell$) | النقطة اللي ما كتتحركش |
| Récurrence | Initialisation + hérédité + conclusion | الدومينو: الأولى + التسلسل |

## 6. FAQ du chapitre

**Q1. Comment choisir entre différence et quotient pour la monotonie ?**
Différence = méthode universelle. Quotient = quand $u_n$ a des produits/factorielles/puissances ($u_n > 0$ exigé !)
et qu'on compare à 1. Récurrence via $f$ = quand $u_{n+1} = f(u_n)$ avec $f$ monotone.
بالدارجة: الفرق عامة، والخارج للجداءات والأسس ($u_n > 0$ إجباري!)، والترجع للتراجعية مع $f$ رتيبة!

**Q2. Bornée ⟹ convergente ?**
NON ! $(-1)^n$ est bornée ($-1 \le u_n \le 1$) mais diverge (saute sans fin). Il faut monotone + bornée DU BON CÔTÉ.
بالدارجة: لا! $(-1)^n$ محدودة وما كتقاربش (كتنقز)! خاص الرتابة + القيد المناسب!

**Q3. Pourquoi la limite vérifie $\ell = f(\ell)$ ?**
Parce que $u_{n+1}\to\ell$ ET $f(u_n)\to f(\ell)$ (continuité !), et $u_{n+1} = f(u_n)$ : les deux limites sont égales.
C'est le passage à la limite dans une égalité.
بالدارجة: حيت $u_{n+1}$ كتمشي لـ $\ell$ و$f(u_n)$ كتمشي لـ $f(\ell)$ (الاتصال!) وهما متساويين ← $\ell = f(\ell)$!

**Q4. $q^n$ : tous les cas ?**
$|q|<1\to 0$ ; $q = 1\to 1$ ; $q>1\to+\infty$ ; $q\le-1$ : diverge (pas de limite). Le cas $q = -1$ piégeux : $(-1)^n$
saute, pas de limite !
بالدارجة: $|q|<1$ ← صفر، $q>1$ ← لانهاية، $q \le -1$ ← ما كايناش نهاية! $q = -1$ كتنقز وما كتستقرش!

**Q5. La limite peut-elle égaler la borne ?**
OUI ! 2020R : $u_n < 2$ strictement, mais $\lim u_n = 2$. Les inégalités STRICTES deviennent LARGES à la limite.
بالدارجة: إيه! 2020R: $u_n < 2$ ولكن النهاية $= 2$. المتباينات الصارمة كتولي واسعة فالنهاية!

**Q6. Qu'est-ce qu'une suite auxiliaire $v_n$ ?**
Un changement de variable : $v_n$ exprimée en fonction de $u_n$, choisie pour être SIMPLE (arithmétique/géométrique).
On résout $v_n$ (facile), puis on « remonte » à $u_n$. C'est LE pont récurrente → explicite.
بالدارجة: تبديل المتغير: $v_n$ مختارة باش تكون ساهلة (حسابية/هندسية)! حل $v_n$ ومن بعد رجع لـ $u_n$ — هادا هو الجسر من التراجعية للصريحة!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : $u_0$ calculé ; récurrence en 3 temps nommés ; « $(v_n)$ arithmétique/géométrique car… » ;
$v_0$ + formule explicite ; vérification ($n = 0$ redonne $u_0$ !) ; $\boxed{\text{limite}}$.
**Erreurs fréquentes** : $u_n$ vs $S_n$ confondus ❌ ; « bornée donc convergente » ❌ ; $q^n$ avec $q\le-1$ ❌ ;
récurrence sans initialisation ❌ ; point fixe = preuve de convergence ❌ ; exposant $n$ vs $n+1$ dans les sommes ❌.

## 8. Sources de ce chapitre
- National Maths SX 2020 Rattrapage Ex.1 (suites $u_{n+1} = \frac{3u_n-8}{2u_n-5}$, $v_n$ arithmétique) — énoncé +
  corrigé via etude-generale.com (Y. Matioui). Accès : 2026-09-15.
  https://etude-generale.com/examen-national-math-2020-science-physique-corrige/
  ✅ Filière confirmée SP (audit 2026-09-15) : en-tête officiel du corrigé RR 22F = « شعبة العلوم التجريبية »
  (Sciences Expérimentales, SVT + Sciences Physiques) — papier commun PC+SVT ; label « ST » = erreur d'étiquetage.
- Même source : Ex.2 (complexes → Math-06/08), Ex.3 + Problème (études → Math-01/02/05/07/09) — banque pour la suite.
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-15.

## 9. Le « pourquoi » profond — du discret qui devient continu 🔬

**Pourquoi la récurrence prouve pour une INFINITÉ de cas ? (les dominos + l'axiome)**
L'initialisation fait tomber le domino $n_0$ ; l'hérédité prouve que CHAQUE domino fait tomber le suivant.
Résultat : tous tombent — c'est une induction mathématiquement rigoureuse (axiome de Péano : $\mathbb{N}$ est
construit comme ça !). Sans initialisation, l'hérédité prouve « SI $P(n)$ ALORS $P(n+1)$ » dans le vide : une chaîne
sans premier maillon. D'où le rituel 3 temps : ancre (init) + chaîne (hérédité) + conclusion.

**Pourquoi « monotone + bornée ⟹ converge » ? (la complétude de $\mathbb{R}$)**
Une suite croissante majorée monte... mais plafonnée : elle ne peut pas fuir à $+\infty$ (plafond !) ni osciller
(croissante !). Elle est donc « coincée » vers le PLUS PETIT plafond possible (borne sup — qui EXISTE dans
$\mathbb{R}$ : c'est la complétude, admise au bac). Intuition : monter dans une pièce à plafond bas = finir collé
au plafond. C'est un théorème d'EXISTENCE : il garantit $\ell$ sans le calculer (le calcul vient après : explicite,
gendarmes, point fixe...).

**Pourquoi $\ell = f(\ell)$ ? (la continuité fait passer à la limite)**
$u_{n+1} = f(u_n)$ : à gauche, $u_{n+1}\to\ell$ ; à droite, $u_n\to\ell$ donc $f(u_n)\to f(\ell)$ PAR CONTINUITÉ de $f$.
Deux expressions égales à chaque rang → limites égales → $\ell = f(\ell)$. Sans continuité, $f(u_n)$ pourrait
sauter ailleurs ! Et sans convergence PROUVÉE, $\ell$ n'existe pas : le point fixe donne le SUSPECT, jamais le
verdict. (2020R : $(\ell-2)^2 = 0$ → suspect unique $\ell = 2$, verdict confirmé par la forme explicite.)

**Ponts :** ch.01 (limites : opérations, CC, gendarmes — le moteur de calcul) ; ch.02 (variations de $f$ pour
$u_{n+1} = f(u_n)$ ; auxiliaire $g$ ≈ auxiliaire $v_n$ : MÊME philosophie !) ; PC radioactivité ch.03
($N(t)$ continu ≈ suite géométrique discrète : $e^{-\lambda t}$ vs $q^n$) ; info (boucles `for` = suites
récurrentes : $u$ ← $f(u)$ !).

> بالدارجة: علاش الترجع كيثبت لانهاية ديال الحالات؟ حيت: الأولى طايحة + كل وحدة كتطيّح اللي وراها = **كلشي طايح**! (هادشي من بديهيات $\mathbb{N}$!) وعلاش رتيبة+محدودة كتقارب؟ حيت طالعة بسقف = **مآلها ملتصقة بالسقف** (أصغر سقف موجود فـ $\mathbb{R}$)! وعلاش $\ell = f(\ell)$؟ حيت الجهتين كيمشيو للنهاية والاتصال كيخلي $f$ تتبع! النقطة الثابتة = **المشتبه**، والتقارب المبرهن = **الحكم**!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $u_n$ vs $S_n$ vs $n$ — trois objets, trois destins.**
*Le clic :* $n$ = le COMPTEUR (tend vers $+\infty$, toujours) ; $u_n$ = le TERME (peut converger !) ;
$S_n = u_0+\cdots+u_n$ = la SOMME (autre suite !). « $\lim S_n$ » avec la formule de $u_n$ = hors-sujet total.
Test : « de QUOI je prends la limite ? » — nommer l'objet avant de calculer.
بالدارجة: $n$ = العداد (كيمشي للانهاية ديماً)، $u_n$ = الحد (يقدر يستقر!)، $S_n$ = المجموع (متتالية أخرى!). سول راسك «ديالاش هاد النهاية؟» قبل ما تحسب!

**C2. « Bornée donc convergente » — le $(-1)^n$ qui tue.**
*Le clic :* $(-1)^n$ est bornée ($|u_n| = 1$) mais saute $-1, +1, -1, +1\ldots$ sans jamais se fixer : DIVERGE.
Bornée = « reste dans un enclos » ; convergente = « se fixe sur un point ». L'enclos n'oblige pas à se fixer !
Il faut LA MONOTONIE en plus (qui interdit les sauts éternels).
بالدارجة: $(-1)^n$ محدودة وكتنقز بلا توقف! المحدودية = «باقية فالحظيرة»، والتقارب = «مستقرة فالنقطة». الحظيرة ما كتجبرش على الاستقرار — خاص **الرتابة**!

**C3. La limite peut TOUCHER la borne stricte.**
*Le clic :* 2020R : $u_n < 2$ pour tout $n$, mais $\lim = 2$ ! Se rapprocher sans jamais toucher, à la limite on
touche. Règle : les inégalités strictes deviennent LARGES par passage à la limite ($< \to \le$). Celui qui écrit
« $\ell < 2$ donc $\ell\ne 2$, absurde » a TOUT faux (et pourtant $u_n = \frac{4n+1}{2n+1} < 2$ tend bien vers 2 !).
بالدارجة: 2020R: $u_n < 2$ ديماً ولكن النهاية $= 2$! القرب بلا لمس، فالنهاية كيلمس! القاعدة: الصارمة كتولي واسعة فالنهاية ($<$ ← $\le$). اللي قال «مستحيل» غلط وخا $u_n < 2$ صحيحة!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Limites (ch.01) : opérations, FI, CC, $q^n$ continu ($e^x$) — le moteur de calcul des limites de suites.
2. Calcul algébrique : fractions, puissances, identités — $v_{n+1}-v_n$ ne pardonne pas.
3. Variations de fonctions (ch.02) : pour $u_{n+1} = f(u_n)$ (signe, monotonie de $f$).
4. Sommes usuelles : $1+2+\cdots+n$, puissances de 10.

**Si la récurrente bloque — plan B :**
Le mur : $u_{n+1} = f(u_n)$ dont on ne voit ni monotonie ni limite. **Fallback officiel** : (1) calcule
$u_1, u_2, u_3$ (calculette !) → CONJECTURE (croissante ? vers 2 ?) ; (2) si l'énoncé définit $v_n$ : fonce sur
$v_{n+1}-v_n$ ou $v_{n+1}/v_n$ (c'est TOUJOURS arithmétique ou géométrique au national !) ; (3) si rien n'est donné,
tente le point fixe $\ell = f(\ell)$ pour deviner la limite, puis prouve encadrement + monotonie vers elle.
بالدارجة: إلا وحلتي: حسب $u_1, u_2, u_3$ وخمن! وإلا عطاوك $v_n$: حسب الفرق ولا الخارج — **ديماً حسابية ولا هندسية فالوطني**! وإلا والو: خمن النهاية بالنقطة الثابتة ومن بعد برهن بالحصر والرتابة!
