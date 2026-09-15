---
chapitre: "10 - Équations différentielles"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (canon national : y'+ay=0, y'+ay=b, y''+w²y=0) + ponts PC"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 10 — Équations différentielles

> 📋 **Exigible au bac** : $(E_0)$ : $y' + ay = 0$ → $y = Ce^{-ax}$ ; $(E)$ : $y' + ay = b$ → $y = Ce^{-ax} + b/a$ ; $(E_2)$ : $y'' + \omega^2 y = 0$ → $y = A\cos(\omega x) + B\sin(\omega x)$ ; conditions initiales ; applications (radioactivité, RC, oscillateurs).

## 1. Accroche — le detective et la vitesse 🕵️

Un détective ne voit pas la voiture, mais il connaît **à chaque instant sa vitesse en fonction de sa position** : « la vitesse vaut toujours le double de la distance restante ». Peut-il retrouver le trajet complet ? Oui — c'est exactement une équation différentielle : **une équation dont l'inconnue est une fonction**, reliée à ses dérivées. Au bac, 3 types seulement — et chacun a sa recette.

> بالدارجة : المعادلة التفاضلية = معادلة المجهول ديالها **دالة** ماشي عدد. كتعطيك العلاقة بين الدالة والمشتقة ديالها، ونتايا كتقلب على الدالة. في الباك غير 3 أنواع — وكل وحدة عندها الوصفة ديالها.

## 2. Résumé du cours (exigible au bac)

**Type 1 — $(E_0)$ : $y' + ay = 0$ (sans second membre).** Solutions sur $\mathbb{R}$ : $\boxed{y(x) = Ce^{-ax}}$ où $C \in \mathbb{R}$ est une constante arbitraire. Cas vedette : $y' = -ky$ ($k > 0$) → décroissance exponentielle $Ce^{-kx}$ (radioactivité P04, charge RC, refroidissement). Condition initiale $y(x_0) = y_0$ → $C$ unique : $C = y_0 e^{ax_0}$.

**Type 2 — $(E)$ : $y' + ay = b$ ($a \neq 0$, $b$ constante).** Recette en 2 temps : (1) solution particulière constante $y_p = b/a$ (elle annule $y'$ : $0 + a(b/a) = b$ ✓) ; (2) ajouter le général de $(E_0)$. Solutions : $\boxed{y(x) = Ce^{-ax} + b/a}$. La constante $b/a$ est la **valeur d'équilibre** (vers quoi tend $y$ si $a > 0$). Condition initiale → $C$ unique.

