---
chapitre: "12 - Mouvements de projectiles"
unite: "Physique S2 - Mécanique"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (style national PC) - verbatim en backfill"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 12 — Mouvements de projectiles

> 📋 **Exigible au bac** : projectile dans $\vec{g}$ (trajectoire, portée, flèche), particule chargée dans
> $\vec{E}$ uniforme (déflexion), particule chargée dans $\vec{B}$ (mouvement circulaire uniforme, cyclotron).

## 1. Accroche — du ballon au cyclotron ⚽⚛️

**FR :** Un footballeur frappe : le ballon décrit une PARABOLE et retombe 40 m plus loin. Un écran cathodique
défléchit des électrons : MÊME parabole (avec $\vec{E}$ au lieu de $\vec{g}$) ! Et dans un cyclotron, des protons
tournent en SPIRALE à 99 % de $c$ pour soigner des cancers. Trois machines, UNE méthode : PFD projeté (ch.10 !) →
équations horaires → trajectoire. Tout le chapitre = le PFD qui dessine des courbes.

**بالدارجة:** الكوايري ضرب الكرة: كترسم **قطع مكافئ** وكطيح بعيد! الشاشة القديمة كتحرف الإلكترونات: **نفس** القطع (بـ $\vec{E}$ بدل $\vec{g}$)! والسيكلوترون كيدور البروتونات فـ **حلزون** باش يداوي السرطان! ثلاثة الآلات، **منهجية وحدة**: المبدأ مسقط ← المعادلات الزمنية ← المسار! هاد الفصل = المبدأ اللي كيرسم المنحنيات!

## 2. Résumé du cours (exigible au bac)

### 2.1 Projectile dans $\vec{g}$ (référentiel terrestre galiléen)
- Conditions initiales : $\vec{v}_0$ ($v_0$, angle $\alpha$), position $O$ (origine). PFD : $m\vec{g} = m\vec{a}$ →
  $a_x = 0$, $a_y = -g$ (axe $y$ vers le haut).
- Horaires : $\boxed{x = v_0\cos\alpha\cdot t}$ ; $\boxed{y = -\frac{1}{2}gt^2+v_0\sin\alpha\cdot t}$ ;
  $v_x = v_0\cos\alpha$ (CONSTANTE !), $v_y = -gt+v_0\sin\alpha$.
- Trajectoire (éliminer $t$) : $\boxed{y = -\frac{g}{2v_0^2\cos^2\alpha}x^2+x\tan\alpha}$ (parabole !).
- Portée ($y = 0$, $x\ne 0$) : $\boxed{P = \frac{v_0^2\sin 2\alpha}{g}}$ (max à $\alpha = 45°$ !).
- Flèche ($v_y = 0$) : $\boxed{F = \frac{v_0^2\sin^2\alpha}{2g}}$ ; durée : $T = \frac{2v_0\sin\alpha}{g}$.

### 2.2 Particule chargée dans $\vec{E}$ uniforme (déflexion électrostatique)
- Force : $\vec{F} = q\vec{E}$ → PFD : $\vec{a} = \frac{q}{m}\vec{E}$ (poids NÉGLIGÉ devant $qE$ pour $e^-$, $p^+$ !).
- MÊME mathématique que le projectile avec $g \to |q|E/m$ (selon le signe de $q$ !) : parabole, déviation
  $Y = \frac{|q|EL^2}{2mv_0^2}$ (plaques de longueur $L$, entrée ⊥ à $\vec{E}$).
- Application : oscilloscope, imprimante à jet d'encre, canon à électrons.

### 2.3 Particule chargée dans $\vec{B}$ (uniforme, $\vec{v}_0 \perp \vec{B}$)
- Force de Lorentz : $\vec{F} = q\vec{v}\wedge\vec{B}$ (⊥ à $\vec{v}$ : NE TRAVAILLE PAS → $|\vec{v}| = \text{Cte}$ !).
- PFD : mouvement CIRCULAIRE UNIFORME de rayon $\boxed{R = \frac{mv}{|q|B}}$ ; période $\boxed{T = \frac{2\pi m}{|q|B}}$
  (INDÉPENDANTE de $v$ ! — le secret du cyclotron).
- Sens de rotation : règle des 3 doigts ($\vec{F} = q\vec{v}\wedge\vec{B}$ : signe de $q$ !).
- Cyclotron (principe) : $\vec{B}$ courbe + $\vec{E}$ alternatif accélère à chaque demi-tour ($f = f_{cyclotron}$ :
  synchronisme possible CAR $T$ indépendante de $v$ !).

