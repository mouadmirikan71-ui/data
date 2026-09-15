---
chapitre: "01 - Limites et continuité"
unite: "S1 - Analyse de base"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "AlloSchool Maths 2BAC SP (Limites et continuité) + Manuel Massar Maths 2BAC SP + synthèse prof"
date_collecte: "2026-09-14"
type: "summary"
langues: "FR + Darija + LaTeX"
---

# Chapitre 01 — Limites et continuité

> 📋 **Exigible au bac (cadre de référence)** : Limites finies/infinies, opérations, formes indéterminées, limites usuelles, continuité, TVI + corollaire (solution unique), prolongement par continuité
> *Source : `00_Programme_officiel/programme_officiel.md` (v1 — à recouper avec le PDF officiel en Phase 3).*
*(CHAPITRE MODÈLE : même gabarit LaTeX + Darija pour les 13 autres)*

## 1. Accroche — l'intuition avant la formule 🎯

**FR :** Une limite, c'est la réponse à : « vers quoi se dirige $f(x)$ quand $x$ s'approche de quelque chose (un nombre, $+\infty$) ? » Imagine que tu marches vers un mur en faisant à chaque pas la moitié du chemin restant : tu t'approches sans jamais toucher — ta position a pour **limite** le mur. Toutes les définitions du chapitre disent exactement ça, en langage rigoureux.

**بالدارجة:** النهاية هي الجواب على سؤال: «فين غادية الدالة ملي $x$ كيقرب لشي حاجة؟» تخيل غادي للحيط وكل خطوة كتدير نص الطريق اللي بقات — كتقرب بلا ما توصل، البلاصة اللي غادي ليها هي **النهاية**. كل التعاريف ديال هاد الفصل كيقولو نفس الحاجة ولكن باللغة الدقيقة ديال الماط.

## 2. Résumé du cours (français + LaTeX, exigible au bac)

### 2.1 Limites usuelles (à savoir par cœur)
$$\lim_{x\to+\infty} x^n = +\infty,\quad \lim_{x\to+\infty} \frac{1}{x^n} = 0,\quad \lim_{x\to 0^+} \frac{1}{x} = +\infty,\quad \lim_{x\to 0^-} \frac{1}{x} = -\infty$$
$$\lim_{x\to+\infty} e^x = +\infty,\quad \lim_{x\to-\infty} e^x = 0,\quad \lim_{x\to+\infty} \ln x = +\infty,\quad \lim_{x\to 0^+} \ln x = -\infty$$

