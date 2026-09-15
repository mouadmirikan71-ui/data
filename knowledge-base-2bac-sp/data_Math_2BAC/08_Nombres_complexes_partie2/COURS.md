---
chapitre: "08 - Nombres complexes (partie 2 : trigonométrie, Moivre, transformations)"
unite: "S2 - Algèbre"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.2 Q2-Q5 (réels, SP confirmé) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11), ancré 2020R"
---

# Chapitre 08 — Complexes P2 (trigo, Moivre, transformations)

> 📋 **Exigible au bac** : forme trigo $r(\cos\theta+i\sin\theta)$, argument (mod $2\pi$), forme exponentielle
> $re^{i\theta}$, produit/quotient/puissances, Moivre, racines $n$-ièmes, translation/rotation/homothétie,
> angles via $\arg\frac{c-a}{b-a}$. (P1 algébrique → ch.06.)

## 1. Accroche — multiplier, c'est tourner ! 🎡

**FR :** Prends $b = \cos\frac{\pi}{8}+i\sin\frac{\pi}{8}$ (un point du cercle unité) et multiplie n'importe quel
$z$ par $b$ : $z$ TOURNE de $\pi/8$ autour de l'origine ! C'est exactement la rotation du national 2020R
($z' = bz$, $C \to B \to A$ : deux rotations de $\pi/8$ = $\pi/4$ !). Pourquoi ? Parce que multiplier des complexes
= multiplier les MODULES et ADDITIONNER les ARGUMENTS. La forme $a+ib$ (ch.06) sert à additionner ; la forme
$re^{i\theta}$ sert à multiplier/tourner. Tout le chapitre = passer de « calculer » à « transformer ».

**بالدارجة:** خود $b = \cos\frac{\pi}{8}+i\sin\frac{\pi}{8}$ (نقطة فالدائرة) وضرب أي $z$ فيها: $z$ **كيدور** بـ $\pi/8$ حول الأصل! هادي بالضبط الدوران ديال 2020R ($z' = bz$: $C \to B \to A$ — جوج دورانات $\pi/8$ = $\pi/4$)! علاش؟ حيت ضرب العقديين = ضرب **المعيارين** وجمع **العمدتين**! الشكل $a+ib$ للجمع، والشكل $re^{i\theta}$ للضرب والدوران! هاد الفصل = من «الحساب» لـ «التحويل»!

## 2. Résumé du cours (exigible au bac)

### 2.1 Forme trigonométrique & argument
- $z = r(\cos\theta+i\sin\theta)$, $r = |z| > 0$, $\theta = \arg(z)$ **modulo $2\pi$**.
- Lecture : $\cos\theta = a/r$, $\sin\theta = b/r$ (+ figure : le quadrant tranche !).
- ⚠️ L'argument n'est PAS unique : $\arg(z) = \theta_0 + 2k\pi$. Deux complexes égaux ⟺ mêmes $r$ et $\theta$ mod $2\pi$.

### 2.2 Forme exponentielle — $e^{i\theta} = \cos\theta+i\sin\theta$
- $z = re^{i\theta}$. Mêmes règles que l'exponentielle réelle : $e^{i\theta}e^{i\theta'} = e^{i(\theta+\theta')}$ ;
  $1/e^{i\theta} = e^{-i\theta}$ ; $\overline{e^{i\theta}} = e^{-i\theta}$ ; $|e^{i\theta}| = 1$.
- Produit : modules ×, arguments + : $r_1e^{i\theta_1}\cdot r_2e^{i\theta_2} = r_1r_2e^{i(\theta_1+\theta_2)}$.
- Quotient : modules ÷, arguments −. Puissance : $ (re^{i\theta})^n = r^ne^{in\theta}$.

### 2.3 Moivre (le cas $|z| = 1$)
- $\boxed{(\cos\theta+i\sin\theta)^n = \cos n\theta+i\sin n\theta}$. 2020R : $b^2 = a$ ($2\times\pi/8 = \pi/4$ !),
  $a^{2020} = e^{i505\pi} = -1\in\mathbb{R}$.

### 2.4 Racines $n$-ièmes
- $z^n = a = \rho e^{i\alpha}$ : $\boxed{n}$ solutions : $z_k = \sqrt[n]{\rho}\,e^{i(\alpha+2k\pi)/n}$, $k = 0..n-1$
  (polygone régulier sur le cercle de rayon $\sqrt[n]{\rho}$ !).
- Cas réflexe : $z^n = 1$ : $e^{i2k\pi/n}$. Cubiques : $1, j, j^2$ ($j = e^{i2\pi/3}$, $1+j+j^2 = 0$).

### 2.5 Transformations du plan (écriture complexe)
- Translation de vecteur $\vec{u}(b)$ : $\boxed{z' = z+b}$.
- Rotation de centre $\Omega(\omega)$, angle $\alpha$ : $\boxed{z'-\omega = e^{i\alpha}(z-\omega)}$.
  Cas 2020R ($\Omega = O$, $\alpha = \pi/8$) : $z' = e^{i\pi/8}z = bz$.
- Homothétie de centre $\Omega(\omega)$, rapport $k$ (réel) : $z'-\omega = k(z-\omega)$.
- Nature : reconnaître la transformation depuis $z' = az+b$ ($|a| = 1$ → rotation/translation ; $a$ réel → homothétie).

### 2.6 Angles & triangles (géométrie active)
- $\boxed{(\overrightarrow{AB},\overrightarrow{AC}) = \arg\frac{z_C-z_A}{z_B-z_A}}$ (mod $2\pi$).
- $|a-b| = |b-c|$ ⟹ isocèle en B (2020R Q4a !). Triangle équilatéral direct : $\frac{c-a}{b-a} = e^{\pm i\pi/3}$.
- Alignement : $\frac{d-b}{c-b}\in\mathbb{R}$ (2020R Q5b : $d/b = 2\cos\frac{\pi}{8}\in\mathbb{R}$ ⟹ O, B, D alignés !).

### 2.7 Linéarisation (puissances → cos/sin multiples)
- Euler : $\cos\theta = \frac{e^{i\theta}+e^{-i\theta}}{2}$, $\sin\theta = \frac{e^{i\theta}-e^{-i\theta}}{2i}$. Élever au carré/cube + Moivre → :
- $\boxed{\cos^2\theta = \frac{1+\cos 2\theta}{2}}$ ; $\boxed{\sin^2\theta = \frac{1-\cos 2\theta}{2}}$ ; $\boxed{\sin\theta\cos\theta = \frac{\sin 2\theta}{2}}$.
- $\boxed{\cos^3\theta = \frac{\cos 3\theta+3\cos\theta}{4}}$ ; $\boxed{\sin^3\theta = \frac{3\sin\theta-\sin 3\theta}{4}}$.
- Usage n°1 : PRIMITIVER ($\int\cos^2 = \frac{x}{2}+\frac{\sin 2x}{4}$ — pont M04/M09 !) ; usage n°2 : résoudre $\cos^2 x = a$ (via $\cos 2x$ !).
- ⚠️ $\cos^2\theta \neq \cos\theta^2$ ; et $\cos^2+\sin^2 = 1$ ne linéarise RIEN (c'est l'inverse : replier !).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** الشكل الأسي $re^{i\theta}$ = **الإحداثيات القطبية**! $r$ = البعد، و$\theta$ = الاتجاه. الضرب = تمديد + تدوير!

1. **العمدة:** الزاوية ديال النقطة ($\cos\theta = a/r$، $\sin\theta = b/r$). ماشي وحيدة (+ $2k\pi$)! الربع هو اللي كيحدد القيمة الصحيحة — رسم ديماً!
2. **الأسي:** $e^{i\theta} = \cos\theta+i\sin\theta$ — نفس قواعد الأسي الحقيقي! الجداء: المعيارين يتضربو والعمدتين يتجمعو! الخارج: يتقسمو ويتنقصو! القوة: $r^n$ و$n\theta$!
3. **موافر:** $(\cos\theta+i\sin\theta)^n = \cos n\theta+i\sin n\theta$ — القوة = ضرب الزاوية! 2020R: $b^2 = a$ حيت $2\times\pi/8 = \pi/4$!
4. **الجذور:** $z^n = a$ ← $n$ حلول على مضلع منتظم! $z^3 = 1$: $1, j, j^2$ ($j = e^{i2\pi/3}$)! الهندسة كتعطيك العدد قبل الحساب!
5. **التحويلات:** الإزاحة $z+b$، الدوران $e^{i\alpha}(z-\omega)+\omega$، التحاكي $k(z-\omega)+\omega$! الدوران = ضرب (تدوير!) + إزاحة (تغيير المركز)!
6. **الزوايا:** $(\overrightarrow{AB},\overrightarrow{AC}) = \arg\frac{c-a}{b-a}$! والاستقامة: الخارج **حقيقي**! 2020R Q5: $d/b = 2\cos(\pi/8)$ حقيقي ← مصطفين!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — ارسم قبل ما تحسب!** أي تمرين عقدي-هندسي: حط النقط فالدائرة ($|z| = 1$؟ فين الزاوية؟). 2020R: $C = 1$ (الزاوية 0)، $B$ ($\pi/8$)، $A$ ($\pi/4$) — الرسم كيبين الدوران قبل الصيغ!

**الخطوة 2 — $e^{i\theta}$ للضرب، $a+ib$ للجمع.** قوى وجداءات؟ حول للأسي! مجموع وفروق؟ بقى جبري! اللي حسب $(1+i)^{10}$ بالتوزيع تعذب — بالأسي: $(\sqrt{2}e^{i\pi/4})^{10} = 32e^{i5\pi/2} = 32i$ فسطر!

**الخطوة 3 — الدوران: الصيغة + المعنى.** $z'-\omega = e^{i\alpha}(z-\omega)$: «رجع للمركز ($-\omega$)، دور ($\times e^{i\alpha}$)، رجع ($+\omega$)»! إلا المركز هو الأصل: $z' = e^{i\alpha}z$ مباشرة!

**الخطوة 4 — الزوايا بالخارج.** $(\overrightarrow{AB},\overrightarrow{AC}) = \arg\frac{c-a}{b-a}$ — البسط = الثاني ($AC$)، المقام = الأول ($AB$)! الترتيب كيحدد الإشارة! والمثلث المتساوي الساقين بالمعيارات ($|a-b| = |b-c|$)، والزوايا بالعمد!

**الخطوة 5 — الأخطاء القاتلة:** العمدة بلا $2k\pi$ (ناقصة!)؛ $\arg(z_1z_2)$ محسوب بالجمع بلا تعديل (mod $2\pi$!)؛ الدوران بلا $-\omega$ (دوران حول الأصل بدل $\Omega$!)؛ $|e^{i\theta}| = e^{i\theta}$ (= 1!)؛ $z^3 = 1$ ← حل واحد (3 حلول!)؛ الاستقامة بالخارج **العقدي** (خاصو يكون حقيقي!).

## 5. Définitions clés (FR + Darija)

| Notion | FR | بالدارجة |
|---|---|---|
| $\arg(z)$ mod $2\pi$ | Angle de $z$ (non unique !) | عمدة العدد — الزاوية |
| $re^{i\theta}$ | Forme exponentielle | الشكل الأسي |
| Moivre | $(\cos\theta+i\sin\theta)^n = \cos n\theta+i\sin n\theta$ | القوة = ضرب الزاوية |
| $z'-\omega = e^{i\alpha}(z-\omega)$ | Rotation $(\Omega,\alpha)$ | الدوران |
| $\arg\frac{c-a}{b-a}$ | Angle $(\overrightarrow{AB},\overrightarrow{AC})$ | الزاوية بالخارج |
| $j = e^{i2\pi/3}$ | Racine cubique ($1+j+j^2 = 0$) | الجذر التكعيبي |

## 6. FAQ du chapitre

**Q1. Pourquoi deux formes ($a+ib$ et $re^{i\theta}$) ?**
Parce que chacune a son talent : $a+ib$ pour ADDITIONNER (partie par partie), $re^{i\theta}$ pour MULTIPLIER
(modules ×, angles +). Le champion CONVERTIT selon l'opération !
بالدارجة: حيت كل وحدة وموهبتها: الجبري للجمع، والأسي للضرب! البطل كيحول حسب العملية!

**Q2. L'argument, pourquoi « mod $2\pi$ » ?**
Parce que $\theta$ et $\theta+2\pi$ = MÊME direction (tour complet !). $\arg(z)$ = une famille infinie.
En pratique : donner la valeur principale ($]-\pi,\pi]$) + mentionner $2k\pi$.
بالدارجة: حيت $\theta$ و$\theta+2\pi$ نفس الاتجاه (دورة كاملة)! العمدة عائلة لانهائية — عطي القيمة الرئيسية وزيد $2k\pi$!

**Q3. $e^{i\theta}$, c'est une vraie exponentielle ?**
C'est une EXTENSION (Euler) : elle garde TOUTES les règles ($e^ae^b = e^{a+b}$...) avec $a,b$ imaginaires.
$|e^{i\theta}| = 1$ toujours (cercle unité !). Et $e^{i\pi}+1 = 0$ (la plus belle formule !).
بالدارجة: توسيع (أويلر): نفس القواعد مع أسس تخيلية! والمعيار ديماً 1 (دائرة الوحدة)! و$e^{i\pi}+1 = 0$ أجمل صيغة!

**Q4. Rotation : pourquoi $z'-\omega$ des deux côtés ?**
« Ramener au centre ($z-\omega$), tourner ($\times e^{i\alpha}$), renvoyer ($+\omega$) » ! Sans $-\omega$, tu
tournes autour de O au lieu de $\Omega$. Le $-\omega$/ $+\omega$ = changement de repère déguisé.
بالدارجة: «رجع للمركز، دور، رجع»! بلا $-\omega$ كتدور حول الأصل ماشي $\Omega$! الـ $\pm\omega$ = تبديل المعلم متنكر!

**Q5. Comment prouver un alignement ?**
$\frac{d-b}{c-b}\in\mathbb{R}$ (angle nul ou plat !). 2020R : $d/b = b+\bar{b} = 2\cos\frac{\pi}{8}\in\mathbb{R}$
⟹ O, B, D alignés. Le quotient RÉEL = signature de l'alignement !
بالدارجة: الخارج **حقيقي** = الاستقامة (زاوية معدومة ولا مسطحة)! 2020R: $d/b = 2\cos(\pi/8)$ حقيقي ← مصطفين!

**Q6. Racines $n$-ièmes : pourquoi $n$ solutions ?**
$z^n = \rho e^{i\alpha}$ : $|z| = \sqrt[n]{\rho}$ (unique !) mais $\arg(z) = (\alpha+2k\pi)/n$ : $n$ valeurs
DISTINCTES mod $2\pi$ ($k = 0..n-1$) — polygone régulier ! $k = n$ redonne $k = 0$ (tour complet).
بالدارجة: المعيار وحيد ($\sqrt[n]{\rho}$) ولكن العمدة $n$ قيم مختلفة (مضلع منتظم)! $k = n$ كيرجع لـ $k = 0$!

**Q7. Linéariser : pourquoi et comment retenir ?**
Parce que $\cos^2$/$\sin^2$ ne se primitivent PAS directement ! Euler ($e^{\pm i\theta}$) transforme les puissances en $\cos 2\theta$/$\cos 3\theta$ (primitivables !). Retenir : $\cos^2 = (1+\cos 2\theta)/2$ (PLUS), $\sin^2 = (1-\cos 2\theta)/2$ (MOINS) — le signe suit le co !
بالدارجة: حيت $\cos^2$ ما عندها أصلية مباشرة! أويلر كيحول القوى لـ $\cos 2\theta$ (عندها أصلية!)! حفظ: $\cos^2$ بالزائد و$\sin^2$ بالناقص!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : $|z|$ + $\cos\theta$/$\sin\theta$ + quadrant ; $e^{i\theta}$ avec $\theta$ SIMPLIFIÉE ;
rotation : centre + angle + formule complète ; angle : quotient dans le BON ordre ; alignement : quotient RÉEL ;
$\boxed{\text{résultats}}$.
**Erreurs fréquentes** : $\arg$ sans mod $2\pi$ ❌ ; rotation autour de O au lieu de $\Omega$ ❌ ;
$|e^{i\theta}|\ne 1$ ❌ ; $z^n = 1$ : $n-1$ solutions ❌ ; quotient d'angle inversé (signe !) ❌ ;
$b+\bar{b} = 2b$ ($= 2\text{Re}(b)$ !) ❌ ;
linéarisation : $\cos^2 = (1-\cos 2\theta)/2$ (signe inversé !) ❌ ; $\cos^3$ sans le $/4$ ❌ ; primitiver $\cos^2$ terme à terme sans linéariser ❌.

## 8. Sources de ce chapitre
- National Maths SX 2020 Rattrapage Ex.2 Q2-Q5 (trigo, Moivre, rotation, triangle, alignement) — filière SP
  confirmée (RR 22F). https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ +
  corrigé officiel https://www.alloschool.com/element/109814 (barème : Q2a 0.75, Q2b 0.5, Q3a 0.25, Q3b 0.5,
  Q4a 0.75, Q4b 0.5, Q5a 0.25, Q5b 0.75).
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-15.

## 9. Le « pourquoi » profond — la multiplication géométrique 🔬

**Pourquoi multiplier = tourner + dilater ? (Euler)**
$e^{i\theta} = \cos\theta+i\sin\theta$ : multiplier par $e^{i\theta}$, c'est appliquer la rotation d'angle $\theta$
(démo : $(a+ib)(\cos\theta+i\sin\theta)$ = formule de rotation du plan !). Donc $z_1z_2$ : on tourne $z_1$ de
$\arg(z_2)$ et on dilate de $|z_2|$. La forme $re^{i\theta}$ SÉPARE les deux effets (taille $r$, direction $\theta$)
que $a+ib$ mélange. C'est pour ça que TOUT (puissances, racines, rotations) devient trivial en exponentielle :
on a choisi le BON langage.

**Pourquoi Moivre ? (l'itération de la rotation)**
$z^n$ = « tourner $n$ fois de $\theta$ » = tourner de $n\theta$ (et dilater $r^n$). Moivre n'est PAS une formule à
apprendre : c'est l'ÉVIDENCE « $n$ rotations de $\theta$ = 1 rotation de $n\theta$ » écrite en complexes !
2020R : $b^2 = a$ parce que 2 rotations de $\pi/8$ = 1 rotation de $\pi/4$ — le dessin LE DIT avant le calcul.

**Pourquoi $n$ racines ? (le tour complet partagé)**
$z^n = 1$ : « $n$ rotations identiques = tour complet ($2\pi$) » → chaque rotation $= 2\pi/n$... mais AUSSI
$2\times2\pi/n$ ($n$ fois $= 2$ tours $= 1$ tour mod $2\pi$ !), etc. : $k$ tours partagés en $n$ ($k = 0..n-1$)
→ $n$ angles distincts → $n$ racines en polygone régulier. La géométrie COMPTE les solutions avant l'algèbre !

**Pourquoi $\arg\frac{c-a}{b-a}$ = angle ? (la division annule les tailles)**
$\frac{\overrightarrow{AC}}{\overrightarrow{AB}}$ : quotient de deux vecteurs = (rapport des LONGUEURS) ×
$e^{i(\text{angle entre eux})}$. Prendre $\arg$ = jeter les longueurs, garder l'angle ! Si le quotient est RÉEL :
angle $0$ ou $\pi$ = alignement (2020R Q5b !). Si $|num| = |den|$ : triangle isocèle (2020R Q4a !). Le quotient
complexe EST l'outil « triangle » : module ⟷ côtés, argument ⟷ angles.

**Ponts :** ch.06 (P1 : le calcul — sans lui pas de trigo !) ; trigo (cercle, $\cos/\sin$ remarquables) ;
Physique RLC/ondes (phase = argument ! $e^{i\omega t}$ : TOUTE la physique vibratoire !) ; Maths suites
($u_n = r^ne^{in\theta}$ : spirales discrètes !) ; géométrie classique (les complexes PROUVENT les théorèmes :
Ptolémée, Simson... en bonus).

> بالدارجة: علاش الضرب = تدوير + تمديد؟ حيت $e^{i\theta}$ **هي** الدوران بزاوية $\theta$! الشكل الأسي كيفصل الحجم ($r$) على الاتجاه ($\theta$) اللي الجبري كيخلطهم! وموافر ماشي صيغة للحفظ: هي بديهية «$n$ دورانات = دوران واحد كبير» مكتوبة بالعقديين! وعلاش $n$ جذور؟ «$n$ دورانات متساوية = دورة كاملة» ← كل دوران $= 2\pi/n$ (ولا ضعفها، ولا...)! والخارج العقدي هو أداة المثلثات: المعيار ← الأضلاع، والعمدة ← الزوايا!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $\arg(z_1z_2) = \arg(z_1)+\arg(z_2)$ — modulo $2\pi$ !**
*Le clic :* la somme peut sortir de $]-\pi,\pi]$ : $\arg = 5\pi/4$ ? C'est $5\pi/4-2\pi = -3\pi/4$ (même direction !).
Oublier de RAMENER dans l'intervalle = réponse fausse (ou incomplète). Réflexe : « somme → ramener mod $2\pi$ ».
بالدارجة: المجموع يقدر يخرج من $]-\pi,\pi]$: $5\pi/4$ هي $-3\pi/4$ (نفس الاتجاه)! اللي ما رجعش للفترة غلط! المنعكس: «جمع ← رد mod $2\pi$»!