### 2.4 Repère de Frenet (complément utile)
- $(\vec{T},\vec{N})$ : tangent + normal centripète. $\vec{a} = \frac{dv}{dt}\vec{T}+\frac{v^2}{R}\vec{N}$ :
  tangentiel (change $|\vec{v}|$) + normal (change la DIRECTION). Circulaire uniforme : $a_T = 0$, $a_N = v^2/R$.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** الحركة المستوية = **حركتين مستقيميتين مستقلتين** ($x$ و$y$)! حل كل محور بوحدو ($x$: منتظمة، $y$: متسارعة) ومن بعد جمع!

1. **القذيفة:** $x$ بسرعة ثابتة ($v_0\cos\alpha$ — ما كاين حتى قوة أفقية!)، و$y$ سقوط بتسارع $-g$! المسار = حذف الزمن ← قطع مكافئ! المدى أعظمي فـ $45°$ ($P = v_0^2\sin 2\alpha/g$)!
2. **الجسيم فـ $\vec{E}$:** نفس الرياضيات مع $g \to qE/m$! الإلكترون كينحرف عكس $\vec{E}$ (شحنة سالبة!) ← قطع مكافئ ← الشاشات! الثقل مهمل (صغير بزاف قدام $qE$)!
3. **الجسيم فـ $\vec{B}$:** قوة لورنتز **عمودية على السرعة** ← ما كتخدمش ← السرعة ثابتة الشدة! والقوة الجابذة ($qvB = mv^2/R$) ← **دائرة منتظمة**! الدور $T = 2\pi m/qB$ **مستقل على السرعة** — هادا هو سر السيكلوترون!
4. **فرينيه:** التسارع = مماسي (كيبدل الشدة) + ناظمي (كيبدل الاتجاه: $v^2/R$)! الدائري المنتظم: غير الناظمي ($v^2/R$ للداخل)!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — المحاور أولاً!** $x$ أفقي ($v_x$ ثابتة إلا ما كاين قوة أفقية!)، $y$ عمودي. الشروط البدئية ($v_{0x} = v_0\cos\alpha$، $v_{0y} = v_0\sin\alpha$) — الغلطة هنا = كلشي غالط!

**الخطوة 2 — المبدأ مسقط على كل محور.** $x$: غالباً $a_x = 0$ ← $x = v_{0x}t$! $y$: $a_y = -g$ (ولا $qE/m$) ← $y = \frac{1}{2}a_yt^2+v_{0y}t$! محور بمحور — ما تخلطش!

**الخطوة 3 — المسار = حذف $t$.** من $x(t)$: $t = x/v_{0x}$ ← عوض فـ $y(t)$ ← $y(x)$ (قطع مكافئ)! المدى: $y = 0$! الذروة: $v_y = 0$! الأسئلة الكلاسيكية = هاد الثلاثة!

**الخطوة 4 — $\vec{B}$: دائرة مباشرة!** $\vec{v} \perp \vec{B}$ ← دائري منتظم ($R = mv/qB$)! القوة عمودية ← السرعة ثابتة! الاتجاه: قاعدة الأصابع + إشارة $q$! والدور مستقل على $v$ (سؤال السيكلوترون المفضل)!

**الخطوة 5 — الأخطاء القاتلة:** $v_{0x}/v_{0y}$ مقلوبين ($\cos$ مع $x$!)؛ $y_0$ منسي (القذف من علو!)؛ $45°$ للمدى الأعظمي منسية؛ الثقل معتبر مع الإلكترون (مهمل!)؛ $R = mv/qB$ بالـ $v^2$ (غلط! $R$ بالـ $v$!)؛ إشارة $q$ فالاتجاه (الإلكترون عكس $\vec{E}$!)!

## 5. Définitions & formules clés (FR + Darija)

| Notion FR (LaTeX) | Énoncé FR | بالدارجة |
|---|---|---|
| $x = v_0\cos\alpha\cdot t$ | MRU horizontal (projectile) | الأفقي: منتظمة |
| $y = -\frac{1}{2}gt^2+v_0\sin\alpha\cdot t$ | MRUV vertical | العمودي: متسارعة |
| $P = \frac{v_0^2\sin 2\alpha}{g}$ | Portée (max à $45°$) | المدى (أعظم فـ $45°$) |
| $F = \frac{v_0^2\sin^2\alpha}{2g}$ | Flèche ($v_y = 0$) | الذروة |
| $\vec{a} = \frac{q}{m}\vec{E}$ | Particule dans E (poids négligé) | الجسيم فالمجال الكهربائي |
| $R = \frac{mv}{|q|B}$, $T = \frac{2\pi m}{|q|B}$ | Circulaire uniforme (B) | الدائري المنتظم |
| $\vec{a} = \frac{dv}{dt}\vec{T}+\frac{v^2}{R}\vec{N}$ | Frenet : tangentiel + normal | فرينيه: المماسي + الناظمي |