**Type 3 — $(E_2)$ : $y'' + \omega^2 y = 0$ ($\omega > 0$).** Solutions : $\boxed{y(x) = A\cos(\omega x) + B\sin(\omega x)}$, $A, B \in \mathbb{R}$. Deux constantes → il faut **deux** conditions ($y(0)$ et $y'(0)$ en général). Dérivée utile : $y'(x) = -A\omega\sin(\omega x) + B\omega\cos(\omega x)$. Physique : oscillateur harmonique (ressort P14/P15, pendule), $\omega$ = pulsation, $T = 2\pi/\omega$.

**Méthode universelle (les 3 pas) :** ① identifier le type + recopier $a$ (ou $\omega$) **avec son signe** ; ② écrire la solution générale (formule) ; ③ injecter la/les condition(s) initiale(s) → déterminer $C$ (ou $A, B$). **Réflexe or** : toujours **vérifier** en redérivant et en réinjectant dans l'équation (30 secondes qui sauvent des points).

**Lecture physique (ponts PC) :** $a > 0$ dans $y' + ay = 0$ → retour vers 0 (amortissement, décroissance) ; $a < 0$ → explosion (emballement, comme $e^{+kx}$ en M07). Dans $y' + ay = b$ ($a > 0$), $b/a$ = régime permanent (ex : vitesse limite en chute avec frottement P11, tension finale du condensateur).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**النوع 1 — $y' + ay = 0$ (بلا طرف ثاني) :** الحل : $\boxed{y = Ce^{-ax}}$ حيث $C$ ثابت اختياري. المثال النجم : $y' = -ky$ ← تناقص أسّي (النشاط الإشعاعي، شحن المكثف). الشرط الابتدائي $y(x_0) = y_0$ كيعطيك $C$ وحيدة.

**النوع 2 — $y' + ay = b$ :** الوصفة : (1) حل خاص ثابت $y_p = b/a$ ؛ (2) زيد الحل العام ديال النوع 1. الحل : $\boxed{y = Ce^{-ax} + b/a}$. القيمة $b/a$ هي **قيمة التوازن** (فين كتمشي $y$ إلا كان $a > 0$).

**النوع 3 — $y'' + \omega^2 y = 0$ :** الحل : $\boxed{y = A\cos(\omega x) + B\sin(\omega x)}$. جوج ثوابت ← خاصك **جوج** شروط ($y(0)$ و $y'(0)$). الفيزياء : الهزاز التوافقي (النابض، النواس)، $\omega$ هي النبض، $T = 2\pi/\omega$.

**المنهجية (3 خطوات) :** ① حدد النوع وانسخ $a$ (ولا $\omega$) **بالإشارة ديالو** ؛ ② كتب الحل العام (الصيغة) ؛ ③ عوّض الشرط الابتدائي ← حدد $C$ (ولا $A, B$). **العادة الذهبية** : ديما **تحقق** بإعادة الاشتقاق والتعويض في المعادلة.

**القراءة الفيزيائية :** $a > 0$ ← رجوع للصفر (تخامد) ؛ $a < 0$ ← انفجار (بحال $e^{+kx}$). في النوع 2 ($a > 0$)، $b/a$ = النظام الدائم (السرعة الحدية، التوتر النهائي).

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — شنو كتقلب ؟ دالة، ماشي عدد.** المعادلة العادية : $2x + 3 = 7$ ← الجواب عدد ($x = 2$). المعادلة التفاضلية : $y' + 2y = 0$ ← الجواب **دالة** ($y = Ce^{-2x}$). السؤال ديما : «شكون هي الدالة اللي المشتقة ديالها مربوطة بيها بهاد الطريقة ؟»

**الخطوة 2 — النوع 1 : فكّر في $e$.** $y' = -2y$ معناها : «المشتقة = $-2$ × الدالة». شكون هي الدالة اللي مشتقتها متناسبة معاها ؟ **الأسّية !** $(e^{-2x})' = -2e^{-2x}$ ✓. إذن الحل $Ce^{-2x}$ — والـ $C$ كتحددها بالشرط الابتدائي (نقطة البداية). حفظ : *المعامل $a$ كيدخل في الأسّ بإشارة معاكسة.*

**الخطوة 3 — النوع 2 : التوازن + الرجوع.** $y' + 2y = 6$ : تخيّل حوض فيه ثقب (التسرب $-2y$) وصنبور كيصب ($+6$). التوازن : التسرب = الصب ← $2y = 6$ ← $y = 3$ (الحل الخاص $b/a$). والفرق مع التوازن كيتناقص أسّياً ($Ce^{-2x}$). الحل الكامل : توازن + رجوع = $3 + Ce^{-2x}$.

**الخطوة 4 — النوع 3 : اللي كتدور كترجع.** $y'' = -4y$ معناها : «المشتقة الثانية = $-4$ × الدالة». شكون كيرجع لنفسو (بإشارة ناقص) من بعد جوج اشتقاقات ؟ **$\cos$ و $\sin$ !** $(\cos 2x)'' = -4\cos 2x$ ✓. إذن $A\cos 2x + B\sin 2x$ — وجوج ثوابت حيت اشتقينا جوج مرات (خاصك الموضع والسرعة في البداية).

**الخطوة 5 — الغلطة القاتلة : الإشارة.** $y' = 3y$ ← $a = -3$ (ردّها للشكل $y' + ay = 0$ : $y' - 3y = 0$) ← الحل $Ce^{+3x}$ ماشي $Ce^{-3x}$ ! **القاعدة : ديما كتب المعادلة على الشكل النظامي اللول، عاد قرا $a$.**

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Équation différentielle | معادلة تفاضلية | équation d'inconnue fonction (+ dérivées) |
| Ordre | الرتبة | rang de la dérivée la + haute (1 ou 2 au bac) |
| Solution générale | الحل العام | famille avec $C$ (ou $A, B$) arbitraires |
| Solution particulière | الحل الخاص | une fonction qui vérifie (ex : $b/a$) |
| Condition initiale | الشرط الابتدائي | $y(x_0) = y_0$ → fixe $C$ (unicité) |
| Valeur d'équilibre | قيمة التوازن | $b/a$ : limite si $a > 0$ |
| Pulsation $\omega$ | النبض | $y = A\cos\omega x + B\sin\omega x$, $T = 2\pi/\omega$ |

## 6. FAQ du chapitre

**1. Pourquoi une constante $C$ ? Et pourquoi elle disparaît avec la CI ?** Dériver tue les constantes : une infinité de fonctions ($C$ quelconque) ont « la même dérivée relative ». La CI choisit **laquelle** passe par le point imposé (unicité). / الاشتقاق كيقتل الثوابت — الشرط الابتدائي كيختار وحدة من العائلة.

**2. $y' = 3y$ : $a = 3$ ou $-3$ ?** Mets sous forme $y' + ay = 0$ : $y' - 3y = 0$ donc $a = -3$, solution $Ce^{+3x}$. **Toujours normaliser d'abord !** / ردّها للشكل النظامي اللول : $a = -3$ ← الحل $Ce^{+3x}$.

**3. Pourquoi $b/a$ est-il solution de $y' + ay = b$ ?** Une constante a une dérivée nulle : $0 + a(b/a) = b$ ✓. C'est l'équilibre (dérivée nulle = état stationnaire). / الثابت مشتقتو صفر : $0 + a(b/a) = b$ ✓ — هو التوازن.

**4. Pourquoi deux constantes pour l'ordre 2 ?** Chaque intégration apporte une constante ; ordre 2 = 2 intégrations = $A$ et $B$ = il faut position ET vitesse initiales. / كل مكاملة كتجيب ثابت : الرتبة 2 = جوج ثوابت = الموضع والسرعة.

**5. $\cos$ ou $\sin$ — comment choisir $A$ et $B$ ?** On ne choisit pas : les CI décident. $y(0) = A$ (car $\cos 0 = 1$, $\sin 0 = 0$) et $y'(0) = B\omega$. / الشروط الابتدائية كتقرر : $y(0) = A$ و $y'(0) = B\omega$.

**6. Quel lien avec la physique ?** $N' = -\lambda N$ (radioactivité), $u_c' + u_c/RC = E/RC$ (condensateur), $y'' + \omega^2 y = 0$ (ressort). Même maths, trois mondes. / نفس الرياضيات : الإشعاعية، المكثف، النابض.

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **Signe de $a$** : $y' = 3y$ → $a = -3$ → $e^{+3x}$. Normaliser AVANT de recopier. ($e^{+3x}$ vs $e^{-3x}$ = 0 ou plein de points.)
- 🪤 **$C$ oublié ou « déterminé » sans CI** : sans condition initiale, $C$ reste arbitraire — ne jamais l'inventer.
- 🪤 **Ordre 2 avec une seule condition** : $A$ et $B$ exigent 2 CI ; avec une seule, exprimer l'une en fonction de l'autre.
- 🪤 **$\omega$ vs $\omega^2$** : $y'' + 9y = 0$ → $\omega = 3$ (racine !) → $\cos 3x$, pas $\cos 9x$.
- Mots-clés : *forme normalisée, solution générale/particulière, équilibre $b/a$, unicité (CI), vérification par réinjection.*

## 8. Sources de ce chapitre

- Canon national 2BAC SP (3 types exigibles + CI) — synthèse prof ; applications PC (P04 radioactivité, P11 chute, P14/P15 oscillateurs).

## 9. Le « pourquoi » profond — pourquoi $e$, pourquoi $\cos$ 🔬

**Pourquoi l'exponentielle gouverne l'ordre 1 ?** L'équation $y' = ky$ demande : « quelle fonction est proportionnelle à sa dérivée ? » Or $e^{kx}$ est (à un facteur près) la **seule** : c'est sa définition même ($(e^u)' = u'e^u$, M07). Les équa-diff d'ordre 1 ne sont donc pas un chapitre isolé : ce sont les **ombres de l'exponentielle** — chaque fois que la variation est proportionnelle à l'état (désintégrations, charge, refroidissement), $e$ apparaît. C'est pour ça que toute la physique en est pleine.

**Pourquoi $\cos/\sin$ gouvernent $y'' + \omega^2 y = 0$ ?** L'équation demande une fonction qui, dérivée deux fois, se retrouve au signe près. Or dériver $\cos$, c'est tourner d'un quart de tour dans le cercle trigonométrique (M02) : deux quarts de tour = demi-tour = opposé. $\cos$ et $\sin$ sont les **seules** fonctions bornées avec cette propriété — d'où les oscillations éternelles (sans frottement).

**Pourquoi l'unicité (une CI = une solution) ?** Une équa-diff d'ordre 1 dit « en chaque point, la pente est imposée » : c'est un champ de directions. Partir d'un point avec des pentes imposées partout ne laisse qu'**un seul chemin** possible — comme suivre une rivière depuis sa source. La CI = le point de départ ; le champ = l'équation.

**Liens croisés :** M07 — $e^{kx}$ comme solution universelle de l'ordre 1 ; M02 — $\cos/\sin$ et le cercle ; M04 — résoudre = primitiver (intégrer) ; PC — $N' = -\lambda N$ (P04), $v' + kv = g$ (P11), $x'' + \omega^2 x = 0$ (P14/P15) : trois chapitres de PC qui SONT ce chapitre.

## 10. Les 3 confusions qui coûtent des points 😵

**1. « $y' = 3y$ donne $e^{-3x}$. »** Non : $a = -3$. **Le déclic :** récite *« $y'$ + $ay$ = 0, je normalise d'abord »* — écris $y' - 3y = 0$ au brouillon, le signe devient imbattable.

**2. « $y'' + 9y = 0$ donne $\cos 9x$. »** Non : $\omega^2 = 9$ donc $\omega = 3$. **Le déclic :** $\omega$ est une *fréquence* (ce qui multiplie $x$), $\omega^2$ son carré dans l'équation — passer de l'équation à la solution exige une **racine carrée**.

**3. « La solution particulière, c'est avec $C = 0$. »** Non : $C = 0$ donne UNE solution particulière du type 1, mais pour le type 2, « particulière » = la constante d'équilibre $b/a$. **Le déclic :** *générale = famille ($C$) ; particulière = un membre choisi* (équilibre ou CI).

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** dérivées (M02 : $(e^u)'$, $(\cos)'$), exponentielle (M07 : sens de $e^{kx}$), trigonométrie (M02 : $\cos 0$, $\sin 0$). **Test 30 s :** $(e^{-2x})'$ → $-2e^{-2x}$ sans hésiter ; $(\sin 3x)'$ → $3\cos 3x$.

**Plan B — le plus dur (ne plus se tromper de signe/formule) :** fiche de 3 lignes recopiée en tête d'exercice : ① $y' + ay = 0$ → $Ce^{-ax}$ ② $y' + ay = b$ → $Ce^{-ax} + b/a$ ③ $y'' + \omega^2 y = 0$ → $A\cos\omega x + B\sin\omega x$. Puis : normaliser → recopier $a$/$\omega$ → CI → **vérifier** (redériver + réinjecter). Zéro réflexion, 100 % de réussite.

**Fiche réflexes :** *inconnue = fonction · normaliser d'abord · $a$ dans l'exposant ($-ax$) · $b/a$ = équilibre · $\omega = \sqrt{\ } $ · 2 CI pour l'ordre 2 · vérifier toujours.*
