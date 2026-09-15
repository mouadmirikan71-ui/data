---
chapitre: "06 - Nombres complexes (partie 1 : forme algébrique)"
unite: "S2 - Algèbre"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.2 Q1 (réel, SP confirmé) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11), ancré 2020R"
---

# Chapitre 06 — Nombres complexes, partie 1 (forme algébrique)

> 📋 **Exigible au bac** : $i^2 = -1$, forme algébrique $a+ib$, opérations, conjugué, module, plan complexe
> (affixe, distance $|z_A-z_B|$), équations du 2nd degré dans $\mathbb{C}$. (Trigo/Moivre/rotations → ch.08.)

## 1. Accroche — le nombre qui n'existait pas 🌀

**FR :** $x^2+1 = 0$ n'a AUCUNE solution réelle : impossible ! Au XVIe siècle, les mathématiciens ont fait un pari
fou : « et si on INVENTAIT une solution, $i$, avec $i^2 = -1$ ? » Résultat : non seulement ça marche, mais TOUT
devient plus simple — chaque équation a ses solutions, l'électricité s'explique (impédances !), les fractales
naissent. Le complexe n'est pas « compliqué » : c'est un COUPLE $(a,b)$ écrit $a+ib$, un point du plan !
Le national 2020R l'utilise dès Q1 : $z^2-\sqrt{2}z+1 = 0$ → deux solutions conjuguées. Tout le chapitre =
calculer avec $i$ comme avec $x$ (en se souvenant que $i^2 = -1$).

**بالدارجة:** المعادلة $x^2+1 = 0$ ما عندها حتى حل حقيقي — مستحيلة! الرياضيين قالو: «وإلا **اخترعنا** الحل $i$ حيث $i^2 = -1$؟» والنتيجة: كلشي تسهل — أي معادلة ولات عندها حلولها، والكهرباء تفسرات! العدد العقدي ماشي «معقد»: هو **زوج $(a,b)$** مكتوب $a+ib$ — نقطة فالمستوى! الوطني 2020R بدا بيه: $z^2-\sqrt{2}z+1 = 0$ ← جوج حلول مترافقين. هاد الفصل = حسب مع $i$ بحال $x$ (وتفكر $i^2 = -1$)!

## 2. Résumé du cours (exigible au bac)

### 2.1 Forme algébrique & opérations
- $z = a+ib$ ($a = \text{Re}(z)$, $b = \text{Im}(z)$), $i^2 = -1$.
- Égalité : $a+ib = a'+ib' \iff a = a'$ ET $b = b'$. Addition/soustraction : partie par partie.
- Produit : $(a+ib)(c+id) = (ac-bd)+i(ad+bc)$ (distributivité + $i^2 = -1$ !).
- ⚠️ $\text{Re}(z)$, $\text{Im}(z)$ sont des RÉELS (pas de $i$ dedans !).