## 6. FAQ du chapitre

**Q1. Pourquoi la trajectoire est une parabole ?**
Parce que $x\propto t$ (degré 1) et $y\propto t^2$ (degré 2) : éliminer $t$ donne $y\propto x^2$ ! Tout mouvement
« MRU × MRUV » est parabolique (projectile, électron dans E, goutte d'encre...) !
بالدارجة: $x$ درجة 1 و$y$ درجة 2 ← حذف الزمن كيعطي $y$ تابع لـ $x^2$! أي حركة «منتظمة × متسارعة» قطع مكافئ!

**Q2. Pourquoi $45°$ = portée max ?**
$P\propto\sin 2\alpha$ : max quand $\sin 2\alpha = 1$ ⟺ $\alpha = 45°$. Physique : compromis — $0°$ : vite mais
retombe tôt ; $90°$ : haut mais $v_x = 0$ ; $45°$ : le juste milieu !
بالدارجة: المدى تابع لـ $\sin 2\alpha$: أعظمي ملي $= 1$ ← $45°$! حل وسط: $0°$ سريع ولكن كيطيح دغيا، $90°$ عالي ولكن بلا أفقية!

**Q3. Pourquoi négliger le poids de l'électron ?**
$mg = 9,1\times10^{-31}\times9,8\approx 10^{-29}\,N$ vs $eE\approx 10^{-16}\,N$ (pour $E = 10^3\,V/m$) : rapport
$10^{13}$ ! Le poids est 10 000 milliards de fois plus petit — invisible. (Toujours JUSTIFIER la négligence !)
بالدارجة: الثقل $10^{-29}$ ضد الكهربائية $10^{-16}$: مليون مليون مرة أصغر — ما كيبانش! (وديماً برر الإهمال!)

**Q4. Pourquoi $\vec{B}$ ne change pas $|\vec{v}|$ ?**
$\vec{F} = q\vec{v}\wedge\vec{B}$ est TOUJOURS ⊥ à $\vec{v}$ → puissance $P = \vec{F}\cdot\vec{v} = 0$ → pas de
travail → $E_c$ constante → $|\vec{v}|$ constante ! $\vec{B}$ TOURNE, il ne pousse pas.
بالدارجة: القوة ديماً عمودية على السرعة ← القدرة صفر ← الشغل صفر ← الطاقة ثابتة! $\vec{B}$ **كيدور**، ما كيدفعش!

**Q5. Pourquoi $T$ indépendante de $v$ (cyclotron) ?**
$T = 2\pi R/v$ et $R = mv/qB$ : les $v$ SE SIMPLIFIENT → $T = 2\pi m/qB$ ! Plus vite = plus grand cercle, pile
dans les temps pour le même tour. D'où le synchronisme du cyclotron (fréquence FIXE !).
بالدارجة: $T = 2\pi R/v$ و$R = mv/qB$: الـ $v$ كيتحيدو! الأسرع = دائرة أكبر، بنفس الدور بالضبط! وهنا سر السيكلوترون (تردد ثابت)!

**Q6. Frenet : à quoi ça sert ?**
À LIRE l'accélération : $a_T = dv/dt$ (ça accélère/ralentit ?) + $a_N = v^2/R$ (ça tourne, rayon $R$ ?).
Circulaire uniforme : $a_T = 0$, $a_N = v^2/R$ vers le centre — tout est dit en une ligne !
بالدارجة: باش **تقرا** التسارع: المماسي (واش كتسرع؟) + الناظمي (واش كتدور؟ بشحال؟)! الدائري المنتظم: غير $v^2/R$ للداخل — كلشي فسطر!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : système + référentiel galiléen ; PFD projeté ($a_x$, $a_y$) ; conditions initiales
($v_{0x}$, $v_{0y}$) ; horaires ; trajectoire (élimination de $t$) ; « poids négligé car… » (particules) ;
$\boxed{\text{résultats}}$.
**Erreurs fréquentes** : $v_{0x} = v_0\sin\alpha$ ❌ ; $y_0$ oublié (tir depuis une hauteur) ❌ ; E avec poids
non négligé sans justification ❌ ; $R = mv^2/qB$ ❌ ; signe de $q$ (sens de $\vec{F}$/déviation) ❌ ;
$45°$ affirmée sans $\sin 2\alpha$ ❌.

## 8. Sources de ce chapitre
- Synthèse prof (cours + exercices type-bac) : rédaction originale pour cette base, 2026-09-15.
- Backfill prévu : questions mouvements verbatim du national PC (sessions 2023-2025 prioritaires).

## 9. Le « pourquoi » profond — l'indépendance des axes 🔬

**Pourquoi $x(t)$ et $y(t)$ sont indépendants ? (la linéarité)**
Le PFD est une équation VECTORIELLE linéaire : $\vec{a} = \sum\vec{F}/m$ se projette en 2 équations SCALAIRES
indépendantes ($a_x = F_x/m$, $a_y = F_y/m$). Ce qui pousse en $x$ ne touche pas $y$ (axes ⊥ !). D'où le « miracle »
du projectile : chute verticale + avance horizontale COEXISTENT sans se parler (Galilée : la balle tirée et la
balle lâchée touchent le sol ENSEMBLE !). Moral : face au plan, PENSE 2×1D, jamais 1×2D !

**Pourquoi parabole (et pas ellipse/cercle) ?**
$x\propto t^1$ + $y\propto t^2$ ⟹ $y\propto x^2$ : c'est le DEGRÉ 2 (accélération CONSTANTE !) qui fait la parabole.
Avec $\vec{a}$ variable (ressort, gravitation), d'autres courbes (ellipses !) apparaissent. La parabole EST la
signature de « $\vec{a}$ constant + $\vec{v}_0$ inclinée ». Retenir les signatures : $\vec{a} = \vec{0}$ → droite,
$\vec{a} = \text{Cte}$ → parabole, $\vec{a} = -v^2/R$ centripète → cercle, $\vec{a} = -\omega^2\vec{r}$ → ellipse !

**Pourquoi $\vec{B}$ fait des cercles ? (force ⊥ vitesse, norme Cte)**
$|\vec{F}| = |q|vB$ : $v$ Cte (pas de travail !) + $B$ uniforme ⟹ $|\vec{F}|$ Cte, TOUJOURS ⊥ à $\vec{v}$ (courbure
constante !). Courbure constante = CERCLE (par définition géométrique : $R = 1/\text{courbure}$ !). Et
$qvB = mv^2/R$ donne $R$ : la « force » fournit exactement le centripète requis. Si $v$ changeait ($E$ présent !),
le cercle deviendrait spirale (cyclotron !) — d'où la différence E vs B.

**Pourquoi le cyclotron marche ? (le synchronisme miraculeux)**
$T = 2\pi m/qB$ indépendante de $v$ : quel que soit le tour (petit/lent ou grand/vite), le proton revient AU MÊME
RYTHME. Donc un champ $\vec{E}$ alternatif de fréquence $f = 1/T$ le pousse À CHAQUE demi-tour, en phase, jusqu'à
des MeV ! Sans cette indépendance, il faudrait ajuster la fréquence en continu (synchrotron : c'est ce qu'on fait
quand $m$ devient relativiste !). Limite du cyclotron classique : Einstein ($m = \gamma m_0$ casse le synchronisme).

**Ponts :** Newton ch.10 (le PFD projeté : TOUT part de là !) ; chute verticale ch.11 (cas 1D : $\alpha = 90°$ !) ;
satellites ch.28 (gravitation : $\vec{a}$ variable → ellipses/cercles orbitaux !) ; oscillateurs ch.14-15
($\vec{a} = -\omega^2\vec{x}$ : retour élastique) ; Maths vecteurs/dérivées ($\vec{v} = d\vec{r}/dt$ : la cinématique
EST du calcul différentiel !) ; SVT (biomécanique : saut, lancer — paraboles du corps !).

> بالدارجة: علاش $x$ و$y$ مستقلين؟ حيت المبدأ خطي: اللي كيدفع فـ $x$ ما كيقيسش $y$! الرصاصة المقذوفة والطايحة كيوصلو للأرض **مع بعض** (غاليلي)! القاعدة: واجه المستوى بـ **جوج × 1D**! وعلاش قطع مكافئ؟ $x$ درجة 1 + $y$ درجة 2 ← $y$ تابع لـ $x^2$! القطع هو **بصمة** التسارع الثابت! و$\vec{B}$ كيدير دوائر حيت القوة عمودية وثابتة الشدة ← انحناء ثابت = **دائرة**! والسيكلوترون خدام حيت الدور مستقل على السرعة ← تردد واحد كيدفع فكل نص دورة!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $v_{0x} = v_0\cos\alpha$ vs $v_0\sin\alpha$ — le test $\alpha = 0$.**
*Le clic :* $\alpha = 0$ (tir horizontal) → $v_{0x}$ doit valoir $v_0$ ENTIER → c'est $\cos$ ($\cos 0 = 1$ !).
$\alpha = 90°$ (tir vertical) → $v_{0x} = 0$ → $\cos 90 = 0$ ✔. Même test que le plan incliné (§10-C1 ch.10) :
les CAS LIMITES tranchent TOUJOURS les $\sin/\cos$ !
بالدارجة: $\alpha = 0$ (أفقي) ← $v_{0x} = v_0$ كاملة ← هو **$\cos$**! $\alpha = 90°$ ← صفر ← $\cos 90 = 0$ ✔! نفس اختبار المستوى المائل: **الحالات الحدية** كتحسم ديماً!

**C2. $\vec{E}$ dévie, $\vec{B}$ courbe — deux effets, deux signatures.**
*Le clic :* $\vec{E}$ : force CONSTANTE (direction fixe) → PARABOLE (comme $\vec{g}$ !). $\vec{B}$ : force TOURNANTE
(toujours ⊥ à $\vec{v}$) → CERCLE. « Électron dans E : trajectoire circulaire » = FAUX (c'est parabolique !).
« Dans B : parabole » = FAUX (c'est circulaire !). Retiens : E = g (chute), B = fronde (tourne).
بالدارجة: $\vec{E}$: قوة ثابتة الاتجاه ← **قطع مكافئ** (بحال الثقل)! $\vec{B}$: قوة دوارة (عمودية ديماً) ← **دائرة**! حفظ: E = الثقل (طيحة)، B = المقلاع (دوران)!

**C3. $R = mv/qB$ : $v$ au numérateur — plus vite = PLUS GRAND cercle !**
*Le clic :* contre-intuitif (on s'attend à « plus vite = plus courbé ») : $R\propto v$ — à 2× plus vite, rayon 2×
plus grand (l'inertie « résiste » à la courbure : $mv^2/R = qvB$ → $R = mv/qB$). Vérifie par $T = 2\pi R/v$ :
les $v$ se simplifient (indépendance !) — si ton $R$ avait $v^2$, $T$ dépendrait de $v$ (contradiction !).
بالدارجة: عكس الحدس: الأسرع = دائرة **أكبر** ($R \propto v$ — القصور كيقاوم الانحناء)! تحقق: $T = 2\pi R/v$ خاص الـ $v$ يتحيدو — إلا $R$ فيها $v^2$ راه غالطة!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Newton (ch.10) : PFD + projection + cas limites — TOUT le chapitre en découle.
2. Dérivées/primitives (Maths) : $\vec{v} = \dot{\vec{r}}$, $\vec{a} = \dot{\vec{v}}$ — cinématique = calcul diff.
3. Trigo : $\sin/\cos$, $\sin 2\alpha = 2\sin\alpha\cos\alpha$ (portée !).
4. Vecteurs + produit vectoriel (sens de $q\vec{v}\wedge\vec{B}$ : règle des 3 doigts !).

**Si les horaires emmêlent — plan B :**
Le mur : $x(t)$, $y(t)$, $v_x$, $v_y$ mélangés + $t$ qui résiste. **Fallback** : (1) TABLEAU 2 colonnes ($x$ | $y$) :
$a$, $v(t)$, $x(t)$ dans chaque — JAMAIS de mélange ; (2) questions SANS $t$ (portée, flèche, vitesse en un point) :
éliminer $t$ EN PREMIER (trajectoire $y(x)$, $v^2 = \ldots$) ; (3) $\vec{B}$ : écrire $qvB = mv^2/R$ DIRECTEMENT
(c'est LE réflexe circulaire, pas besoin des horaires !) ; (4) vérifier les UNITÉS : $v_0^2/g$ en mètres ✔ !
بالدارجة: إلا تخلطو المعادلات: **جدول بجوج أعمدة** ($x$ | $y$): $a$، $v(t)$، $x(t)$ فكل واحد — عمرك تخلط! والأسئلة بلا $t$: حذف الزمن **أولاً**! و$\vec{B}$: كتب $qvB = mv^2/R$ **مباشرة** (منعكس الدائري)! وتأكد بالوحدات ($v_0^2/g$ بالأمتار ✔)!
