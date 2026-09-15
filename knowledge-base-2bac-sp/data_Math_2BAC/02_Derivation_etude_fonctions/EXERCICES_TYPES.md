---
chapitre: "02 - Dérivation et étude de fonctions"
unite: "S1 - Analyse de base"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituée (style national PC/SVT) + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 5 type-bac + 1 vraie 2020R + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 02 (Dérivation & études)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **R1-R5 = type-bac reconstituées** (variations, asymptote oblique, TVI, composée $e^x$, optimisation)
> + **Q6 = VRAIE** (2020 Rattrapage, Problème — fonction auxiliaire + variations). Chaque corrigé = méthode complète + 🪤.

## R1 — Variations + extrema + tangente

🏷️ matière=Math · année=— · session=— · chapitre=M2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** $f(x) = 2x^3-3x^2-12x+5$ sur $\mathbb{R}$. (a) Variations + extrema. (b) Tangente en $0$.

**Corrigé :**
(a) 1. $f$ polynôme → dérivable sur $\mathbb{R}$ : $f'(x) = 6x^2-6x-12 = 6(x-2)(x+1)$.
2. Signe : $+$ puis $-$ puis $+$ → croissante sur $]-\infty,-1]$, décroissante sur $[-1,2]$, croissante sur $[2,+\infty[$.
3. $\boxed{\text{max local } f(-1) = 12}$ ; $\boxed{\text{min local } f(2) = -15}$ ($f'$ s'annule + change de signe ✔).
(b) $f(0) = 5$, $f'(0) = -12$ → $\boxed{y = -12x+5}$.
> بالدارجة: عمّل $f'$ ($6(x-2)(x+1)$) ← الإشارة باينة! القيم الحدية: حسب $f(-1)$ و$f(2)$ — الجدول بلا قيم ناقص! والمماس: الصيغة $y=f'(a)(x-a)+f(a)$ مباشرة.

## R2 — Asymptote oblique (2 méthodes !)
**Énoncé :** $f(x) = \frac{x^2+1}{x}$ sur $]0,+\infty[$. (a) Variations. (b) Montrer que $y = x$ est asymptote en $+\infty$.

**Corrigé :**
(a) $f'(x) = \frac{2x\cdot x-(x^2+1)}{x^2} = \frac{x^2-1}{x^2}$. Sur $]0,+\infty[$ : $-$ sur $]0,1[$, $+$ sur $]1,+\infty[$ →
$\boxed{\text{min } f(1) = 2}$. (Bonus : $\lim_{0^+}f = +\infty$ → asymptote verticale $x = 0$.)
(b) **Méthode 1 : division.** $f(x) = x + \frac{1}{x}$ → $f(x)-x = \frac{1}{x} \to 0$ → $\boxed{y=x\text{ asymptote}}$ (courbe au-dessus, écart $> 0$).
**Méthode 2 : limites.** $\frac{f(x)}{x} = \frac{x^2+1}{x^2} \to 1$, puis $f(x)-1\cdot x = \frac{1}{x} \to 0$. ✅ Même conclusion.
> بالدارجة: جوج طرق للمائل! **القسمة** ($x+\frac{1}{x}$ — سريعة للكسور) ولا **النهايات** ($f/x$ من بعد $f-ax$ — عامة). القسمة أسرع إلا كانت دالة كسرية!

## R3 — TVI + encadrement (balayage)

🏷️ matière=Math · année=— · session=— · chapitre=M2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Montrer que $f(x) = x^3+x-1$ s'annule une unique fois sur $\mathbb{R}$, et encadrer ce zéro $\alpha$ à $0,1$ près.

**Corrigé :**
1. $f$ polynôme → continue sur $\mathbb{R}$ ; $f'(x) = 3x^2+1 > 0$ → strictement croissante.
2. $\lim_{-\infty}f = -\infty$, $\lim_{+\infty}f = +\infty$ → $0$ est entre les deux → $\boxed{\text{unique } \alpha\in\mathbb{R}}$.
3. Balayage : $f(0) = -1 < 0$, $f(1) = 1 > 0$ → $\alpha\in]0,1[$ ; $f(0,6) = -0,184 < 0$, $f(0,7) = 0,043 > 0$ →
   $\boxed{\alpha\in]0,6\,;0,7[}$.
> بالدارجة: الوصفة: **اتصال + رتابة تامة + النهايات** = حل وحيد! ومن بعد **المسح** (balayage): جرب القيم حتى تحصر الصفر. $f(0,6)$ سالبة و$f(0,7)$ موجبة ← الصفر بيناتهم!

## R4 — Composée $e^x$ + asymptote horizontale

🏷️ matière=Math · année=— · session=— · chapitre=M2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** $f(x) = (x-1)e^x$ sur $\mathbb{R}$. (a) Variations. (b) Limites + asymptote éventuelle.

**Corrigé :**
(a) $f'(x) = e^x + (x-1)e^x = xe^x$. Signe = signe de $x$ ($e^x > 0$ toujours !) → décroissante sur $]-\infty,0]$,
$\boxed{\text{min } f(0) = -1}$, croissante sur $[0,+\infty[$.
(b) $\lim_{+\infty}f = +\infty$ ; $\lim_{-\infty}f = 0$ (croissances comparées : $xe^x\to 0$) →
$\boxed{y = 0\text{ asymptote horizontale}}$ (courbe en dessous : $f < 0$ sur $]-\infty,1[$).
> بالدارجة: $e^x$ ديماً موجبة ← الإشارة = إشارة $x$ بوحدو! والنهاية فـ $-\infty$ صفر (الأسي كيقتل الخطي) ← **مقارب أفقي**. لاحظ: هاد التمرين كيجمع الفصل 1 (النهايات) والفصل 2 (التغيرات) — بحال الوطني!

## R5 — Optimisation (le classique utile)

🏷️ matière=Math · année=— · session=— · chapitre=M2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Parmi tous les rectangles de périmètre $20\,m$, lequel a la plus grande aire ? (Justifier.)

**Corrigé :**
1. Côtés $x$ et $y$, $2x+2y = 20$ → $y = 10-x$, $x\in]0,10[$. Aire : $A(x) = x(10-x) = 10x-x^2$.
2. $A'(x) = 10-2x = 0$ → $x = 5$ ; $A'' = -2 < 0$ → maximum. $\boxed{\text{carré } 5\times5\,,\, A_{\max} = 25\,m^2}$.
> بالدارجة: مسائل التحسين (optimisation): **عبّر عن المطلوب بدالة واحدة** ← اشتق ← صفر المشتقة ← تحقق (هنا $A''<0$ = نهاية عظمى). والنتيجة جميلة: المربع كيربح! هاد النمط (مساحة/حجم أعظمي) كيتعاود بزاف!

## Question 6 — VRAIE (2020 R, Problème I + II.3)

🏷️ matière=Math · année=2020 · session=R · chapitre=M2 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Données :** $g(x) = e^{1-x}+\frac{1}{x}-2$ sur $]0,+\infty[$, puis $f$ (cf. ch.01 Q6 : $f(x) = (1-x)e^{1-x}-x^2+5x-3-2\ln x$).
**Énoncés officiels :** « Montrer que $g'(x) < 0$ sur $]0,+\infty[$ » ; « Déduire le signe de $g$ ($g(1) = 0$) » ;
« Montrer que $f'(x) = (x-2)g(x)$ » ; « Montrer que $f$ décroît sur $]0,1]$ et $[2,+\infty[$, croît sur $[1,2]$ ».
**Corrigé-type :**
1. $g'(x) = -e^{1-x}-\frac{1}{x^2} < 0$ (somme de 2 strictement négatifs !) → $g$ strictement décroissante ;
   $g(1) = 1+1-2 = 0$ → $\boxed{g > 0\text{ sur }]0,1[}$ et $\boxed{g < 0\text{ sur }]1,+\infty[}$.
2. $f'(x) = (x-2)e^{1-x}-2x+5-\frac{2}{x}$ ; or $(x-2)g(x) = (x-2)e^{1-x}+\frac{x-2}{x}-2x+4$ = même expression ✔ →
   $\boxed{f'(x) = (x-2)g(x)}$.
3. Signe $(x-2)\times$signe$(g)$ : $-$ sur $]0,1]$, $+$ sur $[1,2]$, $-$ sur $[2,+\infty[$ ✔.
> بالدارجة: هادي هي **تقنية المساعدة $g$** ديال الوطني! $g'$ سالبة باينة ($-e^{...}-1/x^2$ — جوج سوالب!) ← $g$ هابطة ← الإشارة من $g(1) = 0$! ومن بعد $f' = (x-2)g$ ← الإشارة = جداء إشارتين! اللي حاول يدرس إشارة $f'$ مباشرة بلا $g$ غرق!
> Source : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ — ✅ filière confirmée SP : l'en-tête officiel du corrigé (RR 22F) indique « شعبة العلوم التجريبية » (Sciences Expérimentales, مسلكا SVT + Sciences Physiques) : papier commun PC+SVT (le label « ST » d'AlloSchool/du fichier est une erreur d'étiquetage).

## VRAIE — 2025N Problème II (réciproque φ⁻¹ de $f(x) = x-\frac{(\ln x)^2}{x}$)

🏷️ matière=Math · année=2025 · session=N · chapitre=M2 · type=VRAIE · fidélité=reconstitué-corrigé · niveau=★★★ · barème=partie du Problème (11)

> ⚠️ Énoncé **reconstitué** depuis le mining Tier A du sujet intégral (scribd 878589899 : fonction, TVI, tangente, φ⁻¹ — formulation exacte des sous-questions à recouper). La fonction et les objets ($J$, tangente, $(\varphi^{-1})'$) sont Tier A ; la découpe Q1-Q4 suit le canevas national.
> Admis de l'étude (Partie I) : $f$ définie, continue et dérivable sur $]0,+\infty[$, $f'(x) = 1-\frac{2\ln x-(\ln x)^2}{x^2} > 0$ sur $]0,+\infty[$ (le terme soustrait est $< 0,29$ partout), $\lim_{0^+}f = -\infty$, $\lim_{+\infty}f = +\infty$, $f(1) = 1$, $f'(1) = 1$. On pose $\varphi = f$.

**Q1.** Montrer que $\varphi$ réalise une bijection de $]0,+\infty[$ sur un intervalle $J$ à déterminer.
**Q2.** On note $\varphi^{-1}$ sa réciproque. Déterminer $\varphi^{-1}(1)$ et $(\varphi^{-1})'(1)$.
**Q3.** Donner l'équation de la tangente $(T)$ à $C_\varphi$ au point d'abscisse $1$, puis celle de la tangente $(T')$ à $C_{\varphi^{-1}}$ au point d'abscisse $1$.
**Q4.** Tracer $C_{\varphi^{-1}}$ sur le même repère que $C_\varphi$ (justifier la construction).

**Corrigé-type :**
1. $\varphi$ continue (dérivable) et STRICTEMENT croissante ($f' > 0$) sur $]0,+\infty[$ → bijection sur $\boxed{J = ]\lim_{0^+}f,\lim_{+\infty}f[ = \mathbb{R}}$.
2. $\varphi^{-1}(1) = a \iff \varphi(a) = 1 \iff \boxed{a = 1}$ (car $f(1) = 1$). $\boxed{(\varphi^{-1})'(1) = \frac{1}{\varphi'(1)} = \frac{1}{1} = 1}$.
3. $(T)$ : $y = f'(1)(x-1)+f(1) = \boxed{y = x}$. Par symétrie $y = x$ : $(T')$ est la symétrique de $(T)$ ; or $(T) : y = x$ est invariante → $\boxed{(T') : y = x}$ (tangente au point $(1,1)$, fixe de la symétrie !).
4. $C_{\varphi^{-1}}$ = symétrique de $C_\varphi$ par rapport à la droite $y = x$ : chaque point $(a,b) \in C_\varphi$ donne $(b,a) \in C_{\varphi^{-1}}$ (ici $(1,1)$ fixe, tangente commune $y = x$).
> بالدارجة: الوصفة الوطنية للعكسية: **اتصال + رتابة تامة** ← تقابل! $J$ من النهايات ($-\infty$ لـ $+\infty$ = $\mathbb{R}$)! $\varphi^{-1}(1)$: قلب السؤال ($f(a) = 1$ ← $a = 1$)! المشتقة: **$1/f'$** ($1/1 = 1$)! والمماس: التناظر حول $y = x$ — وهنا $y = x$ ثابت ← المماس نفسو! والمنحنى: **نقطة بنقطة بالتناظر** ($(a,b)$ ← $(b,a)$)!

## R6 — ENTRAÎNEMENT (bijection + tangente symétrique, 2 méthodes !)

🏷️ matière=Math · année=— · session=— · chapitre=M2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★ · barème=—

**Énoncé :** $g(x) = x+\ln x$ sur $I = ]0,+\infty[$. (a) Montrer que $g$ est une bijection de $I$ sur $\mathbb{R}$. (b) Soit $h = g^{-1}$. Calculer $h(1)$ et $h'(1)$. (c) Tangente à $C_h$ en $(1,1)$ ?
**Corrigé :** (a) $g'(x) = 1+1/x > 0$ → strictement croissante, continue → bijection sur $J = ]\lim_{0^+}g,\lim_{+\infty}g[ = \boxed{\mathbb{R}}$ ($0^+ : -\infty$ ; $+\infty : +\infty$). (b) $h(1) = a \iff g(a) = 1$ ; $g(1) = 1+0 = 1$ → $\boxed{h(1) = 1}$ ; $\boxed{h'(1) = 1/g'(1) = 1/2}$. (c) **Méthode 1 (symétrie) :** tangente à $C_g$ en $(1,1)$ : $y = 2(x-1)+1 = 2x-1$ ; symétrique par $y=x$ : $x = 2y-1 \iff \boxed{y = \frac{x+1}{2}}$. **Méthode 2 (formule) :** $y = h'(1)(x-1)+h(1) = \frac{1}{2}(x-1)+1 = \boxed{\frac{x+1}{2}}$. ✅
> بالدارجة: $g = x+\ln x$: المشتقة $1+1/x$ موجبة ← تقابل على $\mathbb{R}$! $h(1)$: $g(1) = 1$ ← الجواب $1$! $h'(1) = 1/g'(1) = 1/2$! والمماس بجوج طرق: **التناظر** ($x = 2y-1$ ← $y = (x+1)/2$) ولا **الصيغة** ($y = h'(1)(x-1)+h(1)$) — نفس النتيجة!

## R7 — ENTRAÎNEMENT (réciproque EXPLICITE : résoudre $y = f(x)$)

🏷️ matière=Math · année=— · session=— · chapitre=M2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★ · barème=—

**Énoncé :** $f(x) = x^2+2x$ sur $I = [-1,+\infty[$. (a) Bijection sur $J$ ? (b) Exprimer $f^{-1}(y)$ explicitement. (c) Vérifier $(f^{-1})'(0) = 1/f'(0)$.
**Corrigé :** (a) $f'(x) = 2x+2 \ge 0$ sur $I$ (nulle en $-1$ seule) → strictement croissante → bijection sur $\boxed{J = [f(-1),+\infty[ = [-1,+\infty[}$. (b) $y = x^2+2x = (x+1)^2-1 \iff (x+1)^2 = y+1 \iff x+1 = +\sqrt{y+1}$ ($x \ge -1$ !) → $\boxed{f^{-1}(y) = -1+\sqrt{y+1}}$. (c) $(f^{-1})'(y) = \frac{1}{2\sqrt{y+1}}$ → $(f^{-1})'(0) = 1/2$ ; $1/f'(0) = 1/2$ ✔.
> بالدارجة: هنا العكسية عندها صيغة! $y = (x+1)^2-1$ ← $(x+1)^2 = y+1$ ← **الجذر الموجب** ($x \ge -1$!) ← $f^{-1}(y) = -1+\sqrt{y+1}$! اللي خدا $\pm$ نسى المجال! والتحقق: $(f^{-1})'(0) = 1/f'(0) = 1/2$ — الصيغة خدامة!

## 🪤 Pièges testés par question
- **R1** : $f(-1)$, $f(2)$ non calculés (tableau incomplet) ❌ ; tangente avec $f(0)$ faux ❌.
- **R2** : asymptote $y=x$ « devinée » sans $\lim(f-x) = 0$ ❌ ; signe de $f'$ sur $]0,+\infty[$ traité comme sur $\mathbb{R}$ ❌.
- **R3** : TVI sans continuité/monotonie ❌ ; encadrement sans valeurs numériques ❌ ; « $\alpha = 0,65$ » (le milieu n'est PAS le zéro !) ❌.
- **R4** : $(e^x)'$ avec $u'$ inventé ($e^x$ se dérive seul !) ❌ ; $\lim_{-\infty}(x-1)e^x = -\infty$ (oublier les CC !) ❌.
- **R5** : deux variables gardées jusqu'au bout (pas de réduction à $A(x)$) ❌ ; extremum sans vérification max/min ❌ ; domaine $]0,10[$ oublié ❌.
- **Q6** : $(1/x)' = +1/x^2$ (c'est $-1/x^2$ !) ❌ ; signe de $g$ sans utiliser $g(1) = 0$ ❌ ; $f'$ non factorisée par $(x-2)$ (signe illisible !) ❌.
- **2025N** : bijection sans continuité ❌ ; $J$ faux (limites $0^+$/$+\infty$ non lues ❌) ; $\varphi^{-1}(1)$ cherché par « formule » (utiliser $f(1) = 1$ !) ❌ ; $(T')$ sans la symétrie $y = x$ ❌.
- **R6** : $J = ]0,+\infty[$ (c'est l'image $]-\infty,+\infty[$ !) ❌ ; $h'(1) = g'(1) = 2$ (c'est $1/2$ !) ❌ ; symétrie $x\leftrightarrow y$ oubliée d'un côté ❌.
- **R7** : $x+1 = \pm\sqrt{y+1}$ (le signe $+$ imposé par $I$ !) ❌ ; $J$ sans $f(-1)$ ❌ ; $(f^{-1})'$ sans $1/2$ (dérivée de $\sqrt{}$ !) ❌.

---
*R1-R5 = type-bac ; Q6 = vraie nationale (2020 R, Problème). Backfill complémentaire : études verbatim sessions récentes (banque Fayssal : PDFs par thèmes 2011-2025, accès direct à finaliser).*
