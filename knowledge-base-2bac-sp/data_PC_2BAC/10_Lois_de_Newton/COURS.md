---
chapitre: "10 - Lois de Newton"
unite: "Physique S2 - Mécanique"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (style national PC) - verbatim en backfill"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 10 — Lois de Newton

> 📋 **Exigible au bac (cadre de référence)** : référentiels (galiléens), 1ère loi (inertie), 2ème loi
> ($\sum\vec{F} = m\vec{a}$, PFD), 3ème loi (actions réciproques), bilan de forces, projection — **chapitre central**.

## 1. Accroche — le bus qui freine 🚌

**FR :** Le bus freine brutalement : ton corps part EN AVANT. Personne ne t'a poussé ! C'est l'INERTIE (1ère loi) :
ton corps « veut » garder sa vitesse, et c'est le bus qui a changé la sienne. Deuxième scène : tu pousses une
voiture en panne (lourde !) vs un caddie (léger !) : même poussée, accélérations très différentes — c'est la 2ème
loi ($\vec{a} = \sum\vec{F}/m$ : la masse RÉSISTE). Tout le chapitre = 3 lois qui gouvernent TOUT mouvement
(ponts, fusées, planètes, ballons) + la méthode (bilan → PFD → projection → équations horaires).

**بالدارجة:** الكار فرمل بالزربة: جسمك مشى **للقدام** — حتى واحد ما دفعك! هادا هو **القصور** (القانون 1): جسمك «بغا» يحافظ على سرعتو، والكار هو اللي بدل سرعتو! المشهد 2: دفعتي طوموبيل خاسرة (ثقيلة!) ضد كروسة (خفيفة!): نفس الدفعة، تسارع مختلف بزاف — هادا القانون 2 ($\vec{a} = \sum\vec{F}/m$: الكتلة **كتقاوم**)! هاد الفصل = 3 قوانين كيحكمو **أي حركة** + المنهجية (الجرد ← المبدأ ← الإسقاط ← المعادلات الزمنية)!

## 2. Résumé du cours (exigible au bac)

### 2.1 Référentiels — galiléen ou pas ?
- Référentiel = objet de référence + horloge (terrestre, géocentrique, héliocentrique... **Galiléen** : où le
  principe d'inertie est vérifié (terrestre ≈ galiléen pour les mouvements courants ; le bus qui freine NE l'est PAS !).
- Les lois de Newton ne s'appliquent QUE dans un référentiel galiléen (à PRÉCISER en début d'exercice !).

