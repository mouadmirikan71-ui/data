---
chapitre: "13 - Dénombrement"
unite: "S4 - Dénombrement et probabilités"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (canon national : A/C/P, Pascal, binôme de Newton)"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 13 — Dénombrement

> 📋 **Exigible au bac** : $A_n^p = \frac{n!}{(n-p)!}$ (ordre, sans répétition) ; $P_n = n!$ ; $C_n^p = \frac{n!}{p!(n-p)!}$ (sans ordre) ; $n^p$ (p-listes, avec répétition) ; Pascal $C_n^p = C_{n-1}^p + C_{n-1}^{p-1}$ ; binôme $(a+b)^n = \sum_{k=0}^{n} C_n^k a^{n-k}b^k$ ; $2^n$ parties.

## 1. Accroche — le cadenas et la salade 🔐🥗

Un cadenas à 3 chiffres : l'ordre compte (1-2-3 ≠ 3-2-1) → **arrangement**. Une salade de 3 fruits : l'ordre ne compte pas (pomme-poire-banane = banane-pomme-poire) → **combinaison**. Tout le dénombrement tient en DEUX questions : **(1) l'ordre compte-t-il ? (2) peut-on répéter ?** Deux oui/non → 4 cases → 4 formules. Le reste, c'est du calcul.

> بالدارجة : القفل بالأرقام : الترتيب مهم (1-2-3 ماشي 3-2-1) ← **ترتيب**. الشلادة بالفواكه : الترتيب ما مهمش ← **توفيقة**. كاع العدّ كيتلخص في جوج أسئلة : **(1) واش الترتيب مهم ؟ (2) واش التكرار مسموح ؟** جوج نعم/لا ← 4 خانات ← 4 صيغ. الباقي غير حساب.

## 2. Résumé du cours (exigible au bac)

**Principes.** **Multiplicatif** : $n_1$ choix puis $n_2$ choix → $n_1 \times n_2$ (cases successives : multiplier). **Additif** : cas disjoints → additionner (« OU » = $+$, « ET » = $\times$). **Complémentaire** : « au moins un » = total $-$ « aucun » (souvent 10× plus rapide !).

**Les 4 cases (tableau maître) :**

| | Sans répétition | Avec répétition |
|---|---|---|
| **Ordre compte** | **Arrangements** $A_n^p = \frac{n!}{(n-p)!}$ | **p-listes** $n^p$ |
| **Ordre sans importance** | **Combinaisons** $C_n^p = \frac{n!}{p!(n-p)!}$ | (hors programme) |

**Cas particuliers :** $P_n = n!$ (permutations : ranger $n$ objets) ; $C_n^0 = C_n^n = 1$, $C_n^1 = n$, symétrie $C_n^p = C_n^{n-p}$ (choisir $p$ = écarter $n-p$).

