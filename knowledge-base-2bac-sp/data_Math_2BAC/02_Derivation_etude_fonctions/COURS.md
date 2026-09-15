---
chapitre: "02 - Dérivation et étude de fonctions"
unite: "S1 - Analyse de base"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (style national PC/SVT) - verbatim en backfill (banque Fayssal repérée)"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 02 — Dérivation & étude de fonctions

> 📋 **Exigible au bac** : nombre dérivé, tangente, dérivées usuelles + opérations + composées, signe de $f'$ →
> variations, extrema, TVI (rappel ch.01), asymptotes (verticales, horizontales, obliques), plan d'étude + tracé.

## 1. Accroche — le compteur de vitesse 🏎️

**FR :** Le compteur de ta voiture affiche 90 km/h : c'est la dérivée de ta position ! La dérivée = la vitesse
instantanée de variation. Pourquoi c'est puissant ? Parce qu'au lieu de calculer $f$ en 1000 points pour deviner
sa forme, tu calcules $f'$ UNE fois et son SIGNE te dit tout : $f' > 0$ → ça monte, $f' < 0$ → ça descend,
$f' = 0$ → sommet ou creux. Tout le chapitre = transformer une formule en portrait (variations + asymptotes + courbe).

**بالدارجة:** العداد ديال الطوموبيل كيقول 90 km/h — هادي هي المشتقة ديال الموقع! المشتقة = **السرعة اللحظية ديال التغير**.
علاش قوية؟ حيت بلا ما تحسب $f$ فـ 1000 نقطة، كتحسب $f'$ مرة وحدة والإشارة ديالها كتقول لك كلشي: موجبة = طالعة، سالبة = هابطة، صفر = قمة ولا قعر!

## 2. Résumé du cours (exigible au bac)

### 2.1 Nombre dérivé & tangente
- Taux d'accroissement en $a$ : $\tau(h) = \frac{f(a+h)-f(a)}{h}$. Si $\lim_{h\to 0}\tau(h) = \ell$ (finie),
  $f$ est **dérivable en $a$** et $f'(a) = \ell$.
- **Tangente** en $a$ : $\boxed{y = f'(a)(x-a) + f(a)}$ (à savoir par cœur !).
- Dérivable ⟹ continue (mais continue ⇏ dérivable : $|x|$ et $\sqrt{x}$ en 0 !).

### 2.2 Dérivées usuelles (tableau cœur)

| $f$ | $f'$ | $f$ | $f'$ |
|---|---|---|---|
| $k$ | $0$ | $x^n$ | $nx^{n-1}$ |
| $\sqrt{x}$ | $\frac{1}{2\sqrt{x}}$ | $\frac{1}{x}$ | $-\frac{1}{x^2}$ |
| $e^x$ | $e^x$ | $\ln x$ | $\frac{1}{x}$ |
| $\sin x$ | $\cos x$ | $\cos x$ | $-\sin x$ |

### 2.3 Opérations & composées
- $(u+v)' = u'+v'$ ; $(ku)' = ku'$ ; $(uv)' = u'v+uv'$ ; $\left(\frac{1}{v}\right)' = -\frac{v'}{v^2}$ ;
  $\left(\frac{u}{v}\right)' = \frac{u'v-uv'}{v^2}$.
- **Composée** : $(g\circ f)' = f'\times(g'\circ f)$. Cas réflexes : $(u^n)' = nu'u^{n-1}$ ;
  $(e^u)' = u'e^u$ ; $(\ln u)' = \frac{u'}{u}$ ; $(\sqrt{u})' = \frac{u'}{2\sqrt{u}}$.
- ⚠️ L'oubli du facteur $u'$ (« dérivée intérieure ») est LA faute n°1 du chapitre.