**C2. Rotation : $z' = e^{i\alpha}z$ vs $z'-\omega = e^{i\alpha}(z-\omega)$ — le centre !**
*Le clic :* $z' = e^{i\alpha}z$ tourne autour de O UNIQUEMENT. Centre $\Omega\ne O$ ? Il faut $-\omega$/ $+\omega$
(aller au centre, tourner, revenir). 2020R a $\Omega = O$ (chanceux !) — mais le national adore $\Omega\ne O$.
Test : « l'image de $\Omega$ doit être $\Omega$ » — vérifie avec TA formule !
بالدارجة: $z' = e^{i\alpha}z$ كتدور حول الأصل **فقط**! مركز آخر؟ خاص $-\omega$/ $+\omega$! اختبر: «صورة $\Omega$ خاصها $\Omega$» — جربها فصيغتك!

**C3. Quotient d'angle : $\frac{c-a}{b-a}$ — l'ordre = le signe !**
*Le clic :* $(\overrightarrow{AB},\overrightarrow{AC}) = \arg\frac{c-a}{b-a}$ : le SECOND vecteur au NUMÉRATEUR.
Inverser = angle OPPOSÉ (signe faux !). Moyen mnémotechnique : « on va de AB vers AC : AC au-dessus ».
2020R Q4b : $(BA,BC) = \arg\frac{1-b}{a-b} = 7\pi/8$ — inversé, on obtient $-7\pi/8$ (FAUX ici !).
بالدارجة: الثاني ($AC$) فالبسط! القلب = الزاوية المعاكسة (إشارة غالطة)! تذكر: «من AB لـ AC: AC الفوق»! 2020R: $(BA,BC) = 7\pi/8$ — المقلوب $-7\pi/8$ غالط!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Complexes P1 (ch.06) : $a+ib$, conjugué, module — le socle absolu.
2. Trigo (cercle + valeurs $\pi/6,\pi/4,\pi/3$) — lire/écrire les arguments.
3. Fractions + puissances — $e^{i\theta}$, Moivre, racines.
4. Géométrie plane (triangles, angles orientés) — le sens des résultats.

**Si la trigo bloque — plan B :**
Le mur : $\arg$ illisible, rotation emmêlée. **Fallback** : (1) TOUT redessiner (cercle unité + points : la figure
donne les angles AVANT le calcul !) ; (2) repasser en $a+ib$ pour tout calcul additif (sommes, milieux...) ;
(3) rotation : vérifier sur UN point connu (l'image de $\Omega$ = $\Omega$ ! de O ?...) ; (4) angle : calculer le
quotient en $a+ib$ PUIS lire l'argument (long mais infaillible).
بالدارجة: إلا وحلتي: عاود الرسم (الدائرة + النقط: الشكل كيعطي الزوايا قبل الحساب)! والجمعيات ردهم $a+ib$! والدوران جربو على نقطة معروفة (صورة $\Omega$ هي $\Omega$)! والزاوية: حسب الخارج جبرياً ومن بعد قرا العمدة (طويل ولكن مضمون)!
