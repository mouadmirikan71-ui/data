---
chapitre: "14 - Probabilités"
unite: "S4 - Dénombrement et probabilités"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2025 Normale Ex.3 (réel, SP : urne + binomiale) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 14 — Probabilités

> 📋 **Exigible au bac** : $p(A \cup B) = p(A) + p(B) - p(A \cap B)$ ; équiprobabilité $cardA/card\Omega$ (M13 !) ; $p_A(B) = \frac{p(A\cap B)}{p(A)}$ ; arbre (produit sur un chemin, somme des chemins) ; probas totales ; indépendance $p(A\cap B) = p(A)p(B)$ ; binomiale $B(n,p)$ : $p(X=k) = C_n^k p^k(1-p)^{n-k}$, $E(X) = np$.

## 1. Accroche — le test médical qui ment (presque) 🧪

Un test détecte une maladie à 99 %… mais si 1 personne sur 10 000 est malade, un positif n'est presque sûrement pas malade ! Pourquoi ? Parce que **« sachant que » change l'univers** : on ne compte plus sur tout le monde, seulement sur les positifs. Les probabilités conditionnelles, c'est l'art du **zoom** : changer de loupe ($p_A$) et tout change. Ce chapitre = savoir zoomer (conditionnelles), tout balayer (totales) et répéter (binomiale).

> بالدارجة : تحليلة كتكشف المرض بـ 99%... ولكن إلا كان مريض واحد في 10.000، اللي خرجاتو إيجابية غالباً **ما مريضش** ! علاش ؟ حيت **«بشرط» كتبدّل الكون** : ما كنحسبوش على كولشي، غير على الإيجابيين. الاحتمالات الشرطية = فنّ **التكبير (الزوم)** : بدّل العدسة وكلشي كيتبدّل.

## 2. Résumé du cours (exigible au bac)

**Bases.** Univers $\Omega$, événement $A \subset \Omega$ ; $p(\bar{A}) = 1 - p(A)$ ; $\boxed{p(A \cup B) = p(A) + p(B) - p(A \cap B)}$ (on retire la double compte !) ; $A, B$ **incompatibles** ($A \cap B = \varnothing$) → $p(A \cup B) = p(A) + p(B)$. **Équiprobabilité :** $\boxed{p(A) = cardA/card\Omega}$ — le numérateur ET le dénominateur sont des **dénombrements** (M13 : même modèle des deux côtés !).

**Conditionnelles + arbre.** $\boxed{p_A(B) = \frac{p(A\cap B)}{p(A)}}$ ($p(A) > 0$) : « proba de $B$ SACHANT $A$ ». **Arbre pondéré** : proba d'un chemin = **produit** des branches ; $p(A\cap B) = p(A) \times p_A(B)$. **Formule des probas totales** (partition $A_1, \dots, A_n$) : $\boxed{p(B) = \sum p(A_i)\,p_{A_i}(B)}$ — « tous les chemins qui mènent à $B$ ». **Indépendance :** $A, B$ indépendants $\iff \boxed{p(A\cap B) = p(A)p(B)} \iff p_A(B) = p(B)$ (« $A$ n'apprend rien sur $B$ »).

**Loi binomiale $B(n,p)$.** Schéma de Bernoulli : **3 conditions** — (1) $n$ épreuves **identiques**, (2) **indépendantes**, (3) **2 issues** (succès $p$ / échec $1-p$). $X$ = nombre de succès : $\boxed{p(X=k) = C_n^k\,p^k(1-p)^{n-k}}$, $\boxed{E(X) = np}$. Lecture : $C_n^k$ chemins gagnants × proba d'un chemin ($p^k(1-p)^{n-k}$). Questions types : $p(X = k)$, $p(X \geq 1) = 1 - p(X=0) = 1-(1-p)^n$ (complémentaire !), $p(X \leq 1) = p(X=0)+p(X=1)$.

**Réflexes bac :** « sachant que » → conditionnelle (restreindre !) ; « au moins un » → $1 - p(aucun)$ ; tirages **avec remise** → Bernoulli/binomiale possible ; **sans remise** → PAS binomiale (hypergéométrique, hors programme : dénombrer avec $C$ !).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الأساس :** الكون $\Omega$، الحدث $A$ ؛ $p(\bar{A}) = 1 - p(A)$ ؛ $p(A \cup B) = p(A) + p(B) - p(A \cap B)$ (نقص العدّ المزدوج !). **تساوي الاحتمال :** $p(A) = cardA/card\Omega$ — البسط **و** المقام عدّ (M13 : نفس النموذج في الجهتين !).