### 2.2 1ère loi — principe d'inertie
- $\boxed{\sum\vec{F} = \vec{0} \iff \vec{v}_G = \text{Cte}}$ (immobile ou MRU du centre d'inertie).
- Sens : sans force, on garde sa vitesse (état « naturel » = MRU, PAS le repos !). La masse = mesure de l'inertie.

### 2.3 2ème loi — PFD (le cœur du chapitre)
- $\boxed{\sum\vec{F}_{ext} = m\vec{a}_G}$ (dans un référentiel galiléen, système = centre d'inertie G).
- Méthode : (1) système + référentiel (galiléen !) ; (2) BILAN des forces (schéma !) ; (3) PFD vectoriel ;
  (4) PROJECTION sur les axes ($x,y$) → équations scalaires ; (5) primitiver → $\vec{v}(t)$, $\overrightarrow{OM}(t)$.

### 2.4 3ème loi — actions réciproques
- $\boxed{\vec{F}_{A/B} = -\vec{F}_{B/A}}$ : même droite, sens opposés, même norme — exercées sur des SYSTÈMES
  DIFFÉRENTS (elles ne s'annulent PAS dans un bilan !).
- Applications : propulsion (fusée pousse les gaz ⟸⟹ gaz poussent la fusée), marche, réaction du support.

### 2.5 Forces usuelles (le catalogue)
- Poids : $\vec{P} = m\vec{g}$ ($g \approx 9,8\,m/s^2$, vertical vers le bas, appliqué en G).
- Réaction $\vec{R} = \vec{N}+\vec{f}$ : normale $\vec{N}$ (⊥ support) + frottement $\vec{f}$ (∥, opposé au mouvement ;
  $f = \mu N$ si glissement, loi de Coulomb simplifiée).
- Tension $\vec{T}$ (fil/câble : direction du fil, sens « tire »), poussée d'Archimède (fluides), force électrique
  $\vec{F} = q\vec{E}$, forces de rappel ($-k\vec{x}$ — ch.14-15).

### 2.6 Applications directes (classiques)
- **Chute libre** (sans air) : PFD → $\vec{a} = \vec{g}$ (indépendant de $m$ !) → $v = gt+v_0$, $y = \frac{1}{2}gt^2+v_0t+y_0$.
- **Plan incliné** (angle $\alpha$, sans frottement) : $a = g\sin\alpha$ (projection sur la pente !) ; avec frottement :
  $a = g(\sin\alpha-\mu\cos\alpha)$.
- **Poulie** (Atwood simplifié : $m_1$ sur table + $m_2$ suspendue, fil inextensible) : $a = \frac{m_2}{m_1+m_2}g$.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** نيوتن قال: **القوى كتبدل السرعة** (ماشي كتخلقها)! بلا قوى ← السرعة ثابتة (القصور). بقوى ← التسارع = القوى مقسومة على الكتلة!

1. **القانون 1 (القصور):** $\sum\vec{F} = 0$ ← السرعة ثابتة (سكون ولا مستقيمية منتظمة)! الحالة «الطبيعية» هي الثبات — ماشي السكون! الكتلة = مقياس العناد (الثقيلة صعيبة تحركها وصعيبة تحبسها)!
2. **القانون 2 (المبدأ):** $\sum\vec{F} = m\vec{a}$ — **أهم معادلة فالميكانيك**! المنهجية: الجملة + المرجع (عطالي!) ← جرد القوى (رسم!) ← المبدأ شعاعياً ← **الإسقاط** على المحاور ← معادلات ← كامل بالتكامل ($v$ ومن بعد $x$)!
3. **القانون 3 (الفعل ورد الفعل):** $\vec{F}_{A/B} = -\vec{F}_{B/A}$ — نفس الشدة، عكس الاتجاه، ولكن على **جملتين مختلفين** (ما كيتلاشاوش فالجرد!). الصاروخ كيدفع الغازات ← الغازات كيدفعو الصاروخ!
4. **القوى المعتادة:** الثقل ($m\vec{g}$ للتحت)، رد الفعل (عمودي + احتكاك ضد الحركة)، التوتر (كيجر فاتجاه الخيط). الجرد الناقص = المعادلة غالطة = التمرين ضايع!
5. **التطبيقات:** السقوط الحر ($a = g$ — مستقلة على الكتلة! الريشة والحديد فالفراغ كيطيحو كيف كيف!)، المستوى المائل ($a = g\sin\alpha$)، البكرة ($a = \frac{m_2}{m_1+m_2}g$)!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — أي تمرين ميكانيك بدا بهاد الجملة:** «الجملة: (الجسم)، المرجع: أرضي مفترض عطالي، الجرد: ...» — هاد المقدمة فيها نقط (المنهجية منقطة!) وما كتاخذش 30 ثانية!

**الخطوة 2 — الرسم قبل المعادلة!** رسم الجسم + **جميع** القوى بأسهم مسماة ($\vec{P}$, $\vec{N}$, $\vec{f}$, $\vec{T}$...) + المحاور ($x$ فاتجاه الحركة غالباً!). 90 % ديال أغلاط الإسقاط من رسم ناقص ولا محاور عوجة!

**الخطوة 3 — الإسقاط: القاعدة الذهبية.** المركبة = الشدة × $\cos$ (الزاوية مع المحور)! الثقل على مستوى مائل $\alpha$: $P_x = mg\sin\alpha$ (مع المنحدر)، $P_y = -mg\cos\alpha$ (عمودي). تحقق: إلا $\alpha = 0$ ← $P_x = 0$ ✔ (مستوى أفقي!)، إلا $\alpha = 90°$ ← $P_x = mg$ ✔ (سقوط حر!) — **الحالات الحدية كتكشف الغلط**!

**الخطوة 4 — من التسارع للحركة: كامل جوج مرات!** $a(t)$ ← (تكامل + $v_0$) ← $v(t)$ ← (تكامل + $x_0$) ← $x(t)$! الشروط البدئية ($v_0$, $x_0$) من النص — اللي نساهم خسر الثوابت!

**الخطوة 5 — الأخطاء القاتلة:** مرجع ماشي عطالي (الباص اللي كيفرمل!)؛ قوة ناقصة فالجرد (الاحتكاك!)؛ إسقاط بـ $\sin$ بدل $\cos$؛ $\vec{F}_{A/B}$ و$\vec{F}_{B/A}$ فـ **نفس** الجرد (مستحيل!)؛ الكتلة بالغرام (SI: **kg**!)؛ $g = 10$ بلا ما يقول النص ($9,81$ إلا ما تحددش — شوف النص!)!

## 5. Définitions & formules clés (FR + Darija)

| Notion FR (LaTeX) | Énoncé FR | بالدارجة |
|---|---|---|
| 1ère loi : $\sum\vec{F} = 0 \iff \vec{v}$ Cte | Inertie : on garde sa vitesse sans force | القصور: بلا قوى السرعة ثابتة |
| PFD : $\sum\vec{F} = m\vec{a}_G$ | La loi maîtresse (réf. galiléen !) | القانون الكبير |
| 3ème loi : $\vec{F}_{A/B} = -\vec{F}_{B/A}$ | Réciprocité (2 systèmes ≠ !) | الفعل ورد الفعل |
| $\vec{P} = m\vec{g}$ | Poids ($g \approx 9,8\,m/s^2$) | الثقل |
| $a = g\sin\alpha$ | Plan incliné sans frottement | التسارع فالمستوى المائل |
| $v^2-v_0^2 = 2a(x-x_0)$ | Formule SANS le temps (MRUV) | الصيغة بلا زمن! |

## 6. FAQ du chapitre

**Q1. Pourquoi préciser « référentiel galiléen » ?**
Parce que le PFD est FAUX dans un bus qui freine (ton corps accélère « tout seul » !). Le national exige la phrase :
« référentiel terrestre supposé galiléen » — c'est le ticket d'entrée du PFD.
بالدارجة: حيت المبدأ غالط فالمرجع اللي كيتسارع (الباص!)! الجملة «مرجع أرضي مفترض عطالي» هي **تذكرة الدخول** ديال المبدأ!

**Q2. Inertie = immobilité ?**
NON ! Inertie = garder sa VITESSE (qui peut être $200\,km/h$ !). Un satellite sans force garde son MRU éternellement.
Le repos n'est qu'un cas particulier ($v = 0$).
بالدارجة: لا! القصور = الحفاظ على **السرعة** (وخا 200 km/h)! السكون غير حالة خاصة ($v = 0$)!

**Q3. Pourquoi projeter ? On ne peut pas garder les vecteurs ?**
Parce que $m\vec{a} = \sum\vec{F}$ = 2-3 équations scalaires cachées ! La projection les EXTRAIT (une par axe).
Sans projection, pas d'équation calculable. L'axe $x$ dans le sens du mouvement simplifie tout.
بالدارجة: حيت المعادلة الشعاعية = 2-3 معادلات مخبية! الإسقاط كيخرجهم (وحدة لكل محور)! والمحور $x$ فاتجاه الحركة كيسهل كلشي!

**Q4. Action-réaction : pourquoi elles ne s'annulent pas ?**
Parce qu'elles s'appliquent à des OBJETS DIFFÉRENTS (gaz vs fusée) ! On ne peut additionner que des forces sur le
MÊME système. Dans un bilan, UNE seule des deux apparaît.
بالدارجة: حيت كيتطبقو على **أجسام مختلفة** (الغازات ضد الصاروخ)! الجمع غير للقوى على نفس الجملة! فالجرد كتبان وحدة منهم!

**Q5. $v^2-v_0^2 = 2a\Delta x$ : quand l'utiliser ?**
Quand le temps est ABSENT de la question (« quelle vitesse après 100 m ? »). Elle vient d'éliminer $t$ entre
$v = at+v_0$ et $x = \frac{1}{2}at^2+v_0t+x_0$. Évite un système !
بالدارجة: ملي الزمن **غايب** من السؤال («شحال السرعة من بعد 100 م؟»)! كتجي من حذف $t$ — كتوفر عليك جملة معادلات!

**Q6. $g = 9,81$ ou $10$ ?**
Ce que dit L'ÉNONCÉ ! Par défaut (rien précisé) : $g = 9,81\,m/s^2$ (valeur officielle). Si l'énoncé dit $g = 10$,
utilise 10. Ne JAMAIS inventer.
بالدارجة: اللي قال النص! إلا ما قال والو: $9,81$. إلا قال 10: خدم بـ 10. وعمرك تخترع!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : « système + référentiel terrestre supposé galiléen » ; bilan COMPLET + schéma ;
« d'après la 2ème loi de Newton : $\sum\vec{F} = m\vec{a}_G$ » ; projection explicite ; conditions initiales ;
AN en SI ($kg$, $m$, $s$) ; $\boxed{\text{résultat}}$.
**Erreurs fréquentes** : référentiel non précisé ❌ ; force oubliée (frottement !) ❌ ; $\sin/\cos$ inversés ❌ ;
action+réaction dans le même bilan ❌ ; masse en $g$ ❌ ; $v_0$/$x_0$ oubliés ❌.

## 8. Sources de ce chapitre
- Synthèse prof (cours + exercices type-bac) : rédaction originale pour cette base, 2026-09-15.
- Backfill prévu : questions Newton verbatim du national PC (sessions 2023-2025 prioritaires).

## 9. Le « pourquoi » profond — $F = ma$ gouverne le monde 🔬

**Pourquoi la 1ère loi n'est pas un cas particulier de la 2ème ? (le statut du référentiel)**
$\sum F = 0 \Rightarrow a = 0$ SE DÉDUIT de la 2ème... mais la 1ère loi fait PLUS : elle DÉFINIT les référentiels
galiléens (ceux où elle est vraie) ! Sans elle, la 2ème s'appliquerait n'importe où, même dans le bus qui freine
(où elle est FAUSSE). La 1ère = le MODE D'EMPLOI (« n'utiliser la 2ème que ici »), la 2ème = la MACHINE à calculer.
C'est pour ça que le national exige la phrase sur le référentiel : elle active la garantie !

**Pourquoi $\vec{a} = \sum\vec{F}/m$ ? (la masse comme résistance)**
Réécrite $\vec{a} = \frac{1}{m}\sum\vec{F}$ : à force égale, l'objet 2× plus lourd accélère 2× moins. La masse =
le COEFFICIENT DE RÉSISTANCE au changement de vitesse (inertie QUANTIFIÉE). C'est le même pattern que TOUTE la
physique : effet = cause/résistance ($I = U/R$ ! $a = F/m$ ! $v = F/k$ (frottement) !). Retiens le pattern, pas
(que) la formule.

**Pourquoi chute libre $\Rightarrow a = g$ quelle que soit $m$ ? (le miracle de Galilée)**
PFD : $m\vec{g} = m\vec{a}$ → les $m$ SE SIMPLIFIENT → $\vec{a} = \vec{g}$ ! La masse « qui pèse » (dans $mg$)
et la masse « qui résiste » (dans $ma$) sont ÉGALES — coïncidence profonde (principe d'équivalence d'Einstein !).
Conséquence : marteau + plume tombent ensemble (sur la Lune : vérifié en 1971, Apollo 15 !). Les $m$ qui se
simplifient = signature d'un phénomène UNIVERSEL.

**Pourquoi action = -réaction ? (la conservation de la quantité de mouvement)**
Si A pousse B sans que B repousse A, le système {A+B} créerait du mouvement EX NIHILO (perpetuum mobile !).
La 3ème loi EST la conservation de $\vec{p}_{tot}$ déguisée : ce que A donne à B, B le « rend » à A en sens inverse.
Propulsion, marche, recul du fusil : toujours $\vec{p}$ qui se conserve. (Quantité de mouvement : prolongement
naturel — cf. terminale/supérieur.)

**Ponts :** chutes et projectiles ch.11-12 (APPLICATIONS directes : le PFD projeté !) ; oscillateurs ch.14-15
(PFD + $-kx$ = EDP !) ; satellites ch.28 (PFD + gravitation : Kepler !) ; électricité (analogie $F = ma \leftrightarrow
U = RI$ : cause = résistance × effet) ; Maths EDP ch.10 (primitiver $a(t)$ !) ; SVT muscle ch.02 ($F = ma$ : la force
du muscle ACCÉLÈRE les segments !).

> بالدارجة: علاش القانون 1 ماشي حالة خاصة من 2؟ حيت هو اللي **كيعرف المراجع العطالية** (فين المبدأ خدام)! بلا بيه غادي تستعمل المبدأ فالباص اللي كيفرمل (فين هو غالط)! القانون 1 = **دليل الاستعمال**، والقانون 2 = **آلة الحساب**! وعلاش السقوط الحر مستقل على الكتلة؟ حيت $m$ اللي **كتثقل** و$m$ اللي **كتقاوم** متساويين — كيتحيدو! المطرقة والريشة كيطيحو كيف كيف (تجربة أبولو 15 فالقمر!)! والفعل ورد الفعل = **حفاظ كمية الحركة** متنكر: اللي عطاه A لـ B، B كيردو بالعكس!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $\sin\alpha$ vs $\cos\alpha$ sur le plan incliné — le test des cas limites.**
*Le clic :* $P_x = mg\sin\alpha$ (le long de la pente) ou $mg\cos\alpha$ ? TESTE : $\alpha = 0$ (plan horizontal) →
$P_x$ doit valoir 0 → c'est $\sin$ ($0$) ! $\alpha = 90°$ (mur vertical = chute) → $P_x = mg$ → $\sin 90 = 1$ ✔.
Les CAS LIMITES tranchent en 5 secondes — utilise-les à CHAQUE projection douteuse.
بالدارجة: $P_x = mg\sin\alpha$ ولا $\cos$؟ جرب: $\alpha = 0$ (أفقي) ← $P_x = 0$ ← هو **$\sin$**! $\alpha = 90°$ (سقوط) ← $mg$ ← $\sin 90 = 1$ ✔! **الحالات الحدية** كتحسم فـ 5 ثواني — استعملها فكل إسقاط مشكوك!

**C2. Action-réaction dans le MÊME bilan — l'erreur logique.**
*Le clic :* le livre appuie sur la table ($\vec{F}_{livre/table}$) ET la table soutient le livre
($\vec{F}_{table/livre}$) : paire réciproque ! Mais le bilan DU LIVRE ne contient QUE $\vec{F}_{table/livre}$
(+ le poids). Mettre les deux = compter 2 fois la même interaction = bilan faux. Règle : « bilan de X = forces
SUBIES par X, point ».
بالدارجة: الكتاب كيضغط على الطبلة **و** الطبلة كتهز الكتاب — زوج متبادل! ولكن جرد **الكتاب** فيه غير قوة الطبلة (+ الثقل)! اللي دارهم بجوج حسب نفس التفاعل جوج مرات! القاعدة: «جرد X = القوى اللي **كتعاني** منها X»!

**C3. « $v = 0$ donc $a = 0$ » — FAUX ! (le sommet du lancer)**
*Le clic :* balle lancée vers le haut : au SOMMET, $v = 0$ mais $a = -g$ (le poids agit TOUJOURS !). Vitesse nulle ≠
accélération nulle : $a$ = la PENTE de $v$, pas $v$ ! La balle s'arrête UN INSTANT puis repart (la pente de $v$
ne s'annule pas). Retiens : « $a = 0 \iff v$ CONSTANTE (pas nulle !) ».
بالدارجة: الكرة المقذوفة للفوق: فالقمة $v = 0$ ولكن $a = -g$ (الثقل خدام ديماً)! السرعة صفر ≠ التسارع صفر: $a$ هو **الميل** ديال $v$! القاعدة: «$a = 0$ ⟺ السرعة **ثابتة** (ماشي معدومة!)»!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Vecteurs (2nde/1ère) : somme, projection, $\cos/\sin$ — le langage du chapitre.
2. Primitives (Maths : $a \to v \to x$) — passer de l'accélération au mouvement.
3. Trigonométrie : $\sin/\cos$ d'angles usuels + complémentaires ($\sin\alpha = \cos(90-\alpha)$).
4. Unités SI : $kg$, $m$, $s$, $N = kg\cdot m/s^2$ (vérifier l'homogénéité : $F/m$ en $m/s^2$ ✔ !).

**Si la projection bloque — plan B :**
Le mur : « c'est $\sin$ ou $\cos$ ? » + axes mal choisis. **Fallback officiel** : (1) TOUJOURS mettre $x$ dans le
sens du mouvement (ça annule une composante de $a$ !) ; (2) pour chaque force, dessiner le TRIANGLE ($F$, $F_x$,
$F_y$) et lire : adjacent $= \cos$, opposé $= \sin$ ; (3) VALIDER par les cas limites ($\alpha = 0$, $90°$) ;
(4) si vraiment bloqué : écrire le PFD vectoriel + bilan juste (points partiels !) et admettre les projetées.
بالدارجة: إلا وحلتي فالإسقاط: حط $x$ **فاتجاه الحركة** ديماً! ولكل قوة رسم المثلث (المجاور $= \cos$، المقابل $= \sin$)! وتأكد بالحالات الحدية! وإلا بقات حابسة: كتب المبدأ الشعاعي والجرد (نقط جزئية!) وقبل المسقطات!