### 2.2 Opérations et formes indéterminées (FI)
- Somme/produit/quotient : tableaux d'opérations sur les limites (avec les signes !).
- Les 4 FI : $\frac{0}{0}$, $\frac{\infty}{\infty}$, $\infty - \infty$, $0 \times \infty$. **Une FI = on ne peut pas conclure, il faut transformer l'expression.**
- Techniques de levée (dans l'ordre à essayer) :
  1. **Factoriser** (polynômes, rationnelles : terme de plus haut degré en $\pm\infty$).
  2. **Quantité conjuguée** (différences de racines : multiplier haut et bas par le conjugué).
  3. **Taux d'accroissement** : $\lim_{x\to a}\frac{f(x)-f(a)}{x-a} = f'(a)$ (ex. $\lim_{x\to 0}\frac{\sin x}{x} = 1$, $\lim_{x\to 0}\frac{e^x-1}{x} = 1$, $\lim_{x\to 0}\frac{\ln(1+x)}{x} = 1$).
  4. **Croissances comparées** : $\lim_{x\to+\infty}\frac{e^x}{x^n} = +\infty$, $\lim_{x\to+\infty}\frac{\ln x}{x^n} = 0$ ($e^x$ écrase tout, $\ln$ est écrasé par tout).
  5. **Encadrement / gendarmes** : si $g \le f \le h$ et $g,h \to l$, alors $f \to l$ (classique : $-1 \le \sin x \le 1$).

### 2.3 Continuité
- $f$ est **continue en $a$** si $\lim_{x\to a} f(x) = f(a)$ (la courbe « ne se lève pas le crayon »).
- Continues sur leur domaine : polynômes, rationnelles (là où définies), $\sin$, $\cos$, $e^x$, $\ln$, racines — **à justifier en une ligne** (« $f$ est continue sur $I$ comme ... »).
- **Prolongement par continuité** : si $f$ n'est pas définie en $a$ mais $\lim_{x\to a}f(x) = l$ finie, on pose $g(a) = l$ et $g = f$ ailleurs.

### 2.4 Théorème des valeurs intermédiaires (TVI) — le théorème star du national ⭐
- **TVI** : si $f$ continue sur $[a,b]$, alors pour tout $k$ entre $f(a)$ et $f(b)$, il existe **au moins** $c \in [a,b]$ tel que $f(c) = k$.
- **Corollaire (solution unique)** : si de plus $f$ est **strictement monotone** sur $[a,b]$, alors $c$ est **unique**.
- **Pourquoi il existe** : c'est la version rigoureuse de « une courbe continue qui passe du dessous au dessus d'une droite $y = k$ doit forcément la couper ». Sans continuité, la courbe pourrait « sauter » par-dessus !
- Rédaction-type (à recopier) : ① $f$ continue sur $I$ car... ② $f$ strictement monotone (tableau/signe de $f'$)... ③ $k \in$ intervalle des valeurs... ④ « Donc d'après le corollaire du TVI, l'équation $f(x) = k$ admet une **unique** solution $\alpha \in I$. »

### 2.5 Asymptotes lues sur les limites (pont vers Ch.02)
- $\lim_{x\to a} f = \pm\infty$ → asymptote **verticale** $x = a$.
- $\lim_{x\to\pm\infty} f = l$ (finie) → asymptote **horizontale** $y = l$.
- $\lim_{x\to\pm\infty} [f(x) - (ax+b)] = 0$ → asymptote **oblique** $y = ax + b$.

### 2.6 Lecture graphique (lire une courbe comme au national) 📈
- **Lire une limite sur un graphe** : suivre la courbe des yeux vers la zone demandée ($a^+$, $a^-$, $+\infty$). Point **creux** (○) = valeur approchée mais non atteinte ; point **plein** (●) = valeur prise. Si la courbe « explose » vers le haut/bas près de $x = a$ → limite infinie → asymptote verticale.
- **Reconnaître les asymptotes** : verticale = la courbe colle à une droite $x = a$ sans la traverser (en général) ; horizontale = la courbe s'aplatit vers un palier $y = l$ ; oblique = la courbe suit une droite penchée au loin (à confirmer par le calcul $\lim[f(x)-(ax+b)] = 0$).
- **TVI en image** : une courbe continue entre $A(a, f(a))$ et $B(b, f(b))$ est un trait sans lever le crayon — toute droite horizontale $y = k$ coincée entre les deux hauteurs **coupe forcément** le trait. Si le trait monte/descend toujours (monotonie), il ne coupe qu'**une fois** → solution unique.
- **Méthode réflexe (3 questions)** : ① Que vois-tu ? (décrire : monte, sature, explose...) ② Que dit le calcul ? (limite, signe, TVI...) ③ Les deux sont-ils cohérents ? (si non → erreur de calcul probable).
- ⚠️ **Piège** : une fenêtre graphique trompeuse (mauvaise échelle) peut suggérer une fausse limite — le graphe **illustre**, seul le calcul **prouve**. Ne jamais justifier par « on voit sur la figure » sans calcul.
- بالدارجة: المنحنى كيقرا بالعين قبل الحساب — شوف فين غادية (طالعة؟ مثبتة؟ منفجرة؟)، عاد أكد بالحساب. النقطة المخوية (○) = القيمة مقصودة ولكن ما محققةش، والنقطة العامرة (●) = محققة. والـ TVI بالصورة: خط متواصل من التحت للفوق **ضروري يقطع** أي خط أفقي فالوسط!

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** هاد الفصل فيه جوج أسئلة فقط:
1. **النهايات:** فين غادية الدالة؟ (كتطلع للسما؟ كتهبط؟ كتستقر فشي عدد؟)
2. **الاتصال:** واش المنحنى مرسوم بلا ما نهز القلم؟ (إلا هزيتي القلم = انقطاع)

**الأشكال غير المحددة (FI):** ملي كتعوض وكتلقى $\frac{0}{0}$ ولا $\frac{\infty}{\infty}$، صافي راه **ماشي الجواب** — هادي غير إشارة تقول ليك «بدل الطريقة»! الحلول بالترتيب:
- كاين كثير حدود؟ **عمّل** (factoriser) واختزل.
- كاين الجذر؟ ضرب فالمرافق (الكمية المرافقة).
- كاين $\sin x / x$ ولا $(e^x-1)/x$؟ هادو محفوظين = 1 (معدل التغير).
- كاين $e^x$ ضد $x^n$ ضد $\ln x$؟ **الأُسّي كيربح ديماً، واللوغاريتم كيخسر ديماً** — حفظها بحال ترتيب القوة: $e^x \gg x^n \gg \ln x$.

**مبرهنة القيم الوسطية (TVI):** تخيل طالع فالدروج من الطابق 1 للطابق 5 — ضروري تدوز من الطوابق 2, 3, 4! ما يمكنش تقفز من 1 لـ 5 بلا ما تدوز من الوسط. هادي هي الـ TVI: الدالة المتصلة اللي كطلع من تحت لفوق **ضروري تقطع** أي خط فالوسط. وعلاش مهمة فالوطني؟ حيت هي الطريقة الرسمية باش تبرهن أن معادلة عندها **حل وحيد** — كتستعملها فكل مسألة تحليل تقريباً!

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ فالقسم — خطوة بخطوة)*

**الخطوة 1 — سول راسك: شنو كتسول عليه النهاية؟**
أي نهاية = «فين غادية؟». قبل ما تحسب، **توقع**: $x$ كبير بزاف؟ الدالة كتكبر ولا كتصغر؟ هاد التوقع كيحميك من الأجوبة الحمقة (بحال نهاية موجبة تخرج ليك سالبة).

**الخطوة 2 — عوض أولاً، وفكر ثانياً.**
القاعدة: عوض القيمة وشوف شنو خرج. خرج عدد عادي؟ صافي ساليتي. خرج شكل غير محدد؟ **ما تكتبوش كجواب** — دخل للأسلحة بالترتيب: تعميل ← مرافق ← نهايات محفوظة ← المقارنة. 90% ديال تمارين الوطني كيتحلو بواحد من هاد الربعة.

**الخطوة 3 — الاتصال = جسر للـ TVI.**
ما تحفظش الاتصال بوحدو — فهمو كـ **شرط**: بلا اتصال ما كايناش TVI، وبلا TVI ما تقدرش تبرهن الحل الوحيد. السلسلة: اتصال + رتابة + القيمة محصورة = حل وحيد مضمون. هادي هي الجملة اللي كتجيب النقاط!

**الخطوة 4 — تشبيه واحد يعاونك.**
**الدروج والطوابق:** الدالة المتصلة بحال الدروج — ما يمكنش توصل للفوق بلا ما تدوز من الوسط. الدالة المنقطعة بحال المصعد — كتقفز! ملي تشوف سؤال «بين أن المعادلة تقبل حلاً وحيداً»، فكر مباشرة: **فين هما الدروج؟** (الاتصال + الرتابة).

**الخطوة 5 — ثبت بالمحفوظات.**
هاد النهايات خاصك تعرفهم بالنعاس: $\frac{\sin x}{x}\to 1$، $\frac{e^x-1}{x}\to 1$، $\frac{\ln(1+x)}{x}\to 1$، $e^x/x^n \to +\infty$، $\ln x / x^n \to 0$. أي تمرين نهايات صعيب غالباً مخبي وحدة من هادو!

## 5. Définitions & théorèmes clés (FR + Darija)

| Notion FR (LaTeX) | Énoncé FR | بالدارجة |
|---|---|---|
| Limite | $\lim_{x\to a}f(x) = l$ : $f(x)$ se rapproche de $l$ quand $x$ se rapproche de $a$ | فين غادية الدالة ملي $x$ كيقرب |
| FI | $\frac00, \frac\infty\infty, \infty-\infty, 0\times\infty$ : formes sans conclusion directe | علامة «بدل الطريقة» ماشي الجواب |
| Continuité en $a$ | $\lim_{x\to a}f(x) = f(a)$ | مرسومة بلا ما تهز القلم |
| TVI | $f$ continue sur $[a,b]$ + $k$ entre $f(a),f(b)$ ⟹ $\exists c : f(c) = k$ | طالع الدروج؟ ضروري تدوز من الوسط |
| Corollaire TVI | + stricte monotonie ⟹ $c$ **unique** | الدروج بلا رجوع = طابق واحد فقط |
| Croissances comparées | $e^x \gg x^n \gg \ln x$ en $+\infty$ | الأسي أقوى واحد، اللوغاريتم أضعف واحد |
| Gendarmes | $g \le f \le h$, $g,h \to l$ ⟹ $f \to l$ | محصور بين جوج غادين لنفس البلاصة = تابعهم |

## 6. FAQ du chapitre (vraies questions d'élèves)

**Q1. $\frac{0}{0} = 1$ ? $\frac{\infty}{\infty} = 1$ ?**
**NON !** Ce sont des FI : le résultat dépend du cas ($x/x \to 1$ mais $x^2/x \to 0$). Il faut lever l'indétermination.
**لا!** هادو أشكال غير محددة — النتيجة كتبدل على حساب التمرين، خاصك تخدم باش تجبدها.

**Q2. Quand utiliser la quantité conjuguée ?**
Dès qu'une FI contient une **différence de racines** ($\sqrt{a} - \sqrt{b}$) ou racine moins nombre. On multiplie par le conjugué pour faire apparaître $(a-b)$.
ملي تشوف الفرق ديال الجذور — ضرب فالمرافق باش يبان الفرق ديال ما تحت الجذر.

**Q3. Pourquoi $\lim \frac{\sin x}{x} = 1$ seulement en 0 ?**
Parce que c'est le taux d'accroissement de $\sin$ en 0 (= $\cos 0 = 1$). Ailleurs, pas de FI en général.
حيت هادي هي النسبة ديال التغير ديال $\sin$ فنقطة 0 — فبلايص أخرين ما كايناش هاد الخاصية.

**Q4. TVI ou corollaire : lequel citer ?**
« Il existe (au moins) une solution » → TVI. « **Unique** solution » → **corollaire** (+ monotonie stricte à prouver !).
«يوجد حل» = TVI. «حل **وحيد**» = اللازمة + إثبات الرتابة!

**Q5. Faut-il vraiment justifier la continuité avant le TVI ?**
**OUI, c'est éliminatoire.** « $f$ est continue sur $[a,b]$ comme somme/composée de fonctions continues... » — une ligne qui vaut des points.
**إيه، إجباري!** سطر واحد على الاتصال كيجيب النقاط وبلا بيه الجواب ناقص.

**Q6. $\lim_{x\to 0} \frac{1}{x}$ : pourquoi pas de limite ?**
Limites à gauche ($-\infty$) et à droite ($+\infty$) **différentes** → pas de limite (globale) en 0. Toujours séparer $0^+$ et $0^-$ !
النهاية من اليمين واليسار مختلفين — ملي كيكونو مختلفين ما كايناش نهاية!

## 7. Pièges classiques + mots-clés obligatoires ⚠️

**À écrire absolument** : « forme indéterminée », nom de la technique (« par factorisation / quantité conjuguée / croissances comparées / gendarmes »), « $f$ est continue sur ... car ... », « d'après le corollaire du TVI », $\boxed{\text{résultat}}$.
**Erreurs fréquentes** :
- Conclure sur une FI sans transformation ❌. - Oublier de séparer $0^+$ / $0^-$ ❌.
- TVI sans continuité ni monotonie ❌. - $\sqrt{x^2} = x$ (c'est $|x|$) ❌.
- Appliquer les croissances comparées en $-\infty$ ou en 0 (elles sont en $+\infty$ !) ❌.

## 8. Sources de ce chapitre
- AlloSchool — Maths 2BAC SP, sections « Limites et continuité » (cours + exercices). Accès : 2026-09-14. https://www.alloschool.com/course/mathematiques-2eme-bac-sciences-physiques-biof
- Manuel Massar / Fadaa Maths 2BAC SP — Ch. Limites et continuité (transcription originale).
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-14.
- Note P2 : papiers nationaux Maths-PC en cours de localisation (section AlloSchool 5321 = filière ST uniquement ; le national PC partage l'épreuve « Sciences Expérimentales » avec SVT — à confirmer). `EXERCICES_TYPES.md` = banque type-bac étiquetée en attendant (backfill verbatim prévu).

## 9. 🚀 Pour aller plus loin — le pourquoi que les manuels sautent (niveau maître)

**P1. Pourquoi $0,999\ldots = 1$ EXACTEMENT (et pourquoi on n'y croit pas) ?**
Par les suites géométriques (niveau PC !) : $0,999\ldots = 9(0,1 + 0,01 + 0,001 + \ldots) = 9 \times \frac{0,1}{1-0,1} = 9 \times \frac{1}{9} = 1$. Égalité **exacte**, pas approximation ! L'incrédulité vient d'une confusion : on imagine le *processus* (ajouter des 9 indéfiniment) au lieu du *nombre* (la limite du processus). Une limite n'est pas « presque » : quand l'écart peut devenir plus petit que n'importe quel $10^{-n}$, l'écart **est** zéro. C'est toute la philosophie du chapitre en une égalité.
بالدارجة: $0,999... = 1$ **بالضبط** ماشي تقريباً! البرهان بالمتتالية الهندسية (شوف الحساب الفوق). والسبب اللي كيخلينا ما نتيقوش: كنخلطو بين **المسار** (زيادة التسعات بلا نهاية) و**العدد** (النهاية ديال المسار). النهاية ماشي «تقريباً» — ملي الفرق كيصغار من أي عدد تتخيلو، الفرق **هو** الصفر!

**P2. Les FI ne sont pas des erreurs : ce sont des MATCHS à arbitrer.**
$0/0$ = deux fonctions qui courent vers 0 : **qui arrive « le plus vite » ?** $\frac{x^2}{x} \to 0$ (le numérateur gagne la course vers 0) ; $\frac{x}{x^2} \to +\infty$ (le dénominateur gagne) ; $\frac{7x}{3x} \to \frac{7}{3}$ (match nul → score = rapport des vitesses). Chaque technique de levée (factorisation, conjuguée, taux, croissances comparées) n'est qu'une façon d'**arbitrer le match**. Et l'échelle des vitesses à l'infini : $e^x \gg x^n \gg \ln x$ (« $\gg$ » = gagne toujours). Deviner le gagnant AVANT de calculer transforme les limites en jeu d'intuition.
بالدارجة: الشكل غير المحدد ماشي غلطة — هو **ماتش** بين جوج دوال! شكون كيوصل اللول للصفر؟ $x^2$ كتغلب $x$ (النتيجة 0)، و$x^2$ فالمقام كتغلب (النتيجة $\infty$). وكل تقنية ما هي إلا **تحكيم الماتش**. وسلم القوة: $e^x$ كتغلب الكل، و$\ln$ كتخسر ضد الكل — توقع الرابح قبل الحساب!

**P3. Pourquoi le TVI EXIGE la continuité ? (le contre-exemple qui tue)**
Prenez $f(x) = -1$ si $x < 0$, $+1$ si $x \geq 0$ : elle « passe » de $-1$ à $+1$ sans JAMAIS valoir $0$ — le **saut** en $0$ permet d'éviter toutes les valeurs intermédiaires ! La continuité, c'est exactement **l'interdiction de sauter**. Et la monotonie stricte pour l'unicité ? Sans elle, la courbe peut onduler et recouper $y = k$ trois fois (TVI vérifié, 3 solutions !). Résumé : continuité = *on traverse*, monotonie = *on ne traverse qu'une fois*.
بالدارجة: الدالة اللي كتقفز كتقدر **تدوز من فوق القيمة** بلا ما تاخدها! الاتصال = **ممنوع القفز**. والرتابة = **ممنوع الرجوع** (بلا بيها المنحنى كيتموج وكيقطع الخط 3 مرات — TVI كاين ولكن الحلول 3!). الاتصال كيضمن العبور، والرتابة كتضمن التفرد.

**🔗 Vrais ponts (cross-links) :**
- → **SVT-02 §2.4 (myogramme)** : lire phases/amplitude/durées sur une courbe = exactement le geste du §2.6 ici. Même méthode « décrire → relier → conclure », deux matières.
- → **PC-08/09/10 (cinématique)** : la vitesse instantanée $v = \lim_{\Delta t \to 0}\frac{\Delta x}{\Delta t}$ EST un taux d'accroissement = une limite ! La physique utilise ce chapitre partout sans le dire — le Ch.02 (dérivation) naît formellement ici.
- → **Math-03 (suites, à venir)** : $\lim_{n\to+\infty} u_n$ = même machinerie (opérations, FI, gendarmes) avec $n$ entier au lieu de $x$ réel.

## 10. 😶‍🌫️ Les confusions garanties (quand les yeux se voilent)

**C1. « Limite en $a$ = valeur $f(a)$, toujours »** — Non : la limite décrit l'**approche**, $f(a)$ la **position**. Contre-exemple : $f(x) = \frac{x^2-1}{x-1}$ ($x \neq 1$) : $\lim_{x\to 1}f = 2$ mais $f(1)$ **n'existe pas** (trou !). La limite « s'en fiche » du point lui-même. Test : « $f(2)$ n'existe pas ; la limite en 2 peut-elle exister ? » → Oui !
**C2. « $\infty$ est un (grand) nombre »** — Non : c'est un **comportement**, pas un nombre. $\infty - \infty = 0$ ? Contre-exemples : $x - (x-5) \to 5$ ; $x^2 - x \to +\infty$ ; $x - x^2 \to -\infty$. Trois réponses différentes pour « le même » $\infty - \infty$ ! On ne calcule jamais avec $\infty$ comme avec $10^{100}$.
**C3. « TVI = solution unique »** — Non : TVI seul = **existence** (au moins une). L'**unicité** exige la **monotonie stricte** en plus. Formule : « TVI = ticket d'existence, monotonie = fauteuil unique. » Dessin mental : courbe en vagues coupant 3 fois (TVI ✔, 3 solutions, pas d'unicité).

## 11. 🧭 Signaux adaptatifs (pour l'AI teacher)

**Carte des prérequis (ordre obligatoire) :**
`calcul algébrique (FACTORISATION !) → limites usuelles → opérations + signes → FI + techniques → continuité → TVI + corollaire → lecture graphique`
- Si l'élève bloque sur les **FI** → redescendre à la **factorisation** (80 % des échecs sont de l'algèbre, pas de l'analyse !).
- Si l'élève bloque sur le **TVI** → vérifier les **2 hypothèses séparément** (continuité PUIS monotonie — il en oublie toujours une).
- Si l'élève mélange **$0^+$/$0^-$** → revenir au **tableau de signes** (la limite suit le signe).

**🔄 Angle de secours (si les FI ne passent pas) : le match + l'échelle des vitesses.**
Oublie les techniques 5 minutes : pour chaque FI, demander « **qui gagne la course ?** » avec l'échelle $e^x \gg x^n \gg \ln x$ ($\gg$ = gagne toujours). $\frac{x^2}{e^x}$ ? « $e^x$ gagne » → $0$. $\frac{\ln x}{x}$ ? « $x$ gagne » → $0$. L'élève DEVINE juste avant de savoir prouver — ensuite seulement, montrer que chaque technique (factorisation, conjuguée, taux…) n'est que la preuve formelle du résultat deviné. L'intuition d'abord, la rigueur après : c'est dans cet ordre que ça colle.