**الشرطية + الشجرة :** $p_A(B) = \frac{p(A\cap B)}{p(A)}$ : احتمال $B$ **بشرط** $A$. **الشجرة الموزونة** : احتمال المسار = **جداء** الأغصان ؛ $p(A\cap B) = p(A) \times p_A(B)$. **الاحتمالات الكلية** : $p(B) = \sum p(A_i)\,p_{A_i}(B)$ — «كاع الطرق اللي كتوصّل لـ $B$». **الاستقلال :** $p(A\cap B) = p(A)p(B) \iff p_A(B) = p(B)$ («$A$ ما كتعلّم والو على $B$»).

**القانون ثنائي الحد $B(n,p)$ :** مخطط برنولي : **3 شروط** — (1) $n$ تجارب **متماثلة**، (2) **مستقلة**، (3) **نتيجتين** (نجاح $p$ / فشل $1-p$). $X$ = عدد النجاحات : $p(X=k) = C_n^k\,p^k(1-p)^{n-k}$، $E(X) = np$. القراءة : $C_n^k$ طرق رابحة × احتمال الطريق. الأسئلة : $p(X = k)$ ؛ $p(X \geq 1) = 1-(1-p)^n$ (المتمم !).

**ردود فعل الباك :** «بشرط» ← شرطية (ضيّق الكون !) ؛ «على الأقل واحد» ← $1 - p(حتى واحد)$ ؛ السحب **مع الإرجاع** ← برنولي ممكن ؛ **بلا إرجاع** ← ماشي ثنائي الحد (عدّ بـ $C$ !).

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — الاحتمال = كسر عدّ.** $p(A) = \frac{\text{الحالات المفضلة}}{\text{الحالات الممكنة}}$ — البسط والمقام بجوج **عدّ (M13)** وبنفس النموذج ! صندوق : 3 حمر + 2 خضر، سحب 2 آني : $p(\text{2 حمر}) = \frac{C_3^2}{C_5^2} = \frac{3}{10}$. **الغلطة الوحيدة : البسط بنموذج والمقام بنموذج آخر** (البسط $A$ والمقام $C$ = كارثة). القاعدة : *نفس السحب، نفس الصيغة، فوق وتحت.*

**الخطوة 2 — «بشرط» = بدّل الكون.** $p_A(B)$ : نسى $\Omega$ — الكون الجديد هو $A$ ! مثال : نرد، $A$ = «زوجي» $\{2,4,6\}$، $B$ = «> 3» : $p_A(B) = \frac{|\{4,6\}|}{|\{2,4,6\}|} = \frac{2}{3}$ (ماشي $\frac{3}{6}$ !). **الصيغة $p(A\cap B)/p(A)$ هي هاد التضييق مكتوب رياضياً.**

**الخطوة 3 — الشجرة : اضرب في الطريق، اجمع الطرق.** مصنع : 60% آلة 1 (2% معيب)، 40% آلة 2 (5% معيب). $p(\text{معيب}) = 0,6\times0,02 + 0,4\times0,05 = 0,032$ (الاحتمالات الكلية : طريق 1 + طريق 2). **ارسم ديما الشجرة** — التمرين كيتحلّ بوحدو.

**الخطوة 4 — ثنائي الحد : تحقق من الشروط الثلاثة.** «نرمي قطعة 5 مرات، $p(\text{3 وجيه})$ ؟» : نفس التجربة ✓، مستقلة ✓، نتيجتين ✓ ← $B(5, \frac{1}{2})$ ← $C_5^3(\frac{1}{2})^5 = \frac{10}{32}$. **إلا شرط ناقص (بلا إرجاع !)، ماشي ثنائي الحد** — رجع للعدّ المباشر.

