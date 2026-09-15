---
chapitre: "04 - Fonctions primitives"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Normale Ex.3 Q2 (réel, SP : primitive G + intégrale) + synthèse prof (canon national)"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 04 — Fonctions primitives

> 📋 **Exigible au bac** : $F$ primitive de $f$ sur $I$ $\iff$ $F' = f$ ; unicité à $+C$ près ; tableau usuelles ($x^n$, $1/x \to \ln|x|$, $e^x$, $\cos/\sin$) ; formes $u'u^n$, $u'/u \to \ln|u|$, $u'e^u$ ; linéarité ; lien intégrale $\int_a^b f = F(b) - F(a)$ (M09).

## 1. Accroche — rembobiner le film ⏪

Dériver, c'est passer du trajet à la vitesse. **Primitiver, c'est l'inverse : retrouver le trajet quand on connaît la vitesse.** Si je sais que tu roules à $2x$ près... quelle distance as-tu parcourue ? $x^2$ — mais **à une constante près** (on ne sait pas d'où tu es parti !). Cette constante oubliée, $+C$, vaut des points au bac. Tout le chapitre tient là : *dériver tue les constantes, primitiver les ressuscite (une seule, $C$).*

> بالدارجة : الاشتقاق = من المسار للسرعة. **التكامل (الدالة الأصلية) = العكس : من السرعة للمسار.** إلا عرفتي السرعة $2x$، المسافة $x^2$ — **ولكن زائد ثابت $C$** (ما عرفناش منين بديتي!). هاد $C$ المنسي كيسوى النقط. القاعدة : *الاشتقاق كيقتل الثوابت، والأصلية كتحييها (وحدة، $C$).*

## 2. Résumé du cours (exigible au bac)