### 2.4 Signe de $f'$ → variations → extrema
- $f' > 0$ sur $I$ → $f$ strictement croissante ; $f' < 0$ → strictement décroissante ; $f' = 0$ → constante.
- **Extremum** en $a$ ⟺ $f'$ **s'annule EN CHANGEANT DE SIGNE** en $a$ (s'annuler seul ne suffit pas : $x^3$ en 0 !).

### 2.5 Asymptotes & branches infinies
- **Verticale** $x = a$ : $\lim_{x\to a}f = \pm\infty$ (souvent valeur interdite).
- **Horizontale** $y = \ell$ en $\pm\infty$ : $\lim_{x\to\pm\infty}f = \ell$ (finie).
- **Oblique** $y = ax+b$ : $\lim_{x\to\pm\infty}[f(x)-(ax+b)] = 0$. Méthode rationnelle : division
  ($f(x) = ax+b+\frac{reste}{\ldots}$) ; méthode générale : $a = \lim f(x)/x$, $b = \lim (f(x)-ax)$.
- **Branche parabolique** : $f(x)/x \to \pm\infty$ (direction $Oy$) ou $\to a$ avec $f(x)-ax\to\pm\infty$.

### 2.6 Convexité (complément)
- $f'' \ge 0$ → **convexe** (creux vers le haut, « sourire ») ; $f'' \le 0$ → **concave** (« grimace »).
- **Point d'inflexion** : $f''$ s'annule en changeant de signe (la courbe traverse sa tangente).

### 2.7 Bijection & fonction réciproque (tombé 2025N + 2026N !)
- $f$ continue STRICTEMENT monotone sur $I$ ⟹ **bijection** de $I$ sur $J = f(I)$ (l'intervalle image : lire les limites/tableau !).
- Réciproque $f^{-1} : J \to I$ : $\boxed{y = f(x) \iff x = f^{-1}(y)}$ ; $(f^{-1})' = \frac{1}{f' \circ f^{-1}}$ (là où $f' \ne 0$ !).
- Courbes $C_f$ et $C_{f^{-1}}$ **symétriques par rapport à $y = x$** → tangente à $C_{f^{-1}}$ en $(b,a)$ = symétrique de la tangente à $C_f$ en $(a,b)$.
- Méthode nationale (4 gestes) : (1) continuité + stricte monotonie sur $I$ ; (2) $J = f(I)$ via tableau/limites ;
  (3) tracer $C_{f^{-1}}$ par symétrie (points + tangentes !) ; (4) $(f^{-1})'(b) = 1/f'(a)$ avec $b = f(a)$.
- ⚠️ $f^{-1}$ n'a presque JAMAIS d'expression simple au national ($x - (\ln x)^2/x$ en 2025N !) : on travaille avec $y = f(x)$, jamais en « isolant $x$ ».

### 2.8 Plan d'étude complète (l'ordre qui rapporte)
1. Ensemble de définition (+ parité/périodicité si utile). 2. Limites aux bornes → asymptotes.
3. $f'$ + signe → tableau de variations (avec limites !). 4. TVI/équations éventuelles.
5. Tangentes remarquables + points clés. 6. Tracé soigné (asymptotes en pointillés !).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** المشتقة = **البوصلة ديال الدالة**! الإشارة ديالها كتقول لك واش طالعة ولا هابطة بلا ما تحسب حتى قيمة.

1. **العدد المشتق:** هو نهاية معدل التغير — الميل ديال المماس. المماس: $y = f'(a)(x-a)+f(a)$ — حفظها كيفما هي!
2. **جدول المشتقات:** $x^n \to nx^{n-1}$، $e^x$ ما كتتبدلش (هي البطلة!)، $\ln x \to 1/x$. العمليات: الجمع ساهل، الضرب ($u'v+uv'$) والقسمة كيحتاجو التركيز.
3. **المركبة:** القاعدة الذهبية: **اشتق البرا وخلي الداخل، ومن بعد ضرب فمشتقة الداخل**! $(e^{3x})' = 3e^{3x}$ — اللي نسى الـ 3 خسر!
4. **التغيرات:** إشارة $f'$ = الطلوع والهبوط. والقمة/القعر: $f'$ كتصفر **وكتبدل الإشارة** — الصفر بوحدو ما كافي ($x^3$ فـ 0 ما عندها لا قمة لا قعر)!
5. **المقاربات:** عمودي (النهاية لانهائية)، أفقي (النهاية عدد)، مائل (الفرق كيمشي للصفر). القسمة الإقليدية كتخرج المائل مباشرة!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — أي دراسة دالة بدا بالتعريف والنهايات.** مجال التعريف أولاً (المقام ≠ 0، ما تحت الجذر ≥ 0، $\ln$ ← ما بداخله > 0)،
ومن بعد النهايات فالأطراف ← المقاربات العمودية والأفقية كيبانو بوحدهم!

**الخطوة 2 — المشتقة والإشارة هما القلب.** اشتق، بسّط، عمّل! الهدف: $f'$ على شكل **جداء/خارج** باش الإشارة تبان (مربع ديماً موجب، $e^{شي حاجة}$ ديماً موجبة).
إلا خرجات $f'$ معقدة ← عرّف دالة مساعدة $g$ وادرس إشارتها (تقنية الوطني!).

**الخطوة 3 — الجدول كيجمع كلشي.** جدول التغيرات = التعريف + إشارة $f'$ + السهام + النهايات + القيم الحدية. جدول عامر مزيان = أغلبية النقط وخا الرسم ناقص!

**الخطوة 4 — المماس والتقعر لمسات أخيرة.** المماس فالنقط المهمة ($y = f'(a)(x-a)+f(a)$) والمقاربات بالمنقط — هما اللي كيخليو الرسم احترافي.

**الخطوة 5 — الأخطاء القاتلة:** نسيان $u'$ فالمركبة؛ «$f'(a)=0$ إذن extremum» بلا إشارة؛ المقارب المائل بلا إثبات ($\lim[f-(ax+b)]=0$ إجباري!)؛
الرسم بلا مقاربات ولا مماسات (نص النقطة!).

## 5. Définitions clés (FR + Darija)

| Notion | FR | بالدارجة |
|---|---|---|
| Nombre dérivé | $\lim_{h\to 0}\frac{f(a+h)-f(a)}{h}$ = pente de la tangente | ميل المماس — سرعة التغير فالنقطة |
| Tangente | $y = f'(a)(x-a)+f(a)$ | المستقيم اللي كيلمس المنحنى |
| Extremum | $f'$ s'annule + change de signe | القمة/القعر — الصفر مع تبديل الإشارة |
| Asymptote | Droite approchée à l'infini (ou en $a$) | المستقيم اللي كيقرب منو المنحنى |
| Point d'inflexion | $f''$ s'annule + change de signe | فين التقعر كيتبدل |

## 6. FAQ du chapitre

**Q1. Pourquoi étudier le SIGNE de $f'$ et pas ses valeurs ?**
Parce que seul le signe décide du sens (monte/descend). Les valeurs exactes de $f'$ ne servent qu'aux tangentes.
بالدارجة: حيت الإشارة هي اللي كتحكم فالطلوع والهبوط — القيم ما كيهموك غير فالمماس!

**Q2. $f'(a) = 0$ ⟹ extremum ?**
NON sans le changement de signe ! $f(x) = x^3$ : $f'(0) = 0$ mais 0 monte partout (point d'inflexion, pas d'extremum).
بالدارجة: لا! $x^3$ فـ 0: المشتقة صفر ولكن الدالة طالعة — الصفر خاصو **تبديل الإشارة**!

**Q3. Comment trouver une asymptote oblique vite ?**
Fraction rationnelle : DIVISION euclidienne → partie entière $ax+b$ + reste qui tend vers 0. Sinon : $a = \lim f/x$, $b = \lim (f-ax)$.
بالدارجة: الكسر: القسمة كتعطيك $ax+b$ مباشرة! ولا: $a$ من $f/x$ و$b$ من $f-ax$.

**Q4. Dérivable vs continue ?**
Dérivable ⟹ continue (toujours). Continue ⟹ dérivable ? NON : $|x|$ en 0 (point anguleux), $\sqrt{x}$ en 0 (tangente verticale).
بالدارجة: قابلية الاشتقاق أقوى من الاتصال! المتصلة تقدر تكون مزوية ($|x|$) ولا عمودية ($\sqrt{x}$) فـ 0.

**Q5. C'est quoi une fonction auxiliaire $g$ ?**
Quand $f'$ a un signe illisible, on pose $g$ = le morceau gênant, on étudie $g$ (elle-même !), et son signe donne celui de $f'$.
C'est LA technique du problème national.
بالدارجة: ملي إشارة $f'$ ما بايناش ← سمي الطرف المزعج $g$ وادرسو بوحدو! هادي هي تقنية المسألة الوطنية.

**Q6. Réciproque sans formule : comment faire ?**
On ne cherche PAS $f^{-1}(x)$ ! On utilise $y = f(x) \iff x = f^{-1}(y)$ : équation $f^{-1}(b) = a \iff f(a) = b$, dérivée $(f^{-1})'(b) = 1/f'(a)$, courbe par symétrie $y = x$. 2025N : $\varphi^{-1}$ de $x-(\ln x)^2/x$ — aucune formule, tout par $y = f(x)$ !
بالدارجة: ما تقلبش على صيغة $f^{-1}$! خدم بالتكافؤ $y = f(x) \iff x = f^{-1}(y)$: المعادلات، المشتقة ($1/f'$)، والمنحنى بالتناظر حول $y = x$!

**Q7. Faut-il tracer la courbe à tout prix ?**
OUI si demandé (« construire » = points !), avec asymptotes + tangentes + extrema. Un tracé faux mais cohérent avec TON tableau
perd moins qu'un tracé absent.
بالدارجة: إيه! وخا الجدول عندك فيه غلطة، رسم متوافق معاه حسن من والو!

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : $D_f$ justifié ; « $f$ est dérivable sur… car… » ; $f'$ simplifiée ET factorisée ;
tableau COMPLET (signes + flèches + limites) ; preuves de TOUTE asymptote ; $\boxed{\text{résultats}}$.
**Erreurs fréquentes** : $u'$ oublié (composée) ❌ ; extremum sans changement de signe ❌ ; asymptote oblique
affirmée sans limite ❌ ; tableau sans limites aux bornes ❌ ; tangente avec $f(a)$ mal calculé ❌ ;
réciproque : $J$ faux (limites non lues ❌), $(f^{-1})' = 1/f'$ sans composition ($1/f'(a)$ avec $f(a) = b$ !) ❌,
symétrie par rapport à $Ox$ au lieu de $y = x$ ❌.

## 8. Sources de ce chapitre
- Banque Fayssal Maths — nationaux SX (PC/SVT/ST) par thèmes 2011-2025 (repérée 2026-09-15, PDFs Jimdo à exploiter :
  https://www.fayssalmaths.com/2-bac-sciences-exp%C3%A9rimentales/examens-nationaux-corrig%C3%A9s-math%C3%A9matiques-2bac-sciences-exp%C3%A9rimentales/).
- Scribd — recueil corrigés nationaux Math SX 2003-2023 (extraits : $f'$, variations, TVI — non téléchargeable).
- National 2025N Problème II : réciproque $\varphi^{-1}$ de $f(x) = x-(\ln x)^2/x$ (mining Tier A sujet intégral, scribd 878589899 ; énoncé reconstitué, à recouper).
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-15.

## 9. Le « pourquoi » profond — la dérivée voit l'avenir 🔬

**Pourquoi le signe de $f'$ donne les variations ? (l'intuition des accroissements finis)**
Si $f'(x) > 0$ partout sur $[a,b]$, chaque petit pas $h$ fait monter $f$ d'environ $f'(x)\times h > 0$.
En accumulant des milliers de petits pas positifs, on monte FORCÉMENT : $f(b) > f(a)$. La dérivée positive =
« à chaque instant, la pente penche vers le haut » = impossible de finir plus bas. C'est le théorème des
accroissements finis qui rend cette intuition rigoureuse — le national l'admet, toi tu l'exploites.

**Pourquoi la tangente est la « meilleure droite » ?**
$y = f'(a)(x-a)+f(a)$ n'est pas une droite quelconque : c'est l'unique droite qui épouse la courbe à l'ordre 1
(erreur en $(x-a)^2$, négligeable près de $a$). C'est pour ça que les physiciens linéarisent tout avec des
tangentes (cf. $\tau$ en RC/RL !) : près du point, courbe $\approx$ tangente. Approximation affine = application
n°1 de la dérivée dans la nature.

**Pourquoi $f''$ donne la forme (sourire/grimace) ?**
$f''$ = dérivée de $f'$ = « la pente, elle-même, monte ou descend ? ». Si $f'$ croît ($f''>0$), la pente passe de
négative à positive → creux → « sourire » (convexe). Le point d'inflexion = le moment où la pente cesse
d'augmenter pour diminuer : la courbe traverse sa tangente. $f'$ = vitesse, $f''$ = accélération : même histoire
qu'en physique !

**Ponts :** ch.01 (limites : le taux $\to$ nombre dérivé ; asymptotes) ; Physique (vitesse = $x'$, EDP : on VÉRIFIE
les solutions en dérivant !) ; Suites ch.03 (sens d'une suite $u_{n+1} = f(u_n)$ via les variations de $f$) ;
ln/exp ch.05/07 (les études du national = CE chapitre appliqué à $\ln$ et $e^x$).

> بالدارجة: علاش إشارة $f'$ كتعطي التغيرات؟ حيت $f' > 0$ معناها: **كل خطوة صغيرة كتطلع** — وآلاف الخطوات الطالعة مستحيل يهبطو بك! والمماس ماشي مستقيم عادي: هو **أحسن مستقيم كيعوض المنحنى** قريب من النقطة (الفيزيائيين كيستعملوه فكلشي!). و$f''$ = واش الميل طالع ولا هابط = الابتسامة ولا العبوسة!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. « $f'(a) = 0$ donc extremum en $a$ » — FAUX sans le signe !**
*Le clic :* $x^3$ en 0 : dérivée nulle, PAS d'extremum (ça monte avant ET après). La règle complète :
« $f'$ s'annule en $a$ **ET change de signe** ⟺ extremum ». Le contre-exemple $x^3$ à garder en tête pour toujours.
بالدارجة: $x^3$ فـ 0: المشتقة صفر وما كاين لا قمة لا قعر! القاعدة الكاملة: **صفر + تبديل الإشارة**. حفظ هاد المثال المضاد!

**C2. Asymptote horizontale vs oblique — le test qui tranche.**
*Le clic :* en $\pm\infty$, calcule $\lim f$ D'ABORD : finie → horizontale (c'est fini !) ; infinie → SEULEMENT ALORS
chercher oblique/parabolique via $f(x)/x$. Ceux qui attaquent $f(x)/x$ directement perdent du temps et se trompent.
Ordre : limite → (si infinie) $f/x$ → (si $a$) $f-ax$.
بالدارجة: فاللانهاية: حسب النهاية **أولاً**! عدد ← أفقي وسالات. لانهاية ← عاد قلب على المائل بـ $f/x$. الترتيب كيوفر الوقت!

**C3. Dérivée de la composée : le $u'$ fantôme.**
*Le clic :* $(e^{3x})' = 3e^{3x}$, PAS $e^{3x}$ ! Le réflexe : « je dérive l'extérieur, je RECOPIE l'intérieur, je
MULTIPLIE par la dérivée de l'intérieur ». Trois gestes, toujours. Vérifie sur $(\ln(2x+1))' = \frac{2}{2x+1}$ :
sans le 2, tout le tableau est faux.
بالدارجة: اشتق البرا + عاود الداخل + **ضرب فمشتقة الداخل** — ثلاثة الحركات ديماً! اللي نسى الضرب خسر الجدول كامل!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Limites (ch.01) : taux d'accroissement, FI, croissances comparées — le socle de TOUT le chapitre.
2. Factorisation + tableaux de signes (2nde/1ère) : $f'$ ne sert à rien si son signe est illisible.
3. Identités et équations : résoudre $f'(x) = 0$ proprement (second degré, équations $e^u = k$...).
4. Trigonométrie de base (si $f$ trigo) : cercle, signes de $\sin/\cos$.

**Si $f'$ est inexploitable — plan B :**
Le mur classique : $f'$ ne se factorise pas, signe invisible. **Fallback officiel** : (1) appelle $g$ le numérateur
ou le morceau gênant et étudie $g$ (signe via SES variations + SES valeurs : technique auxiliaire !) ; (2) si ça
coince encore, ADMETS les variations (« on admet le tableau suivant ») et fonce sur la suite du problème (TVI,
tracé, intégrale plus tard) : 70 % des points sont APRÈS le tableau !
بالدارجة: إلا $f'$ ما تفككاتش: سمي الطرف المزعج $g$ وادرسو! وإلا بقات حابسة: **قبل الجدول وكمل** — 70 % ديال النقط من بعد الجدول (TVI، الرسم...)!