**الخطوة 5 — «على الأقل واحد» = $1 - p(0)$.** $p(X \geq 1) = 1 - (1-p)^n$ (المتمم : صفر نجاح). و $p(X \leq k)$ الصغيرة = اجمع $p(X=0) + \cdots + p(X=k)$. **القاعدة : المتمم اللول، الجمع من بعد.**

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Univers $\Omega$ | الكون | tous les cas possibles |
| $p(A \cup B)$ | احتمال الاتحاد | $p(A)+p(B)-p(A\cap B)$ |
| Équiprobabilité | تساوي الاحتمال | $cardA/card\Omega$ (même modèle !) |
| $p_A(B)$ conditionnelle | الشرطي | $p(A\cap B)/p(A)$ — zoom sur $A$ |
| Arbre pondéré | الشجرة الموزونة | produit sur chemin, somme des chemins |
| Probas totales | الاحتمالات الكلية | partitionner puis sommer |
| Indépendance | الاستقلال | $p(A\cap B) = p(A)p(B)$ |
| Binomiale $B(n,p)$ | ثنائي الحد | $C_n^k p^k(1-p)^{n-k}$, $E = np$ |

## 6. FAQ du chapitre

**1. $p(A\cap B)$ ou $p_A(B)$ ?** $p(A\cap B)$ = « les deux » (chemin complet : $p(A)\times p_A(B)$). $p_A(B)$ = « $B$ sachant $A$ » (une branche, univers réduit). / التقاطع = «بجوج» (الطريق كامل). الشرطي = غصن واحد (كون مضيّق).