**Définition.** $F$ est une primitive de $f$ sur un intervalle $I$ si $F$ est dérivable sur $I$ et $\boxed{F' = f}$. **Théorème ($+C$) :** si $F$ est une primitive de $f$ sur $I$, TOUTES les primitives sont $F + C$ ($C \in \mathbb{R}$). Deux primitives diffèrent d'une constante (car $(F - G)' = 0$ → $F - G$ constante). **Sans $+C$, la réponse est fausse** (sauf primitive avec condition $F(x_0) = y_0$ → $C$ déterminée, unique).

**Tableau usuelles (à savoir dans les 2 sens) :**

| $f(x)$ | Primitive $F(x)$ | Condition |
|---|---|---|
| $x^n$ ($n \neq -1$) | $x^{n+1}/(n+1)$ | — |
| $1/x$ | $\ln|x|$ | $x \neq 0$ (par intervalle !) |
| $e^x$ | $e^x$ | — |
| $e^{ax}$ | $e^{ax}/a$ | $a \neq 0$ (« diviser par la dérivée de l'exposant ») |
| $\cos x$ / $\sin x$ | $\sin x$ / $-\cos x$ | — |
| $\cos(ax)$, $\sin(ax)$ | $\sin(ax)/a$, $-\cos(ax)/a$ | — |
| $1/x^2$ | $-1/x$ | ($= x^{-2} \to x^{-1}/(-1)$) |
| $1/\sqrt{x}$ | $2\sqrt{x}$ | $x > 0$ ($= x^{-1/2} \to x^{1/2}/(1/2)$) |

**Formes en $u$ (le cœur du bac) :** $\boxed{u'u^n \to u^{n+1}/(n+1)}$ ($n \neq -1$) ; $\boxed{u'/u \to \ln|u|}$ ; $\boxed{u'e^u \to e^u}$. **Linéarité :** primitive de $\alpha f + \beta g$ = $\alpha F + \beta G$. **Réflexe or : VÉRIFIER en dérivant** $F$ : si $F' = f$, c'est gagné (détecte toutes les erreurs de coefficients).

**Pièges de lecture :** $1/u$ n'est PAS $\ln|u|$ sauf si le numérateur est (à un facteur près) $u'$ : $\int 1/(2x+1)\,dx = \frac{1}{2}\ln|2x+1| + C$ (facteur $1/2$ car $u' = 2$). De même $e^{3x+1} \to e^{3x+1}/3$. Règle : *si l'intérieur est affine $ax + b$, on divise par $a$.*

**Lien intégrale (M09) :** $\int_a^b f(x)\,dx = [F(x)]_a^b = F(b) - F(a)$ — le $C$ s'élimine. **Lien équa-diff (M10) :** résoudre $y' = f$ = primitiver $f$.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**التعريف :** $F$ أصلية لـ $f$ على مجال $I$ إلا كانت $F' = f$. **المبرهنة ($+C$) :** إلا كانت $F$ أصلية، **كاع** الأصليات هما $F + C$. جوج أصليات كيفرق بيناتهم غير ثابت (حيت الفرق مشتقتو صفر). **بلا $+C$ الجواب غالط** (من غير إلا عطاوك شرط $F(x_0) = y_0$ ← $C$ كتتحدد).

**الجدول (حفظو في الاتجاهين) :** $x^n \leftarrow x^{n+1}/(n+1)$ | $1/x \leftarrow \ln|x|$ | $e^x \leftarrow e^x$ | $e^{ax} \leftarrow e^{ax}/a$ | $\cos \leftarrow \sin$ | $\sin \leftarrow -\cos$ | $1/x^2 \leftarrow -1/x$ | $1/\sqrt{x} \leftarrow 2\sqrt{x}$.

**الصيغ بـ $u$ (قلب الباك) :** $u'u^n \leftarrow u^{n+1}/(n+1)$ | $u'/u \leftarrow \ln|u|$ | $u'e^u \leftarrow e^u$. **الخطية :** أصلية المجموع = مجموع الأصليات. **العادة الذهبية : تحقق بالاشتقاق** — إلا لقيتي $F' = f$ صافي ربحتي.

**فخ القراءة :** $1/u$ ماشي $\ln|u|$ إلا كان البسط هو $u'$ (تقريباً) : $\int 1/(2x+1) = \frac{1}{2}\ln|2x+1| + C$ (قسمنا على 2 حيت $u' = 2$). القاعدة : *إلا كان الداخل $ax + b$، قسّم على $a$.*

**الربط :** التكامل (M09) : $\int_a^b f = F(b) - F(a)$ ($C$ كتمشي). المعادلات التفاضلية (M10) : حل $y' = f$ = قلّب على أصلية.

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — اقلب السؤال.** شفتي $f(x) = 3x^2$ ؟ سول : «شكون هي الدالة اللي مشتقتها $3x^2$ ؟» الجواب $x^3 + C$. **الأصلية = سؤال معكوس.** أي تمرين : قرا $f$، تخيّل الاشتقاق راجع اللور.

**الخطوة 2 — $+C$ : ضريبة النسيان.** علاش $C$ ؟ حيت الاشتقاق كينسّي نقطة البداية : $(x^3 + 5)' = (x^3 - 100)' = 3x^2$. ملي كترجع اللور، مستحيل تعرف شحال كان الثابت ← كتكتب $C$. **بلا $C$ : ناقص.** مع شرط ($F(0) = 1$) : عوّض ← $C = 1$ ← وحيدة.

**الخطوة 3 — صيد $u$ (المهارة الكبيرة).** شفتي $(2x+1)^3$ ؟ الداخل $u = 2x+1$، المشتقة $u' = 2$. واش $u'$ كاين قدام ؟ لا ← **جيبو وقسّم** : $\int (2x+1)^3 = \frac{1}{2}\cdot\frac{(2x+1)^4}{4} + C$. شفتي $\frac{2x}{x^2+1}$ ؟ البسط = مشتقة المقام ($u = x^2+1$) ← $\ln(x^2+1) + C$. **اللعبة كلها : قلب على $u$ والمشتقة ديالها.**

**الخطوة 4 — تحقق ديما (30 ثانية).** لقيتي $F$ ؟ اشتقها : إلا خرجات $f$، نعستي مرتاح. هاد العادة كتكشف غلطات المعاملات ($1/2$، $1/3$...) اللي هما 90% من الأخطاء.

**الخطوة 5 — الربط مع التكامل :** التكامل المحدود = $F(b) - F(a)$. الأصلية هي الجسر : تعلمها مزيان و M09 (التكاملات) كيولّي ساهل.

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Primitive | الدالة الأصلية | $F' = f$ sur $I$ |
| $+C$ | زائد ثابت | famille infinie ; $C$ unique avec condition |
| Linéarité | الخطية | $\int(\alpha f + \beta g) = \alpha F + \beta G$ |
| Forme $u'u^n$ | صيغة $u'u^n$ | $\to u^{n+1}/(n+1)$ |
| Forme $u'/u$ | صيغة $u'/u$ | $\to \ln|u|$ (avec $|~|$ !) |
| Forme $u'e^u$ | صيغة $u'e^u$ | $\to e^u$ |
| Vérification | التحقق | dériver $F$ : retrouver $f$ |

## 6. FAQ du chapitre

**1. Pourquoi $+C$ est-il obligatoire ?** $(F + C)' = F' = f$ pour tout $C$ : il y a une infinité de primitives. Oublier $C$ = donner une seule réponse au lieu de toutes. / كاين عدد لا نهائي من الأصليات — $C$ كتجمعهم كاملين.

**2. Pourquoi $\ln|x|$ avec valeur absolue ?** $\ln$ n'existe que pour $> 0$ ; $|x|$ permet de primitiver $1/x$ sur $]-\infty, 0[$ aussi. Au bac, $x > 0$ souvent → $|~|$ facultatif mais jamais faux. / القيمة المطلقة كتخلّي $\ln$ خدام حتى للأعداد السالبة.

**3. Primitive de $1/(2x+1)$ : $\ln(2x+1)$ ?** Non : $\frac{1}{2}\ln|2x+1| + C$ — le $u' = 2$ impose de diviser par 2 (dérive pour vérifier !). / لا : خاصك تقسّم على 2 ($u' = 2$).

**4. $e^{3x+1}$ donne quoi ?** $e^{3x+1}/3 + C$ (« diviser par la dérivée de l'exposant »). / قسّم على مشتقة الأسّ : $/3$.

**5. Dérivée ou primitive — comment ne plus inverser ?** Question « calculer $F'$ » = dériver (descendre). « Déterminer une primitive » = remonter. Le mot *primitive* contient *prime* ($F'$)... piège ! $F$ est primitive de $f$ si $F' = f$ : $F$ est « au-dessus ». / *primitive* = طلع لفوق ($F$)، المشتقة = هبط لتحت.

**6. Toute fonction a-t-elle une primitive explicite ?** Toute continue a des primitives (théorème), mais pas toujours avec des formules usuelles : $e^{-x^2}$ n'a PAS de primitive élémentaire ! (Culture : c'est pour ça que Gauss se calcule autrement.) / الاستمرارية كتضمن الوجود، ماشي الصيغة : $e^{-x^2}$ ما عندوش أصلية بالدوال العادية !

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **$+C$ oublié** : réponse incomplète = points perdus. Réflexe : *pas de bornes → $+C$.*
- 🪤 **$\ln$ sans $|~|$** : $\int u'/u = \ln|u| + C$ — les barres sont exigibles (même si $u > 0$ évident, elles ne coûtent rien).
- 🪤 **Coefficient $1/a$ oublié** : $(2x+1)^3 \to \frac{(2x+1)^4}{8}$, pas $/4$ ! ($u' = 2$ → compenser $1/2$.) Vérifier en dérivant.
- 🪤 **$1/u$ confondu avec $u'/u$** : $\int \frac{dx}{x^2+1} \neq \ln(x^2+1)$ (le numérateur n'est pas $2x$ !) — c'est $\arctan$ (hors 2BAC SP : ne pas inventer).
- Mots-clés : *intervalle $I$, $+C$, repérer $u$ et $u'$, compenser $1/u'$, vérifier par dérivation.*

## 8. Sources de ce chapitre

- National Maths SX 2020 Normale Ex.3 Q2 (réel, SP) : $G(x) = x(-1+4\sqrt{x}/3-\ln x)$ primitive de $g = 2\sqrt{x}-2-\ln x$, $\int_1^4 g = 19/3-8\ln 2$ — https://etude-generale.com/correction-dexamen-national-2020-math-science-physique/ ; + synthèse prof ; ponts M02, M09, M10.

## 9. Le « pourquoi » profond — pourquoi $+C$, pourquoi $\ln$ 🔬

**Pourquoi deux primitives diffèrent-elles d'une constante ?** Si $F' = G' = f$, alors $(F-G)' = 0$ : une fonction de dérivée nulle sur un intervalle est constante (théorème des accroissements finis). C'est profond : *la dérivée voit les variations, pas les positions* — primitiver, c'est retrouver une position à partir de variations, d'où l'ambiguïté $C$ (le point de départ inconnu).

**Pourquoi $\ln|x|$ est-il LA primitive de $1/x$ ?** Sur $]0, +\infty[$, $(\ln x)' = 1/x$ (M05 : $\ln$ est défini comme LA primitive de $1/x$ valant 0 en 1 !). Sur $]-\infty, 0[$, $(\ln(-x))' = (-1)/(-x) = 1/x$. $|x|$ fusionne les deux. Le logarithme n'est pas un hasard : il est **né** comme primitive de $1/x$ (M04 ⟷ M05 : chaque chapitre engendre l'autre).

**Pourquoi certaines fonctions n'ont-elles pas de primitive « formula » ?** $e^{-x^2}$ est continue → elle A des primitives (aire sous la courbe, M09). Mais aucune combinaison finie de fonctions usuelles ne se dérive en $e^{-x^2}$ (théorème de Liouville, culture). Moralité : *exister ≠ s'écrire* — les maths distinguent l'existence (analyse) et l'expression (calcul). C'est pour ça que le bac ne demande que des formes $u$ bien choisies.

**Liens croisés :** M02 — primitiver = dériver à l'envers (même tableau, sens inverse) ; M05 — $\ln$ défini via primitive de $1/x$ ; M09 — $F(b) - F(a)$ : la primitive est le moteur du calcul intégral ; M10 — $y' = f$ se résout en primitivant ; PC — vitesse/position, $v(t) = v_0 + at$ = primitive de $a$ !

## 10. Les 3 confusions qui coûtent des points 😵

**1. « Primitive de $x^n$ : $nx^{n-1}$. »** Ça, c'est la DÉRIVÉE ! **Le déclic :** *dériver = exposant descend ($n \to n-1$) ; primitiver = exposant monte ($n \to n+1$, on divise).* Compte sur tes doigts : $x^2 \leftarrow x^3/3$ (monte !).

**2. « $\int \frac{dx}{x^2+1} = \ln(x^2+1)$. »** Faux : $(\ln(x^2+1))' = 2x/(x^2+1) \neq 1/(x^2+1)$. **Le déclic :** $\ln|u|$ exige le $u'$ au numérateur — *pas de $u'$, pas de $\ln$.* La vérification par dérivation tue ce piège en 10 secondes.

**3. « $+C$ aussi pour les intégrales définies. »** Non : $\int_a^b f = F(b) - F(a)$, le $C$ s'élimine ($+C - C$). **Le déclic :** *bornes = $C$ inutile (mais pas faux si écrit puis simplifié) ; pas de bornes = $C$ obligatoire.*

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** dérivées usuelles + composées (M02 : $(u^n)'$, $(\ln u)'$, $(e^u)'$), calcul algébrique (fractions, puissances). **Test 30 s :** $((2x+1)^4)'$ → $8(2x+1)^3$ ; $(\ln(x^2+1))'$ → $2x/(x^2+1)$. Si ça coince, revoir M02 avant.

**Plan B — le plus dur (repérer $u$ et compenser) :** face à $f$, demande-toi : (1) *Quel est l'intérieur $u$ ?* (2) *Sa dérivée $u'$ est-elle devant ?* — oui → formule directe ; non → *est-elle constante ?* → compenser par $1/u'$. Si $u'$ n'est ni présent ni constant → ce n'est pas une forme $u$ (changer de piste). Puis **vérifier** en dérivant. Cette boucle traite 100 % des primitives du bac.

**Fiche réflexes :** *$F' = f$ · pas de bornes → $+C$ · repérer $u$/$u'$ · intérieur affine → $/a$ · $\ln$ avec $|~|$ · vérifier en dérivant.*
