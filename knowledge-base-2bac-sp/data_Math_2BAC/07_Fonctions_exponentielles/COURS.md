---
chapitre: "07 - Fonctions exponentielles"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.3 Q1 (réel, SP confirmé) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11), ancré 2020R"
---

# Chapitre 07 — Fonctions exponentielles

> 📋 **Exigible au bac** : $\exp$ (réciproque de $\ln$), $e\approx 2,718$, propriétés algébriques, $(e^u)' = u'e^u$,
> limites + croissances comparées, études ($e^x\ge x+1$), équations ($X = e^x$), $a^x = e^{x\ln a}$.

## 1. Accroche — le nénuphar qui double 🪷

**FR :** Un nénuphar double chaque jour et couvre l'étang en 30 jours. Quand couvrait-il la MOITIÉ ? Jour 29 !
(Doubler : $2^{29}$ → $2^{30}$.) C'est l'exponentielle : croissance PROPORTIONNELLE à la taille ($y' = y$ !) —
lente puis EXPLOSIVE. Bactéries, intérêts composés, radioactivité inverse, charge RC... partout où « plus c'est
grand, plus ça grandit vite », il y a $e^x$. Le national 2020R l'étudie : $u(x) = e^x-2x+2-3e^{-x}$
($u' = \frac{(e^x-1)^2+2}{e^x} > 0$ : toujours croissante !). Tout le chapitre = dompter la plus puissante des fonctions.

**بالدارجة:** زنبقة الماء كتضاعف كل نهار وكتغطي البركة فـ 30 يوم. فوقاش كانت مغطية **النص**؟ النهار 29! (المضاعفة: $2^{29}$ ← $2^{30}$!) هادي هي الأسية: نمو **متناسب** مع الحجم ($y' = y$!) — بطيء من بعد **متفجر**! البكتيريا، الفوائد المركبة، شحن RC... فينما «كبرات كبرات بسرعة» كاينة $e^x$! الوطني 2020R درسها: $u(x) = e^x-2x+2-3e^{-x}$ (طالعة ديماً)! هاد الفصل = روض أقوى دالة!

## 2. Résumé du cours (exigible au bac)

### 2.1 Définition & nombre $e$
- $\exp$ = réciproque de $\ln$ : $y = e^x \iff x = \ln y$ ($y > 0$). $e = \exp(1)\approx 2,718$.
- $e^0 = 1$, $e^1 = e$, $e^x > 0$ TOUJOURS (le ($-\infty$, $+\infty$) → ($0$, $+\infty$) !).

### 2.2 Propriétés algébriques (les mêmes que les puissances !)
- $e^{a+b} = e^ae^b$ ; $e^{-a} = 1/e^a$ ; $e^{a-b} = e^a/e^b$ ; $(e^a)^b = e^{ab}$.
- $e^a = e^b \iff a = b$ ; $e^a < e^b \iff a < b$ (stricte croissance !).

### 2.3 Dérivée & sens
- $\boxed{(e^x)' = e^x}$ (l'unique fonction égale à sa dérivée avec $f(0) = 1$ !) ; $\boxed{(e^u)' = u'e^u}$.
- $e^x > 0$ ⟹ $e^x$ STRICTEMENT CROISSANTE sur $\mathbb{R}$ (et convexe : $(e^x)'' = e^x > 0$ !).

### 2.4 Limites & croissances comparées (l'arsenal)
- $\lim_{-\infty}e^x = 0^+$ (asymptote $y = 0$ !) ; $\lim_{+\infty}e^x = +\infty$ ; $\lim_{x\to 0}\frac{e^x-1}{x} = 1$.
- $\boxed{\lim_{+\infty}\frac{e^x}{x^n} = +\infty}$ ($e^x$ écrase TOUT polynôme !) ;
  $\boxed{\lim_{-\infty}x^ne^x = 0}$ ; $\lim_{+\infty}xe^{-x} = 0$.
- 2020R : $u$ croissante SANS limites demandées (tableau seul !) — mais les CC servent partout ailleurs.

### 2.5 Inégalité star & tangente
- $\boxed{e^x\ge x+1}$ (égalité en $0$ seulement !) : la courbe est AU-DESSUS de sa tangente en 0 ($y = x+1$).
  (Preuve : $h(x) = e^x-x-1$, $h' = e^x-1$, min en $0$ : $h(0) = 0$ !)

### 2.6 Équations & inéquations (le changement $X = e^x$)
- $e^{2x}-3e^x+2 = 0$ : poser $X = e^x$ ($X > 0$ !) → $X^2-3X+2 = 0$ → $X = 1, 2$ → $\boxed{x = 0\,,\,\ln 2}$.
- $e^a < e^b \iff a < b$ (appliquer $\ln$ : les inégalités se préservent !).

### 2.7 Puissances $a^x$ et $x^\alpha$ (généralisation)
- $a^x = e^{x\ln a}$ ($a > 0$) : $(a^x)' = \ln a\cdot a^x$ ; si $a > 1$ : croissante (même profil que $e^x$ !).
- $x^\alpha = e^{\alpha\ln x}$ ($x > 0$) : $(x^\alpha)' = \alpha x^{\alpha-1}$ (retrouve les puissances !).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** الأسية = **عكس اللوغاريتم**! $y = e^x$ ⟺ $x = \ln y$! والدالة الوحيدة اللي **مشتقتها هي هي** ($y' = y$)!

1. **العدد $e$:** $e \approx 2,718$ — بحال $\pi$ (ثابت طبيعي)! $e^0 = 1$، و$e^x$ **موجبة ديماً** (ما كتوصلش للصفر — مقارب أفقي!)!
2. **القواعد:** نفس الأسس! $e^{a+b} = e^ae^b$، $e^{-a} = 1/e^a$! والمقارنة: $e^a < e^b$ ⟺ $a < b$ (طالعة تماماً — طبق $\ln$ للتبسيط!)!
3. **المشتقة:** $(e^x)' = e^x$ (ما كتتبدلش — البطلة!) و$(e^u)' = u'e^u$ (**$u'$ إجباري** — الغلطة رقم 1!)! 2020R: $u' = \frac{(e^x-1)^2+2}{e^x}$ — البسط موجب ديماً (مربع + 2!) ← طالعة ديماً!
4. **النهايات:** فـ $-\infty$ ← صفر (المقارب!)، فـ $+\infty$ ← لانهاية! والمقارنات: $e^x$ **كتسحق** أي حدية ($e^x/x^n \to +\infty$)! و$(e^x-1)/x \to 1$ (معدل التغير فـ 0!)!
5. **المتباينة النجمة:** $e^x \ge x+1$ (التساوي غير فـ $0$!) — المنحنى **فوق** المماس! (البرهان: $h = e^x-x-1$، القعر فـ $0$!)!
6. **المعادلات:** بدل $X = e^x$ (**$X > 0$** إجباري!) ← معادلة عادية ← رجع ($x = \ln X$)! $e^{2x}-3e^x+2 = 0$ ← $X = 1, 2$ ← $x = 0, \ln 2$!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — $e^x$ موجبة: استعملها!** أي إشارة فيها $e^x$ ← تجاهلها ($e^x > 0$ ديماً)! 2020R: $u' = \frac{(e^x-1)^2+2}{e^x} > 0$ — البسط (مربع+2) والمقام ($e^x$) موجبين ← الإشارة باينة بلا حساب!

**الخطوة 2 — النهايات: حدد المعركة!** $e^x$ ضد حدية فـ $+\infty$ ← $e^x$ كتربح ديماً! $x^n$ ضد $e^x$ فـ $-\infty$ ← $e^x$ كتموت ($x^ne^x \to 0$)! سم المتصارعين قبل ما تحسب!

**الخطوة 3 — المركبة: $u'$ ثم $u'$ ثم $u'$!** $(e^{3x-1})' = 3e^{3x-1}$ — اللي نسى الـ 3 خسر الجدول! و$(e^{-x})' = -e^{-x}$ (السالب!) — أشهر $u'$ منسية!

**الخطوة 4 — المعادلات: التبديل $X = e^x$!** أي معادلة فيها $e^{2x}$ و$e^x$ ← $X$ ← تربيعية ← تحقق ($X > 0$!) ← $x = \ln X$! والجذور السالبة ديال $X$ **مرفوضة** ($e^x > 0$ ديماً)!

**الخطوة 5 — الأخطاء القاتلة:** $u'$ منسية ($(e^{2x})' = e^{2x}$!)؛ $e^{a+b} = e^a+e^b$ (جداء ماشي جمع!)؛ $X \le 0$ مقبولة (مرفوضة!)؛ $\lim_{-\infty}e^x = -\infty$ (= 0+!)؛ $e^x = 0$ عندها حل (مستحيل!)؛ $(e^x-1)/x$ فـ $x \ne 0$ محولة لـ 1 (غير فـ 0!)!

## 5. Définitions clés (FR + Darija)

| Notion | FR | بالدارجة |
|---|---|---|
| $e\approx 2,718$ | Base naturelle ($\exp(1)$) | الأساس الطبيعي |
| $y = e^x \iff x = \ln y$ | Réciproque de $\ln$ | عكس اللوغاريتم |
| $(e^u)' = u'e^u$ | Dérivée de composée | المشتقة — $u'$ إجباري! |
| $e^x/x^n\to+\infty$ | CC : $e^x$ écrase les polynômes | الأسية كتسحق الحديات! |
| $e^x\ge x+1$ | Au-dessus de la tangente en 0 | فوق المماس! |
| $a^x = e^{x\ln a}$ | Puissances généralisées | الأسس العامة |

## 6. FAQ du chapitre

**Q1. Pourquoi $(e^x)' = e^x$ ?**
C'est la DÉFINITION (l'unique solution de $y' = y$, $y(0) = 1$ — admis au bac, démontré au supérieur !).
Intuition : croissance proportionnelle à la taille ⟹ pente = valeur. Tout le reste (limites, CC) en découle !
بالدارجة: هادي هي **التعريف** (الحل الوحيد ديال $y' = y$ مع $y(0) = 1$)! الحدس: النمو المتناسب مع الحجم ← الميل = القيمة! وكلشي الآخر كيتبع!

**Q2. $e^x$ et $\ln x$ : quel lien exact ?**
Réciproques : $e^{\ln x} = x$ ($x > 0$), $\ln(e^x) = x$ (tout $x$). Leurs courbes sont SYMÉTRIQUES par $y = x$ !
Truc : bloqué avec $e^x$ ? Applique $\ln$ (et vice versa) !
بالدارجة: عكس بعض: $e^{\ln x} = x$ و$\ln(e^x) = x$! والمنحنيين متناظرين حول $y = x$! الحيلة: وحلتي مع $e^x$؟ طبق $\ln$ (والعكس)!

**Q3. Pourquoi $e^x$ bat $x^n$ ?**
$y' = y$ : plus $e^x$ grandit, plus sa pente grandit (emballement !). $x^n$ : pente $nx^{n-1}$ qui grandit MOINS vite
que la fonction. L'emballement exponentiel finit toujours par distancer : $\frac{e^x}{x^n}\to+\infty$ !
بالدارجة: $y' = y$: ملي $e^x$ كبرات الميل كيكبر (الانفلات!)! $x^n$: الميل كيكبر بشوية! الانفلات الأسي ديماً كيسبق فاللخر!

**Q4. $(e^x-1)/x\to 1$ : pourquoi ?**
Taux d'accroissement de $e^x$ en $0$ : limite $= (e^x)'(0) = e^0 = 1$ ! (Même mécanisme que $\frac{\sin x}{x}$,
$\frac{\ln(1+x)}{x}$ : toutes les limites « usuelles » sont des NOMBRES DÉRIVÉS déguisés !)
بالدارجة: معدل تغير $e^x$ فـ $0$ = المشتقة فـ $0$ = $1$! (جميع النهايات «الاعتيادية» أعداد مشتقة متنكرة!)

**Q5. $e^x = 0$ ? $e^x < 0$ ?**
IMPOSSIBLE ($e^x > 0$ toujours !). Conséquences : $X = e^x$ exige $X > 0$ (rejeter les $\le 0$ !) ; $e^x = -5$ :
ensemble vide $\emptyset$ (pas « $x = \ln(-5)$ » !).
بالدارجة: مستحيل ($e^x$ موجبة ديماً)! النتائج: $X = e^x$ خاص $X > 0$ (رفض السالب!)؛ $e^x = -5$: مجموعة خاوية (ماشي $\ln(-5)$!)

**Q6. $a^x$ vs $e^x$ ?**
$a^x = e^{x\ln a}$ : MÊME profil si $a > 1$ (croissante, CC !), DÉCROISSANTE si $0 < a < 1$ ($2^x$ monte, $(1/2)^x$
descend !). $(a^x)' = \ln a\cdot a^x$ (le $\ln a$ = le « $u'$ » !).
بالدارجة: $a^x = e^{x\ln a}$: نفس الشكل إلا $a > 1$ (طالعة!)، وهابطة إلا $0 < a < 1$! ($2^x$ طالعة و$(1/2)^x$ هابطة!) والمشتقة $\ln a\cdot a^x$!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : $e^x > 0$ cité (signes, $X > 0$ !) ; $u'$ dans $(e^u)'$ ; CC nommées (« par croissances
comparées ») ; $X = e^x$ + domaine $X > 0$ + retour $x = \ln X$ ; $\boxed{\text{résultats}}$.
**Erreurs fréquentes** : $u'$ oublié ❌ ; $e^{a+b} = e^a+e^b$ ❌ ; $X\le 0$ accepté ❌ ; $\lim_{-\infty}e^x = -\infty$ ❌ ;
$e^x = 0$ résolue ❌ ; $(e^x-1)/x\to 1$ hors de 0 ❌ ; $e^x\ge x+1$ inversée ❌.

## 8. Sources de ce chapitre
- National Maths SX 2020 Rattrapage Ex.3 Q1 ($u' = \frac{(e^x-1)^2+2}{e^x}$, variations, signe de $u$) —
  filière SP confirmée (RR 22F). https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ +
  corrigé officiel https://www.alloschool.com/element/109814.
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-15.

## 9. Le « pourquoi » profond — $y' = y$ gouverne tout 🔬

**Pourquoi $(e^x)' = e^x$ ? (la définition qui fait tout)**
$\exp$ EST définie (au bac : admise ; au sup : construite) comme L'UNIQUE fonction avec $f' = f$ et $f(0) = 1$.
Tout le reste est THÉORÈME : $e^{a+b} = e^ae^b$ (considérer $f(x) = e^{x+a}/e^x$ : $f' = 0$ !), $e^x > 0$
($e^x\cdot e^{-x} = 1$ : jamais nul + continu + $e^0 = 1$ !), CC... Une seule propriété-mère ($y' = y$), TOUTE une
famille de conséquences. C'est l'exemple parfait de la puissance axiomatique !

**Pourquoi $e^x$ écrase $x^n$ ? (l'emballement)**
$y' = y$ : la pente de $e^x$ égale sa VALEUR — plus ça monte, plus ça monte VITE (boucle positive !). $x^n$ :
pente $nx^{n-1}$ : le rapport pente/valeur $= n/x \to 0$ (la croissance relative S'ÉSSOUFFLE !). $e^x$ : rapport
$= 1$ CONSTANT (jamais essoufflé !). À croissance relative constante vs déclinante, la constante gagne TOUJOURS
à long terme : $\frac{e^x}{x^n}\to+\infty$. C'est de l'ÉCONOMIE (taux constant vs taux qui fond !).

**Pourquoi $e^x\ge x+1$ ? (la convexité)**
$(e^x)'' = e^x > 0$ : $e^x$ est CONVEXE (sourire !) → la courbe est AU-DESSUS de TOUTES ses tangentes (propriété
des convexes !), dont $y = x+1$ en $0$. Donc $e^x\ge x+1$ n'est pas un hasard : c'est la convexité + la tangente
en $0$. Généralisation : $e^x$ au-dessus de $y = e^a(x-a)+e^a$ en TOUT $a$ (même raison !).

**Ponts :** ch.05 ($\ln$ : la réciproque — les deux chapitres SE RÉPONDENT : $e^{\ln x} = x$ !) ; ch.01 (limites :
CC, $(e^x-1)/x$ : le taux !) ; ch.02 (dérivées : $(e^u)'$, convexité $f''$ !) ; ch.03 (suites géométriques $q^n$ :
l'exponentielle DISCRÈTE ! $u_{n+1} = q\,u_n$ ⟷ $y' = ky$ !) ; PC RC/RL/RLC ($e^{-t/\tau}$ : inversion du temps !) ;
PC radioactivité ($N = N_0e^{-\lambda t}$ : $e^x$ qui DÉCROÎT !) ; SVT (croissance bactérienne : $N = N_02^{t/T}$ !).

> بالدارجة: علاش $(e^x)' = e^x$؟ حيت هادي هي **التعريف** (الحل الوحيد ديال $y' = y$)! وكلشي الآخر **مبرهنات**: $e^{a+b} = e^ae^b$، $e^x > 0$... خاصية-أم وحدة وعائلة كاملة! وعلاش $e^x$ كتسحق $x^n$؟ حيت النمو النسبي ديالها **ثابت** ($y'/y = 1$ — ما كيتعبش!) ضد المتناقص ($n/x \to 0$ — كيتعب!)! الثابت كيربح ديماً فالمدى الطويل! و$e^x \ge x+1$؟ التقعر (الابتسامة!): المنحنى **فوق** أي مماس!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $(e^{2x})' = e^{2x}$ — le $u'$ fantôme (encore lui !).**
*Le clic :* $(e^u)' = u'e^u$ : $(e^{2x})' = 2e^{2x}$, $(e^{-x})' = -e^{-x}$, $(e^{x^2})' = 2xe^{x^2}$. Le $u'$ EST la
méthode (ch.02-C3 !). 2020R : $u$ contient $-3e^{-x}$ : dérivée $+3e^{-x}$ (le $-$ de $-x$ !) — signe critique !
بالدارجة: $(e^{2x})' = 2e^{2x}$ و$(e^{-x})' = -e^{-x}$ — الـ $u'$ هو الطريقة! 2020R: $-3e^{-x}$ مشتقتها $+3e^{-x}$ (سالب $-x$!) — الإشارة حاسمة!

**C2. $e^{a+b} = e^a+e^b$ — l'addition distribuée.**
*Le clic :* $e^{a+b} = e^a\times e^b$ (PRODUIT !). Test : $e^{1+1} = e^2\approx 7,39$ mais $e+e\approx 5,44$ :
DIFFÉRENT ! L'exponentielle transforme les SOMMES en PRODUITS (c'est sa RAISON D'ÊTRE : $\ln$ fait l'inverse !).
بالدارجة: $e^{a+b} = e^a\times e^b$ (**جداء**!)! اختبر: $e^2 \approx 7,39$ ضد $e+e \approx 5,44$ — مختلفين! الأسية كتحول **المجاميع لجداءات** (هادي هي علاش كاينة!)!

**C3. $X = e^x\le 0$ accepté — le domaine trahi.**
*Le clic :* $e^{2x}-3e^x+2 = 0$ → $X = 1, 2$ : les deux $> 0$ ✔. Mais $e^{2x}+e^x-6 = 0$ → $X = 2, -3$ : $-3$ REFUSÉ
($e^x = -3$ impossible !) → SEUL $x = \ln 2$ ! Toujours filtrer $X > 0$ AVANT de prendre $\ln$.
بالدارجة: $X = 2, -3$: $-3$ **مرفوضة** ($e^x = -3$ مستحيلة!) ← غير $x = \ln 2$! صفي $X > 0$ **قبل** ما تاخذ $\ln$!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. $\ln$ (ch.05) : réciproque, domaine $> 0$, $\ln 1 = 0$ — le miroir de $\exp$.
2. Dérivées composées (ch.02) : $(e^u)' = u'e^u$ — le geste technique n°1.
3. Second degré : $X^2+\ldots$ après $X = e^x$ — équations !
4. Limites (ch.01) : FI, CC — le calcul aux bornes.

**Si l'étude exp bloque — plan B :**
Le mur : $f'$ avec $e^x$ + polynôme mélangés, signe illisible. **Fallback** : (1) FACTORISER $e^{ax}$ (le plus grand
facteur commun !) : $e^{2x}-3e^x = e^x(e^x-3)$ : signe = signe de $(e^x-3)$ ($e^x > 0$ !) ; (2) limite FI : factoriser
le DOMINANT ($e^x$ en $+\infty$, $x^n$ en $-\infty$ !) ; (3) équation emmêlée : $X = e^x$ + filtre $X > 0$ ;
(4) admettre le tableau et foncer (TVI, aires : 70 % des points APRÈS !).
بالدارجة: إلا تخلط $e^x$ مع حدية: **عمّل** بـ $e^{ax}$ ($e^{2x}-3e^x = e^x(e^x-3)$: الإشارة = إشارة $(e^x-3)$)! والنهايات: عمّل بالغالب ($e^x$ فـ $+\infty$)! والمعادلات: $X = e^x$ + التصفية! وإلا بقات حابسة: قبل الجدول وكمل (70 % من بعد)!