**2. Indépendants ou incompatibles ?** **Indépendants** : $p(A\cap B) = p(A)p(B)$ (l'un n'informe pas l'autre — peuvent coexister !). **Incompatibles** : $A\cap B = \varnothing$ (ne coexistent JAMAIS — très dépendants !). Quasi-opposés ! / المستقلة كتتعايش، المتنافية عمرها ما كتتعايش — شبه متضادتين !

**3. Pourquoi $E(X) = np$ ?** En moyenne, proportion $p$ de succès sur $n$ épreuves : $n$ fois $p$. (Ex : 100 lancers à $p = 1/2$ → ~50 piles.) / معدل $p$ نجاح في $n$ تجربة : $n$ مرات $p$.

**4. Sans remise : pourquoi pas binomiale ?** $p$ CHANGE à chaque tirage (composition de l'urne modifiée) → épreuves ni identiques ni indépendantes → dénombrer ($C$) ! / $p$ كيتبدّل كل سحبة ← ماشي متماثلة ← عدّ مباشر !

**5. Arbre ou formule ?** Arbre : 2-3 étapes, conditionnelles en cascade (visuel, sans erreur). Formule : $p_A(B)$ isolé, binomiale (calcul direct). Au bac : arbre d'abord, formules ensuite. / الشجرة للمراحل، الصيغة للحساب المباشر — الشجرة اللولة.

**6. $p(X \geq 2)$ avec $n = 10$ ?** Complémentaire : $1 - p(X=0) - p(X=1)$ (3 termes au lieu de 9 !). / المتمم : $1 - p(0) - p(1)$ (3 حدود بلا 9 !).

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **Modèles mixtes ($A$ en haut, $C$ en bas)** : $p =$ favorable/possible EXIGE le même modèle des 2 côtés. Tout $A$ ou tout $C$ !
- 🪤 **« Sachant que » ignoré** : $p_A(B)$ avec l'univers ENTIER = faux. Restreindre à $A$ (diviser par $p(A)$).
- 🪤 **Binomiale sans vérifier** : « 5 boules sans remise, $p(3$ rouges$)$ » via $C_5^3p^3(1-p)^2$ = FAUX ($p$ change !). Sans remise → $C$ direct.
- 🪤 **$p(X \geq 1) = p(X=1)$** : « au moins 1 » = $1 + 2 + \cdots + n$ ! Complémentaire : $1 - p(X=0)$.
- Mots-clés : *même modèle haut/bas, sachant = restreindre, arbre (× chemin, + chemins), binomiale : 3 conditions, au moins = $1-$aucun.*

## 8. Sources de ce chapitre

- National Maths SX 2025 Normale Ex.3 (réel, SP) : urne 4B+2N (P(A) = 2/5, P(B) = 7/15, non-indépendance, B(3,2/5)) — https://etude-generale.com/correction-dexamen-national-2025-math-science-physique/ ; + synthèse prof ; moteur M13.

## 9. Le « pourquoi » profond — pourquoi diviser, pourquoi multiplier 🔬

**Pourquoi $p_A(B) = p(A\cap B)/p(A)$ ?** « Sachant $A$ » = ne garder que les mondes où $A$ est vrai. Dans ce sous-univers, la part de $B$ = (part de $A$-et-$B$) / (part de $A$) : renormaliser pour que $p_A(A) = 1$ (dans le zoom, $A$ est certain !). **Conditionner = renormaliser** — c'est le geste des tests médicaux, des sondages, du machine learning (Bayes !).

**Pourquoi produit sur un chemin, somme sur les chemins ?** Produit : $p(A\cap B) = p(A)\times p_A(B)$ — enchaîner deux filtres multiplie les proportions (1/2 des élèves sont des filles, 1/3 d'entre elles portent des lunettes → 1/6). Somme : des chemins disjoints vers $B$ partitionnent $B$ → addition (cas disjoints !). **L'arbre exécute les probas totales visuellement.**

**Pourquoi $C_n^k$ dans la binomiale ?** $p^k(1-p)^{n-k}$ = proba d'UN ordre fixé (ex : SSSE…E). Mais les $k$ succès occupent $k$ places quelconques parmi $n$ : $C_n^k$ placements disjoints → multiplier. **Binomiale = Newton probabiliste** : $(p + (1-p))^n = \sum C_n^k p^k(1-p)^{n-k} = 1$ — la distribution EST le binôme de M13 !

**Liens croisés :** M13 — tout quotient de proba = quotient de dénombrements ; Newton $(p+q)^n$ = normalisation de la binomiale ; SVT — génétique (croisements = arbres ! $1/4$, $3/4$ : M14 déguisée) ; PC — désintégrations, erreurs de mesure : Bernoulli partout ; culture — paradoxe de Monty Hall, tests médicaux : conditionnelles contre-intuitives.

## 10. Les 3 confusions qui coûtent des points 😵

**1. « $A$ et $B$ indépendants car disjoints. »** Inverse ! Disjoints = incompatibles = JAMAIS ensemble = dépendance maximale (si $A$ est vrai, $B$ est faux à coup sûr !). **Le déclic :** *indépendants = indifférents (peuvent coexister) ; incompatibles = ennemis (jamais ensemble).* Teste : $p(A\cap B) = 0 \neq p(A)p(B)$ → pas indépendants (sauf proba nulle).

**2. « $p_A(B) = p(A\cap B)$. »** Oubli de la renormalisation ($/p(A)$). **Le déclic :** *$p_A(A)$ doit valoir 1 (dans le zoom, $A$ est certain) — sans division, $p(A\cap A) = p(A) < 1$ : absurde.* La division n'est pas décorative, elle recale le zoom à 1.

**3. « Tirages sans remise → binomiale avec $p$ moyen. »** Il n'y a pas de « $p$ moyen » : la binomiale exige $p$ CONSTANT. **Le déclic :** *remise = mémoire effacée ($p$ fixe) = Bernoulli ; sans remise = mémoire ($p$ change) = hypergéométrique = dénombrer.* Le mot « remise » décide de TOUTE la méthode.

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** dénombrement M13 ($C_n^p$, test d'échange), fractions/%, ensembles ($\cup$, $\cap$, $\bar{A}$). **Test 30 s :** $C_6^2 = 15$ ; $p(\bar{A})$ si $p(A) = 0,3$ → $0,7$ ; $0,5^3 = 0,125$.

**Plan B — le plus dur (reconnaître conditionnelle vs binomiale vs directe) :** ① « sachant que » ou 2 étapes dépendantes → **arbre + conditionnelles** ; ② répétition identique indépendante à 2 issues → **binomiale** (écrire $n$, $p$, $X$ !) ; ③ tirage unique sans « sachant » → **directe** $cardA/card\Omega$ (M13). Si hésitation : dessiner l'arbre — il révèle la structure à coup sûr.

**Fiche réflexes :** *même modèle haut/bas · sachant = zoom ($/p(A)$) · arbre : × chemin, + chemins · binomiale : 3 conditions + $C_n^k$ · au moins = $1-$aucun.*
