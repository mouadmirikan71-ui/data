---
chapitre: "01 - Limites et continuité"
unite: "S1 - Analyse de base"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituée (style national PC/SVT) + corrigés prof"
date_collecte: "2026-09-14"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 5 type-bac + 1 vraie 2020R + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 01 (Limites & continuité)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **R1-R5 = type-bac reconstituées** + **Q6 = VRAIE** (2020 Rattrapage, Problème — limites + branches infinies).
> Chaque corrigé = méthode complète + 🪤.

## R1 — FI rationnelle en $+\infty$

🏷️ matière=Math · année=— · session=— · chapitre=M1 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Calculer $\lim_{x\to+\infty}\frac{2x^2-3x+1}{x^2+5}$.

**Corrigé :**
1. Substitution : $\frac{\infty}{\infty}$ → **FI** → factoriser par le terme dominant ($x^2$) :
$$\frac{x^2(2-\frac{3}{x}+\frac{1}{x^2})}{x^2(1+\frac{5}{x^2})} = \frac{2-\frac{3}{x}+\frac{1}{x^2}}{1+\frac{5}{x^2}}$$
2. Passer à la limite : numérateur $\to 2$, dénominateur $\to 1$.
3. $\boxed{2}$ (rapport des coefficients dominants).
> بالدارجة: فـ $\pm\infty$ الكلمة القوية هي اللي فيها **أكبر أس** — عمّل بيها وشطب! النتيجة = قسمة المعاملين (2/1). هادي أسرع نهاية فالوطني!

## R2 — FI avec racine en 0 (2 méthodes !)
**Énoncé :** Calculer $\lim_{x\to 0}\frac{\sqrt{x+1}-1}{x}$.

**Corrigé — Méthode 1 : quantité conjuguée.**
1. FI $\frac{0}{0}$ avec différence de racines → multiplier par le conjugué :
$$\frac{(\sqrt{x+1}-1)(\sqrt{x+1}+1)}{x(\sqrt{x+1}+1)} = \frac{(x+1)-1}{x(\sqrt{x+1}+1)} = \frac{x}{x(\sqrt{x+1}+1)} = \frac{1}{\sqrt{x+1}+1}$$
2. $\boxed{\frac{1}{2}}$.