**Mots-signaux (bac) :** « tirage **simultané** » / « poignée » / « comité » / « ensemble » → **combinaison** (pas d'ordre) ; « tirage **successif sans remise** » / « podium » / « code » (chiffres distincts) → **arrangement** ; « successif **avec remise** » / « code » (répétitions) / « mot » → **p-liste** $n^p$.

**Pascal + binôme.** $\boxed{C_n^p = C_{n-1}^p + C_{n-1}^{p-1}}$ (triangle de Pascal : chaque case = somme des 2 au-dessus). **Newton :** $\boxed{(a+b)^n = \sum_{k=0}^{n} C_n^k a^{n-k}b^k}$. Applications : $(1+1)^n = 2^n$ (nombre de **parties** d'un ensemble à $n$ éléments) ; $(1-1)^n = 0$ (autant de parties paires qu'impaires).

**Factorielle (calcul) :** $n! = n(n-1)\cdots1$ ; simplifier AVANT de calculer : $\frac{10!}{8!} = 10 \times 9 = 90$ (jamais $3628800/40320$ !).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**المبادئ :** **الضرب** : $n_1$ اختيار من بعد $n_2$ ← $n_1 \times n_2$ («و» = $\times$). **الجمع** : حالات منفصلة ← الجمع («أو» = $+$). **المتمم** : «على الأقل واحد» = المجموع $-$ «حتى واحد» (أسرع 10 مرات !).

**الخانات الأربعة :** الترتيب مهم + بلا تكرار ← **ترتيبات** $A_n^p = \frac{n!}{(n-p)!}$ | الترتيب مهم + بالتكرار ← **قوائم** $n^p$ | الترتيب ما مهمش + بلا تكرار ← **توفيقات** $C_n^p = \frac{n!}{p!(n-p)!}$. الحالات الخاصة : $P_n = n!$ (صفّ $n$ أشياء) ؛ $C_n^p = C_n^{n-p}$ (تختار $p$ = تقصي $n-p$).

**كلمات-الإشارة :** «سحب **آني**» / «لجنة» / «مجموعة» ← **توفيقة** ؛ «سحب **تتابعي بلا إرجاع**» / «منصة» ← **ترتيب** ؛ «**مع الإرجاع**» / «رمز» ← **قائمة** $n^p$.

**باسكال + ثنائي الحد :** $C_n^p = C_{n-1}^p + C_{n-1}^{p-1}$ (مثلث باسكال). **نيوتن :** $(a+b)^n = \sum C_n^k a^{n-k}b^k$. التطبيقات : $2^n$ (عدد الأجزاء) ؛ $(1-1)^n = 0$.

**العاملي (الحساب) :** بسّط **قبل** ما تحسب : $\frac{10!}{8!} = 10 \times 9 = 90$ (عمرك ما تحسب $3628800/40320$ !).

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — سول جوج أسئلة، ديما.** أي تمرين عدّ : **(1) الترتيب مهم ؟** بدّل ترتيب عنصرين : إلا تبدلات النتيجة ← مهم (سطر الفوق : $A$ ولا $n^p$). **(2) التكرار مسموح ؟** واش نفس العنصر يقدر يتعاود ؟ إيه ← العمود اليمين ($n^p$ ولا خارج البرنامج). بجوج لا ← توفيقة $C_n^p$ (الحالة الأكثر شيوعاً في الباك !).

**الخطوة 2 — مثال يوضح كلشي.** صندوق فيه 5 كرات : سحب 3 **دقة وحدة** (آني) ← الترتيب ما مهمش + بلا تكرار ← $C_5^3 = 10$. سحب 3 **وحدة بوحدة بلا إرجاع** ← الترتيب مهم ← $A_5^3 = 60$. **مع الإرجاع** ← $5^3 = 125$. نفس الصندوق، ثلاثة أجوبة — الفرق كلو في السؤالين !

**الخطوة 3 — «على الأقل» = المتمم.** «لجنة من 4 فيها على الأقل امرأة واحدة» : الحساب المباشر (1 + 2 + 3 + 4 نساء) طويل. **المتمم** : المجموع $-$ «صفر نساء» = $C_{10}^4 - C_6^4$ (إلا كانو 6 رجال). **القاعدة : «على الأقل/الأكثر» ← فكّر في المتمم اللول.**

**الخطوة 4 — العاملي : بسّط، ما تحسبش.** $C_{10}^3 = \frac{10!}{3!7!} = \frac{10\times9\times8}{3\times2\times1} = 120$. **الطريقة** : الفوق $p$ عوامل من $n$ نازل، التحت $p!$ : $\frac{10\times9\times8}{6}$. عمرك ما تكتب العاملي كامل !

**الخطوة 5 — ثنائي الحد : $(a+b)^n$ كتفكك.** $(x+1)^4 = C_4^0x^4 + C_4^1x^3 + C_4^2x^2 + C_4^3x + C_4^4$ $= x^4 + 4x^3 + 6x^2 + 4x + 1$. **المعاملات = سطر باسكال** (1-4-6-4-1). والأسس : $x$ نازل ($4\to0$)، الثاني طالع ($0\to4$).

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Factorielle $n!$ | العاملي | $n(n-1)\cdots1$ (simplifier avant !) |
| Arrangement $A_n^p$ | الترتيب | ordre + sans répétition : $n!/(n-p)!$ |
| Permutation $n!$ | التبديلة | ranger $n$ objets |
| Combinaison $C_n^p$ | التوفيقة | sans ordre : $n!/(p!(n-p)!)$ |
| p-liste $n^p$ | القائمة | ordre + répétition |
| « Simultané » | الآني | mot-signal : combinaison |
| Pascal | باسكال | $C_n^p = C_{n-1}^p + C_{n-1}^{p-1}$ |
| Binôme de Newton | ثنائي نيوتن | $(a+b)^n = \sum C_n^k a^{n-k}b^k$ |

## 6. FAQ du chapitre

**1. $A$ ou $C$ — comment trancher en 5 secondes ?** Échange deux éléments : résultat différent → $A$ (ordre) ; identique → $C$. Comité/loto/sac → $C$ ; podium/code/classement → $A$. / بدّل عنصرين : تبدلات النتيجة ← $A$ ؛ نفس الشي ← $C$.

**2. Pourquoi $C_n^p = A_n^p/p!$ ?** $A_n^p$ compte les tirages ORDONNÉS ; chaque paquet de $p$ objets admet $p!$ ordres → on divise par $p!$ pour « oublier » l'ordre. / $A$ كيحسب بالترتيب ؛ كل مجموعة عندها $p!$ ترتيبات ← قسّم باش تنسى الترتيب.

**3. Pourquoi $2^n$ parties ?** Chaque élément : 2 choix (dedans/dehors) → $2\times2\cdots\times2 = 2^n$. (Et $(1+1)^n = \sum C_n^k = 2^n$ le confirme.) / كل عنصر : جوج اختيارات (داخل/خارج) ← $2^n$.

**4. « Au plus 2 » : direct ou complémentaire ?** Ici direct (0, 1, 2 : 3 cas) vs complémentaire (3, 4, … : plus long si $n$ grand). Règle : compter les cas des 2 côtés, choisir le plus court. / حسب الحالات من الجهتين واختار الأقصر.

**5. $(x-1)^n$ avec Newton ?** $(x + (-1))^n$ : signes alternés $(-1)^k$. Ex : $(x-1)^3 = x^3 - 3x^2 + 3x - 1$. / $(x+(-1))^n$ : الإشارات كتتعاقب.

**6. $0! = 1$ ?** Par convention (cohérence : $C_n^0 = n!/(0!n!) = 1$ exige $0! = 1$ ; et $1! = 1\times 0!$). / بالاتفاق (باش $C_n^0 = 1$ تصدق).

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **$A$ au lieu de $C$** (ou inverse) : 80 % des erreurs. Réflexe : *le test d'échange* (5 secondes, infaillible).
- 🪤 **« Au moins un » en direct** : $C + C + C + \cdots$ interminable et faux (doubles comptes !). Complémentaire : total $-$ aucun.
- 🪤 **Double comptage** : « choisir un président PUIS un comité le contenant » compte chaque comité plusieurs fois. Ordonner les choix (le cas particulier d'abord, sans chevauchement).
- 🪤 **Factorielles calculées** : $10!/8!$ à la calculatrice = erreurs + temps. Simplifier : $10 \times 9$.
- Mots-clés : *ordre ? répétition ? simultané/successif, complémentaire, simplifier $n!$, ligne de Pascal.*

## 8. Sources de ce chapitre

- Canon national 2BAC SP (4 cases, Pascal, Newton) — synthèse prof ; pont M14 (probabilités : $cardA/card\Omega$).

## 9. Le « pourquoi » profond — pourquoi 4 formules seulement 🔬

**Pourquoi $C_n^p = n!/(p!(n-p)!)$ ?** Construis en 2 temps : (1) range $p$ objets distincts pris parmi $n$ : $A_n^p = n(n-1)\cdots(n-p+1)$ choix ordonnés ; (2) chaque ensemble de $p$ a été compté $p!$ fois (ses ordres) → diviser par $p!$. Le dénominateur $p!(n-p)!$ raconte l'histoire : $(n-p)!$ = « oublier les non-choisis », $p!$ = « oublier l'ordre ». **Compter = construire puis quotienter par les symétries.**

**Pourquoi le triangle de Pascal marche ?** $C_n^p$ = choisir $p$ parmi $n$. Isoler le $n$-ième élément : soit on le prend (reste $C_{n-1}^{p-1}$), soit non (reste $C_{n-1}^p$). Ces 2 cas disjoints partitionnent → somme. Chaque identité combinatoire est une **histoire de tri** : « avec/sans $x$ ».

**Pourquoi $(a+b)^n$ fait apparaître $C_n^k$ ?** Développer $(a+b)(a+b)\cdots(a+b)$ : chaque terme choisit $a$ ou $b$ dans chaque parenthèse. Le terme $a^{n-k}b^k$ = « choisir les $k$ parenthèses qui donnent $b$ » = $C_n^k$ façons. **Newton = dénombrement déguisé en algèbre** — et $(1+1)^n = 2^n$ en est le cadeau.

**Liens croisés :** M14 — $p =$ cas favorables / cas possibles : TOUTE proba d'équiprobabilité est un quotient de dénombrements ; M03 — suites et récurrences : Pascal est une récurrence double ; info/PC — $2^n$ : bits, états microscopiques (entropie !) ; M09 — $\int$ vs $\sum$ : compter (discret) puis intégrer (continu), même instinct.

## 10. Les 3 confusions qui coûtent des points 😵

**1. « Tirage successif → $A$, toujours. »** Avec remise, c'est $n^p$ (p-liste), pas $A$ ! **Le déclic :** *successif SANS remise = $A$ ; successif AVEC remise = $n^p$.* Le mot « remise » change tout — le surligner dans l'énoncé.

**2. « Au moins une boule rouge : $C$ (rouges) $\times$ $C$ (reste). »** Faux : chevauchements (2 rouges comptées 2 fois : une comme « la » rouge, une dans le reste). **Le déclic :** *« au moins » = complémentaire (total $-$ aucun), JAMAIS de multiplication directe.* Teste avec un mini-cas ($n = 3$) pour sentir le double compte.

**3. « $(x+2)^3 = x^3 + 6x^2 + \cdots$ : le 2 ne change que… »** Si : $(x+2)^3 = \sum C_3^k x^{3-k}2^k = x^3 + 6x^2 + 12x + 8$ — le $2^k$ multiplie CHAQUE terme ($C_3^1 \times 2 = 6$, $C_3^2 \times 4 = 12$). **Le déclic :** *Newton : $a^{n-k}b^k$ — les DEUX bases portent des puissances, pas seulement $x$.*

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** factorielles (calcul mental : $5! = 120$), fractions (simplifications), ensembles ($\cup$, $\cap$, complémentaire). **Test 30 s :** $C_5^2 = 10$ ; $A_5^2 = 20$ ; $\frac{7!}{5!} = 42$.

**Plan B — le plus dur (choisir la bonne formule) :** face à l'énoncé : ① souligner simultané/successif/remise ; ② test d'échange (ordre ?) ; ③ « au moins/au plus » → complémentaire ? ; ④ écrire la formule AVANT les nombres ($C_{?}^{?}$) ; ⑤ calculer en simplifiant. Mini-test : refaire avec $n = 3$ à la main (lister !) pour valider la formule.

**Fiche réflexes :** *ordre ? répétition ? · simultané = $C$ · avec remise = $n^p$ · au moins = total $-$ aucun · simplifier $n!$ · ligne Pascal pour Newton.*