### 2.2 Conjugué — le miroir
- $\bar{z} = a-ib$ (miroir sur l'axe réel). Propriétés : $\overline{z+z'} = \bar{z}+\bar{z'}$ ;
  $\overline{zz'} = \bar{z}\bar{z'}$ ; $\bar{\bar{z}} = z$ ; $z+\bar{z} = 2\text{Re}(z)$ ; $z-\bar{z} = 2i\text{Im}(z)$.
- $z$ réel $\iff z = \bar{z}$ ; $z$ imaginaire pur $\iff z = -\bar{z}$.

### 2.3 Module — la distance
- $\boxed{|z| = \sqrt{a^2+b^2}}$ (toujours $\ge 0$ !). $\boxed{|z|^2 = z\bar{z}}$ (LA formule — à savoir !).
- $|zz'| = |z||z'|$ ; $|1/z| = 1/|z|$ ; inégalité triangulaire : $|z+z'| \le |z|+|z'|$.
- Inverse : $\boxed{\frac{1}{z} = \frac{\bar{z}}{|z|^2}}$ ($z\ne 0$) — multiplier par le conjugué !

### 2.4 Plan complexe (affixe, géométrie de base)
- $M$ d'affixe $z = a+ib$ : point $(a,b)$. $|\overrightarrow{AB}| = |z_B-z_A|$ (distance !).
- $|z-a| = r$ : cercle de centre $A(a)$ et rayon $r$. $|z-a| = |z-b|$ : médiatrice de $[AB]$.

### 2.5 Équations du 2nd degré dans $\mathbb{C}$
- $az^2+bz+c = 0$ ($a,b,c$ réels), $\Delta = b^2-4ac$ :
  - $\Delta > 0$ : 2 solutions réelles (comme avant). $\Delta = 0$ : 1 solution double.
  - $\boxed{\Delta < 0}$ : 2 solutions COMPLEXES CONJUGUÉES : $\boxed{z = \frac{-b\pm i\sqrt{|\Delta|}}{2a}}$.
- Somme $= -b/a$, produit $= c/a$ (Vieta — vérification !). 2020R : $\Delta = -2$ → $\frac{\sqrt{2}\pm i\sqrt{2}}{2}$.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** العدد العقدي = **نقطة فالمستوى**! الجزء الحقيقي = الإحداثي $x$، والتخيلي = الإحداثي $y$. كل عملية جبرية عندها معنى هندسي!

1. **$i^2 = -1$:** القاعدة الوحيدة الجديدة! الضرب: وزع عادي ومن بعد بدل $i^2$ بـ $-1$. $(2+3i)(1-i) = 2-2i+3i-3i^2 = 5+i$ — شفتي؟ توزيع + تعويض!
2. **المرافق ($\bar{z}$):** المراية على المحور الحقيقي ($a+ib \to a-ib$). الفائدة الذهبية: $z\bar{z} = a^2+b^2$ (**حقيقي**!) ← كيستعمل باش نحيدو $i$ من المقام!
3. **المعيار ($|z|$):** المسافة من الأصل: $\sqrt{a^2+b^2}$ — نظرية فيثاغورس! $|z|^2 = z\bar{z}$ هي الصيغة اللي كتربط الجبر بالهندسة!
4. **المعكوس:** $\frac{1}{a+ib} = \frac{a-ib}{a^2+b^2}$ — ضرب البسط والمقام بالمرافق! اللي كتب $\frac{1}{a}+i\frac{1}{b}$ غلط!
5. **الدرجة الثانية:** $\Delta < 0$ ← جوج حلول مترافقين: $\frac{-b\pm i\sqrt{|\Delta|}}{2a}$! المميز السالب ما بقاش «مستحيل» — بقا «عقدي»!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — $i$ بحال $x$ (مع $i^2 = -1$).** أي حساب: وزع، جمع الحدود المتشابهة، وعوض $i^2$. $i^3 = -i$، $i^4 = 1$، والدورة كتعاود ($i^{4k+r} = i^r$)!

**الخطوة 2 — المرافق سلاح التنظيف.** مقام فيه $i$؟ ضرب بالمرافق! $\frac{1}{2+i} = \frac{2-i}{5} = \frac{2}{5}-\frac{1}{5}i$. هاد الحركة (rendre réel le dénominateur) كتتعاود فكل تمرين!

**الخطوة 3 — المعيار = المسافة.** $|z|$: جذر مربعات الجزأين. $|z_A-z_B|$: المسافة بين النقطتين! $|z-a| = r$: دائرة! الهندسة كتخليك **تشوف** الحل قبل ما تحسبو!

**الخطوة 4 — الدرجة الثانية: $\Delta$ كيقرر.** $\Delta \ge 0$: كيفما موالف. $\Delta < 0$: $\frac{-b\pm i\sqrt{|\Delta|}}{2a}$ — جوج مترافقين! تحقق بـ Vieta (المجموع $-b/a$ والجداء $c/a$)!

**الخطوة 5 — الأخطاء القاتلة:** $|z|^2 = a^2-b^2$ (غلط! زائد!)؛ $\frac{1}{a+ib} = \frac{1}{a}+i\frac{1}{b}$ (كارثة!)؛ $\text{Re}(z)$ فيها $i$ (مستحيل — حقيقي!)؛ $\Delta < 0$ ← «pas de solution» (قديم! دابا عقديين!)؛ نسيان $i$ فـ $\pm i\sqrt{|\Delta|}$!

## 5. Définitions clés (FR + Darija)

| Notion | FR | بالدارجة |
|---|---|---|
| $z = a+ib$ | Forme algébrique ($a,b$ réels) | الشكل الجبري |
| $\bar{z} = a-ib$ | Conjugué (miroir axe réel) | المرافق — المراية |
| $|z| = \sqrt{a^2+b^2}$ | Module = distance à O | المعيار = المسافة |
| $|z|^2 = z\bar{z}$ | Le pont algèbre-géométrie | الجسر بين الجبر والهندسة |
| Affixe | $z_M$ = coordonnées complexes de M | لاحقة النقطة |
| $\Delta < 0$ | 2 solutions conjuguées $\frac{-b\pm i\sqrt{|\Delta|}}{2a}$ | جوج حلول مترافقين |

## 6. FAQ du chapitre

**Q1. $i$, ça « existe » vraiment ?**
$i$ existe comme objet mathématique (couple $(0,1)$ avec une multiplication spéciale), pas comme quantité à compter.
Il « existe » autant que $\sqrt{2}$ (qui a aussi choqué en son temps !) — et il MODÉLISE le réel (électricité !).
بالدارجة: $i$ موجود رياضياً (الزوج $(0,1)$ بضرب خاص) — وكيوصف الواقع (الكهرباء)! بحال $\sqrt{2}$ اللي حتى هو صدم الناس فاللول!

**Q2. Pourquoi $z\bar{z} = |z|^2$ ?**
$(a+ib)(a-ib) = a^2-iab+iab-i^2b^2 = a^2+b^2$ : les $i$ s'annulent, $i^2 = -1$ change le signe. C'est une identité
remarquable $(x+y)(x-y)$ déguisée !
بالدارجة: $(a+ib)(a-ib) = a^2+b^2$ — المتطابقة $(x+y)(x-y)$ متنكرة! الـ $i$ كيتلاشى و$i^2$ كتقلب الإشارة!

**Q3. Comment diviser par $a+ib$ ?**
Multiplier haut et bas par le CONJUGUÉ : $\frac{1}{a+ib} = \frac{a-ib}{a^2+b^2}$. Le dénominateur devient réel.
JAMAIS $\frac{1}{a}+i\frac{1}{b}$ !
بالدارجة: ضرب الفوق والتحت بالمرافق! المقام كيولي حقيقي. وعمرك تكتب $\frac{1}{a}+i\frac{1}{b}$!

**Q4. $\Delta < 0$ : pourquoi $\pm i\sqrt{|\Delta|}$ ?**
$x^2 = \Delta = -|\Delta|$ → $x = \pm\sqrt{-|\Delta|} = \pm i\sqrt{|\Delta|}$ (car $i^2 = -1$ !). Le $i$ « absorbe »
le signe moins. La formule $\frac{-b\pm\ldots}{2a}$ reste LA MÊME qu'en réel !
بالدارجة: $x^2 = -|\Delta|$ ← $x = \pm i\sqrt{|\Delta|}$ (حيت $i^2 = -1$)! الـ $i$ كيمتص السالب! والصيغة نفسها ديال الحقيقي!

**Q5. $|z-a| = r$, c'est quoi géométriquement ?**
L'ensemble des points M à distance $r$ de A : le CERCLE de centre A, rayon $r$ ! Et $|z-a| = |z-b|$ : points
équidistants de A et B = MÉDIATRICE de $[AB]$. Le module PARLE géométrie !
بالدارجة: النقط اللي بعدهم على A هو $r$ = **دائرة**! والمتساوية البعد على A وB = **واسط**! المعيار كيهضر بالهندسة!

**Q6. Et la suite (ch.08) ?**
Forme trigo ($r(\cos\theta+i\sin\theta)$), exponentielle ($re^{i\theta}$), Moivre (puissances !), racines $n$-ièmes,
et transformations (rotations !). P1 = calculer, P2 = tourner !
بالدارجة: الشكل المثلثي والأسي وموافر (القوى!) والتحويلات (الدوران!). الجزء 1 = الحساب، والجزء 2 = الدوران!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : $i^2 = -1$ utilisé explicitement ; dénominateur rendu réel (conjugué) ; $\Delta$ calculé
+ cas discuté ; solutions sous forme $a\pm ib$ ; Vieta en vérification ; $\boxed{\text{résultats}}$.
**Erreurs fréquentes** : $|z|^2 = a^2-b^2$ ❌ ; $1/(a+ib) = 1/a+i/b$ ❌ ; $\text{Re}(z)$ avec $i$ ❌ ;
$\Delta < 0$ → « impossible » ❌ ; $\pm\sqrt{|\Delta|}$ sans $i$ ❌ ; $i^3 = 1$ ($= -i$ !) ❌.

## 8. Sources de ce chapitre
- National Maths SX 2020 Rattrapage Ex.2 Q1 ($z^2-\sqrt{2}z+1 = 0$) — filière SP confirmée (RR 22F).
  https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ + corrigé officiel
  https://www.alloschool.com/element/109814 (barème Q1 : 0.75 pt).
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-15.

## 9. Le « pourquoi » profond — inventer pour résoudre 🔬

**Pourquoi $i^2 = -1$ « marche » ? (l'extension qui préserve les règles)**
On ne « prouve » pas $i$ : on CONSTRUIT $\mathbb{C}$ comme les couples $(a,b)$ avec $+$/$\times$ qui prolongent
celles de $\mathbb{R}$, en posant $i = (0,1)$. Miracle : TOUTES les règles (distributivité, commutativité...)
survivent, et $i^2 = (-1,0) = -1$ ! Moral : les maths avancent en INVENTANT des objets qui respectent les anciennes
règles tout en résolvant les anciens impossibles (comme $\sqrt{2}$, comme $0$, comme les négatifs !).

**Pourquoi le conjugué est partout ? (le $i$-tueur)**
$\bar{z}$ est l'unique opération qui « tue » le $i$ : $z\bar{z} = a^2+b^2\in\mathbb{R}^+$. Diviser par $z$ =
multiplier par $\bar{z}$ puis diviser par un RÉEL. Sans conjugué, pas d'inverse, pas de module, pas de géométrie :
c'est l'outil qui ramène $\mathbb{C}$ vers $\mathbb{R}$ quand on en a besoin (distances, normes, dénominateurs).

**Pourquoi $|z|^2 = z\bar{z}$ est LA formule ? (le dictionnaire algèbre ⟷ géométrie)**
À gauche : de la géométrie (distance au carré, Pythagore). À droite : de l'algèbre (produit). Cette égalité DIT
que le plan complexe EST euclidien : $|z_A-z_B|$ mesure vraiment des distances, les cercles $|z-a| = r$ sont de
vrais cercles. Tout l'Ex.2 du national 2020R (triangle isocèle via $|a-b| = |b-c|$ !) repose sur ce dictionnaire.

**Pourquoi $\Delta < 0$ donne des conjugués ? (la symétrie du réel)**
Coefficients réels ⟹ l'équation est « symétrique » par conjugaison : si $z$ est solution, $\bar{z}$ aussi
(conjugue toute l'équation : les réels ne bougent pas !). Donc les solutions non réelles vont par PAIRES
conjuguées — FORCÉMENT. C'est pour ça que 2020R trouve $\frac{\sqrt{2}}{2}\pm i\frac{\sqrt{2}}{2}$ : le $\pm$
n'est pas un hasard, c'est la symétrie !

**Ponts :** ch.08 (trigo/Moivre/rotations : la SUITE) ; ch.02 (2nd degré, discriminant — le socle) ; trigo
(cercle : prépare les arguments !) ; Physique RLC ch.06 (impédance complexe $Z = R+iX$ — les complexes
PILOTENT l'électricité !) ; SVT (aucun — les complexes sont le seul chapitre purement math-physique !).

> بالدارجة: علاش $i^2 = -1$ خدام؟ حيت بنينا $\mathbb{C}$ كأزواج $(a,b)$ كيحترمو نفس القواعد ديال $\mathbb{R}$ — الرياضيات كتتقدم **بالاختراع اللي كيحترم القواعد**! وعلاش المرافق فكل بلاصة؟ حيت هو اللي **كيقتل $i$** ($z\bar{z}$ حقيقي!) — بلا بيه لا معكوس لا معيار لا هندسة! وعلاش $\Delta < 0$ كيعطي مترافقين؟ حيت المعادلة بمعاملات حقيقية **متناظرة**: إلا $z$ حل، $\bar{z}$ حل بالضرورة! الـ $\pm$ ماشي صدفة — هو التناظر!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $|z|^2 = a^2+b^2$ vs $(a+ib)^2$ — le $+$ qui change tout.**
*Le clic :* $|z|^2 = a^2+b^2$ (TOUJOURS réel positif : Pythagore !) mais $z^2 = (a^2-b^2)+2iab$ (complexe !).
$|z|^2 = z\bar{z}$ (avec le CONJUGUÉ !), PAS $z\times z$. Test : $|i|^2 = 1$ mais $i^2 = -1$ — si tu confonds, $1 = -1$ !
بالدارجة: $|z|^2 = a^2+b^2$ (حقيقي موجب ديماً!) ولكن $z^2 = (a^2-b^2)+2iab$ (عقدي!). اختبر: $|i|^2 = 1$ و$i^2 = -1$ — إلا خلطتي، $1 = -1$!

**C2. $\text{Re}(z)$ et $\text{Im}(z)$ sont RÉELS — pas de $i$ !**
*Le clic :* $z = 3+4i$ : $\text{Re} = 3$, $\text{Im} = 4$ (PAS $4i$ !). « $\text{Im}(z) = 4i$ » est la faute la plus
bête du chapitre — et la plus fréquente. Retiens : Re/Im DÉSHABILLENT $z$ (ils enlèvent le $i$).
بالدارجة: $z = 3+4i$: الحقيقي $= 3$ والتخيلي $= 4$ (**ماشي $4i$**)! أغبى غلطة وأكثرها انتشاراً! Re وIm **كيعريو** العدد (كيحيدو $i$)!

**C3. $\Delta < 0$ : « pas de solution » — le réflexe périmé.**
*Le clic :* en Seconde, $\Delta < 0$ = stop. En Terminale complexe, $\Delta < 0$ = 2 solutions CONJUGUÉES
$\frac{-b\pm i\sqrt{|\Delta|}}{2a}$. Le $i$ devant la racine est OBLIGATOIRE ($\pm\sqrt{|\Delta|}$ seul = réel :
FAUX !). Nouveau réflexe : « $\Delta$ négatif ? Je sors le $i$ ! »
بالدارجة: شحال هادي $\Delta < 0$ = حبس. دابا = جوج حلول مترافقين! والـ $i$ قدام الجذر **إجباري**! المنعكس الجديد: «$\Delta$ سالبة؟ خرج الـ $i$!»

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Second degré (discriminant, Vieta) — le socle de §2.5.
2. Fractions + identités remarquables ($(a+b)(a-b)$ !) — le calcul $z\bar{z}$, $1/z$.
3. Pythagore + distances (plan) — le sens de $|z|$, $|z_A-z_B|$.
4. Trigo de base (cercle) — prépare le ch.08 (arguments).

**Si le calcul complexe bloque — plan B :**
Le mur : expressions emmêlées ($1/(2+i)^2$... **Fallback** : (1) TOUT ramener à $a+ib$ par étapes microscopiques
(une opération par ligne : développe, remplace $i^2$, regroupe) ; (2) dénominateur complexe → conjugué SYSTÉMATIQUE ;
(3) VÉRIFIER par le module : $|résultat|$ doit valoir $|numérateur|/|dénominateur|$ (contrôle gratuit !) ;
(4) si une équation résiste : poser $z = x+iy$ ($x,y$ réels) et identifier parties réelle/imaginaire → 2 équations réelles !
بالدارجة: إلا تعقد الحساب: رجع كلشي لـ $a+ib$ **سطر بسطر** (عملية وحدة فالسطر)! المقام العقدي ← المرافق ديماً! وتحقق بالمعيار (|النتيجة| = |البسط|/|المقام|)! وإلا معادلة حبسات: حط $z = x+iy$ وطابق الجزأين ← جوج معادلات حقيقية!