**Corrigé — Méthode 2 : taux d'accroissement (plus rapide !).**
1. Reconnaître : $\frac{\sqrt{1+x}-\sqrt{1}}{x} = \frac{f(1+x)-f(1)}{x}$ avec $f(t) = \sqrt{t}$ → c'est le taux de $f$ en $1$.
2. Donc limite $= f'(1) = \frac{1}{2\sqrt{1}} = \boxed{\frac{1}{2}}$. ✅ Même résultat.
> بالدارجة: جوج طرق! **المرافق** (كتشطب الجذر) ولا **معدل التغير** (كتعرف $f'$ فنقطة). ملي تشوف $\frac{\sqrt{a+x}-\sqrt{a}}{x}$ — راه معدل تغير الجذر! الطريقة الثانية أسرع إلا عقلتي عليها!

## R3 — Croissances comparées

🏷️ matière=Math · année=— · session=— · chapitre=M1 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Calculer $\lim_{x\to+\infty}(e^x - x^2)$.

**Corrigé :**
1. FI $+\infty - \infty$ → factoriser par le plus fort ($e^x$) :
$$e^x\left(1 - \frac{x^2}{e^x}\right)$$
2. Croissance comparée : $\frac{x^2}{e^x} \to 0$ ($e^x$ écrase tout polynôme).
3. $e^x \times (1 - 0) = +\infty$ → $\boxed{+\infty}$.
> بالدارجة: الماتش: $e^x$ ضد $x^2$ — **الأسي كيربح ديماً**! عمّل بالرابح ($e^x$) والباقي كيمشي للصفر. النتيجة: $+\infty$.

## R4 — TVI rédigé (le modèle à recopier)

🏷️ matière=Math · année=— · session=— · chapitre=M1 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Montrer que $f(x) = x^3 - 3x + 1$ s'annule **une unique fois** sur $[0,1]$, i.e. $f(x) = 0$ admet une unique solution $\alpha \in [0,1]$.

**Corrigé (rédaction-type) :**
1. **Continuité** : $f$ est un polynôme donc **continue** sur $[0,1]$. ✔
2. **Monotonie** : $f'(x) = 3x^2 - 3 = 3(x^2-1) < 0$ sur $]0,1[$ → $f$ **strictement décroissante** sur $[0,1]$. ✔
3. **Valeurs** : $f(0) = 1 > 0$ et $f(1) = -1 < 0$ → $0 \in ]f(1), f(0)[$. ✔
4. Conclusion (corollaire du TVI) : $\boxed{\text{il existe un unique } \alpha \in ]0,1[ \text{ tel que } f(\alpha) = 0}$.
> بالدارجة: الوصفة الثلاثية: **اتصال + رتابة + القيمة محصورة** = حل وحيد! بلا وحدة من هاد الثلاثة الجواب ناقص. هاد التحرير (rédaction) حفظو — كيتعاود فكل مسألة تحليل!

## R5 — Limite usuelle trigonométrique

🏷️ matière=Math · année=— · session=— · chapitre=M1 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Calculer $\lim_{x\to 0}\frac{\sin(3x)}{x}$.

**Corrigé :**
1. FI $\frac{0}{0}$ → faire apparaître la forme $\frac{\sin u}{u}$ :
$$\frac{\sin(3x)}{x} = 3\cdot\frac{\sin(3x)}{3x}$$
2. Poser $u = 3x \to 0$ : $\frac{\sin u}{u} \to 1$.
3. $\boxed{3 \times 1 = 3}$.
> بالدارجة: الحيلة: **وازن البسط والمقام** ($3x$ فوق وتحت)! $\sin(شي حاجة)/(نفس الشي حاجة) \to 1$ ملي الشي حاجة $\to 0$. والمعامل 3 اللي زدناه كيبقى: النتيجة 3!

## Question 6 — VRAIE (2020 R, Problème II.1-II.2b)

🏷️ matière=Math · année=2020 · session=R · chapitre=M1 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Données :** $f(x) = (1-x)e^{1-x}-x^2+5x-3-2\ln x$ sur $]0,+\infty[$.
**Énoncés officiels :** (a) « Montrer que $\lim_{x\to0^+}f(x) = +\infty$ puis interpréter géométriquement » ;
(b) « Montrer que $\lim_{x\to+\infty}f(x) = -\infty$ » ;
(c) « Montrer que $\lim_{x\to+\infty}f(x)/x = -\infty$ puis interpréter géométriquement ».
**Corrigé-type :**
(a) $(1-x)e^{1-x}\to e$ ; $-x^2+5x-3\to-3$ ; $-2\ln x\to+\infty$ → $\boxed{+\infty}$ → asymptote verticale $x = 0$.
(b) $(1-x)e^{1-x}\to 0$ (CC : $Xe^X\to 0$) ; $-x^2$ écrase $5x-3-2\ln x$ → $\boxed{-\infty}$.
(c) $f(x)/x = \frac{(1-x)e^{1-x}}{x}-x+5-\frac{3}{x}-2\frac{\ln x}{x}\to-\infty$ → $\boxed{-\infty}$ →
branche parabolique de direction $(Oy)$.
> بالدارجة: الوطني الحقيقي! (a) فـ $0^+$: اللوغاريتم هو اللي كيحكم ($-2\ln x \to +\infty$)! (b) فـ $+\infty$: $-x^2$ كتسحق كلشي (الأسي واللوغاريتم كيموتو)! (c) $f/x \to -\infty$ = **فرع قطع مكافئ باتجاه $Oy$** — التفسير الهندسي إجباري!
> Source : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ — ✅ filière confirmée SP : l'en-tête officiel du corrigé (RR 22F) indique « شعبة العلوم التجريبية » (Sciences Expérimentales, مسلكا SVT + Sciences Physiques) : papier commun PC+SVT (le label « ST » d'AlloSchool/du fichier est une erreur d'étiquetage).

## 🪤 Pièges testés par question
- **R1** : simplifier par $x^2$ sans factoriser proprement (oublier des termes) ; conclure « $\infty/\infty = 1$ » ❌.
- **R2** : développer $(\sqrt{a}-1)(\sqrt{a}+1)$ comme $a - 1$… faux si mal appliqué : $(A-B)(A+B) = A^2-B^2$ avec $A = \sqrt{x+1}$ → $(x+1) - 1$ ✔ ; oublier de simplifier par $x$ avant la limite ❌.
- **R3** : écrire $e^x - x^2 \to \infty - \infty = 0$ ❌ (le match a un gagnant : $e^x$ !).
- **R4** : TVI sans continuité ni monotonie (conclusion parachutée = 0) ; monotonie affirmée sans $f'$ ❌ ; confondre TVI (existence) et corollaire (unicité).
- **R5** : $\sin(3x)/x \to 1$ (oublier le facteur 3 !) ❌ ; appliquer la limite usuelle avec $u \not\to 0$ ❌.
- **Q6** : $-2\ln x\to-\infty$ en $0^+$ (signe : $-\ln\to+\infty$ !) ❌ ; $(1-x)e^{1-x}$ en $+\infty$ traitée $\infty\times0 = 0$ sans CC ❌ ; interprétations géométriques oubliées (exigées par l'énoncé !) ❌.

---
*R1-R5 = type-bac ; Q6 = vraie nationale (2020 R, Problème). Backfill complémentaire : TVI verbatim + sessions récentes (2023-2025).* 
