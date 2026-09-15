---
chapitre: "08 - Nombres complexes (partie 2 : trigonométrie, Moivre, transformations)"
unite: "S2 - Algèbre"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Ex.2 Q2-Q5 (réels, SP confirmé) + 1 type-bac + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 vraies nationales + 1 type-bac + 2e méthode + pièges"
---

# Exercices types + corrigés — Chapitre 08 (Complexes P2)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

> **Q1-Q4 = VRAIES questions** nationales : **2020 Rattrapage Ex.2 Q2-Q5** (trigo/Moivre, rotation, triangle,
> alignement — filière SP confirmée, RR 22F). **R1 = type-bac** (racines cubiques).
> Sources : https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ (sujet SP + corrigé, session 2020R) + https://www.alloschool.com/element/109814 (barème, même papier 2020R).

## Données 2020R (Ex.2)
$a = \frac{\sqrt{2}}{2}+i\frac{\sqrt{2}}{2}$, $b = \cos\frac{\pi}{8}+i\sin\frac{\pi}{8}$ ($|a| = |b| = 1$).
Points : $A(a)$, $B(b)$, $C(c)$ avec $c = 1$. $R$ = rotation de centre $O$, angle $\frac{\pi}{8}$.

## Question 1 — VRAIE (2020 R, Ex.2 Q2a+Q2b, 1.25 pt, 2 méthodes sur Q2a !)

🏷️ matière=Math · année=2020 · session=R · chapitre=M8 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncés officiels :** « Écrire $a$ sous forme trigonométrique et en déduire que $a^{2020}$ est un nombre réel »
(0.75) ; « Soit $b = \cos\frac{\pi}{8}+i\sin\frac{\pi}{8}$. Prouver que $b^2 = a$ » (0.5).

**Corrigé Q2a — Méthode 1 : Moivre direct.**
$|a| = \sqrt{\frac{1}{2}+\frac{1}{2}} = 1$, $\cos\theta = \sin\theta = \frac{\sqrt{2}}{2}$ → $\boxed{a = e^{i\pi/4}}$.
$a^{2020} = e^{i2020\pi/4} = e^{i505\pi} = \cos 505\pi = \boxed{-1\in\mathbb{R}}$ ✔ ($505 = 2\times252+1$ : impair !).
**Corrigé Q2a — Méthode 2 : via $a^4 = -1$.**
$a^2 = e^{i\pi/2} = i$, $a^4 = i^2 = -1$ → $a^{2020} = (a^4)^{505} = (-1)^{505} = \boxed{-1}$. ✅ (Plus malin : pas
besoin de $505\pi$ !)
**Corrigé Q2b :** $b^2 = (e^{i\pi/8})^2 = e^{i2\pi/8} = e^{i\pi/4} = \boxed{a}$ ✔ (Moivre : angle doublé !).
> بالدارجة: جوج طرق لـ $a^{2020}$! **موافر المباشر** ($e^{i505\pi} = -1$ — 505 فردي!) و**الذكي** ($a^2 = i$، $a^4 = -1$ ← $(-1)^{505} = -1$)! الثانية أسرع وأجمل — القوى الكبيرة كتفكك! و$b^2 = a$ حيت **الزاوية تضاعفات** ($\pi/8 \to \pi/4$)!

## Question 2 — VRAIE (2020 R, Ex.2 Q3a+Q3b, 0.75 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M8 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncés officiels :** « Vérifier que $z' = bz$ » (0.25) ; « Déterminer l'image de $C$ par $R$ et montrer que $A$
est l'image de $B$ par $R$ » (0.5).

**Corrigé-type :**
(a) $R$ : $z'-0 = e^{i\pi/8}(z-0)$, et $b = e^{i\pi/8}$ → $\boxed{z' = bz}$ ✔.
(b) $C' = b\cdot c = b\times 1 = b$ → $\boxed{C' = B}$ ; $B' = b\cdot b = b^2 = a$ (Q1 !) → $\boxed{B' = A}$ ✔.
> بالدارجة: الدوران حول الأصل = **الضرب** ($z' = bz$)! صورة $C$: $b\times 1 = b$ ← هي $B$! صورة $B$: $b\times b = b^2 = a$ (السؤال اللي قبل!) ← هي $A$! السلسلة $C \to B \to A$ = جوج دورانات $\pi/8$! الأسئلة مربوطة — استعمل اللي فات!

## Question 3 — VRAIE (2020 R, Ex.2 Q4a+Q4b, 1.25 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M8 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncés officiels :** « Montrer que $|a-b| = |b-c|$ et en déduire la nature du triangle $ABC$ » (0.75) ;
« Déterminer une mesure de l'angle $(\overrightarrow{BA},\overrightarrow{BC})$ » (0.5).

**Corrigé-type :**
(a) $|a-b| = |b^2-b| = |b||b-1| = 1\cdot|b-1| = |b-c|$ ✔ ($|b| = 1$, $c = 1$ !) →
$AB = BC$ → $\boxed{ABC\text{ isocèle en } B}$.
(b) $(\overrightarrow{BA},\overrightarrow{BC}) = \arg\frac{c-b}{a-b}$ ; or $\frac{1-b}{a-b} = \frac{1-b}{b^2-b} = \frac{1-b}{b(b-1)} = -\frac{1}{b} = -e^{-i\pi/8} = e^{i7\pi/8}$
→ $\boxed{(\overrightarrow{BA},\overrightarrow{BC}) = \frac{7\pi}{8}}$ (vérifier : inscrit interceptant le grand arc $AC$ :
$\frac{1}{2}(2\pi-\frac{\pi}{4}) = \frac{7\pi}{8}$ ✔ ; sinus : $AC/\sin\frac{7\pi}{8} = 2R = 2$ ✔).
> بالدارجة: (a) **عمّل بـ $b$** ($|b^2-b| = |b||b-1|$) والمعيار 1 كيسهل! متساوي الساقين فـ $B$! (b) الزاوية = عمدة الخارج ($\frac{1-b}{a-b} = -\frac{1}{b} = e^{i7\pi/8}$)! الجواب $7\pi/8$ (ماشي $\pi/8$!) حيت $B$ فوق القوس الصغير — الزاوية كتقابل **القوس الكبير**! تحقق بنظرية الزاوية المحيطية!

## Question 4 — VRAIE (2020 R, Ex.2 Q5a+Q5b, 1 pt)

🏷️ matière=Math · année=2020 · session=R · chapitre=M8 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
**Énoncés officiels :** « $T$ = translation de vecteur $\vec{u}$, $D$ = image de $A$ par $T$. Vérifier que l'affixe
de $D$ est $b^2+1$ » (0.25) ; « Montrer que $\frac{b^2+1}{b} = b+\bar{b}$ et en déduire que $O$, $B$, $D$ sont
alignés » (0.75).

**Corrigé-type :**
(a) $\vec{u}$ a pour affixe $1 = c$ → $d = a+1 = b^2+1$ (Q1 !) → $\boxed{d = b^2+1}$ ✔.
(b) $\frac{b^2+1}{b} = b+\frac{1}{b} = b+\bar{b}$ (car $b\bar{b} = |b|^2 = 1$ !) $= 2\text{Re}(b) = 2\cos\frac{\pi}{8}\in\mathbb{R}$
→ $\frac{d-0}{b-0}\in\mathbb{R}$ → $\boxed{O, B, D\text{ alignés}}$ ✔ (quotient réel = angle plat !).
> بالدارجة: (a) الإزاحة $+1$ ($d = a+1 = b^2+1$ — استعمل Q1!)! (b) $\frac{b^2+1}{b} = b+\frac{1}{b} = b+\bar{b} = 2\cos(\pi/8)$ **حقيقي** ← الاستقامة! ($1/b = \bar{b}$ حيت $|b| = 1$ — حركة ذهبية!) الخارج الحقيقي = التوقيع ديال الاستقامة!

## R1 — TYPE-BAC (racines cubiques : le polygone)

🏷️ matière=Math · année=— · session=— · chapitre=M8 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé
**Énoncé :** Résoudre dans $\mathbb{C}$ : $z^3 = 1$. (Bonus : $1+j+j^2$ ?)

**Corrigé :**
$|z| = 1$, $\arg(z) = \frac{0+2k\pi}{3}$ ($k = 0,1,2$) → $\boxed{z_0 = 1\,,\, z_1 = e^{i2\pi/3} = j\,,\, z_2 = e^{i4\pi/3} = j^2}$
($j = -\frac{1}{2}+i\frac{\sqrt{3}}{2}$, triangle équilatéral !). Bonus : $1+j+j^2 = \frac{1-j^3}{1-j} = 0$ (car $j^3 = 1$, $j\ne 1$) ✔.
> بالدارجة: $z^3 = 1$: المعيار 1، والعمد $0$, $2\pi/3$, $4\pi/3$ — **مثلث متساوي الأضلاع**! ($j = e^{i2\pi/3}$)! و$1+j+j^2 = 0$ (مجموع هندسي!) — صيغة كتعاود بزاف!

## R2 — ENTRAÎNEMENT (linéariser $\cos^3$ + intégrale, pont M09)

🏷️ matière=Math · année=— · session=— · chapitre=M8 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★ · barème=—

**Énoncé :** (a) Linéariser $\cos^3 x$. (b) En déduire $\int_0^\pi \cos^3 x\,dx$.
**Corrigé :** (a) $\cos^3 x = \left(\frac{e^{ix}+e^{-ix}}{2}\right)^3 = \frac{e^{3ix}+3e^{ix}+3e^{-ix}+e^{-3ix}}{8} = \boxed{\frac{\cos 3x+3\cos x}{4}}$. (b) $\int_0^\pi = \frac{1}{4}\left[\frac{\sin 3x}{3}+3\sin x\right]_0^\pi = \boxed{0}$ ($\sin 3\pi = \sin\pi = 0$ !).
> بالدارجة: أويلر + النشر: $(e^{ix}+e^{-ix})^3$ ← $e^{\pm 3ix} + 3e^{\pm ix}$ ← $(\cos 3x+3\cos x)/4$! والتكامل: الأصلية $[\sin 3x/3+3\sin x]/4$ ← فـ $0$ و$\pi$ كلشي صفر ← **النتيجة 0**! بلا التخطيط (linéarisation) التكامل مستحيل!

> ⚠️ Linéarisation : **aucune VRAIE identifiée** (2020R Ex2 = trigo/rotations/alignement, sans linéarisation ; sessions non relues illisibles). R2 = entraînement pur.

## 🪤 Pièges testés par question
- **Q1** : $a^{2020} = e^{i2020\pi}$ (oublier $/4$ !) ❌ ; $505\pi$ « pair » ❌ (505 impair → $-1$ !) ; $b^2$ par distributivité $(a+ib)^2$ (long et risqué !) ❌.
- **Q2** : $z' = e^{i\pi/8}z$ sans identifier $b$ ❌ ; $B' = b^2$ non relié à $a$ (Q1 !) ❌ ; rotation autour de $B$ au lieu de $O$ ❌.
- **Q3** : $|b^2-b| = |b|^2-|b|$ ❌ (factoriser, pas distribuer !) ; angle $= \pi/8$ (le petit arc ! c'est $7\pi/8$ !) ❌ ; quotient d'angle inversé ❌.
- **Q4** : $d = a+b$ (translation de $\vec{u}$, pas de $\overrightarrow{OB}$ !) ❌ ; $1/b = -b$ ❌ ($= \bar{b}$ !) ; $b+\bar{b} = 2b$ ($= 2\text{Re}(b)$ !) ❌.
- **R1** : UNE seule racine ($z = 1$) ❌ ; $k = 0..3$ (4 valeurs dont un doublon !) ❌ ; $j^2 = e^{i2\pi/3}$ ($= e^{i4\pi/3}$ !) ❌.
- **R2** : $(e^{ix}+e^{-ix})^3$ développé comme $e^{3ix}+e^{-3ix}$ (termes croisés $3e^{\pm ix}$ oubliés !) ❌ ; $/8$ perdu ❌ ; $\int\cos^3$ sans linéariser ❌.

---
*Q1-Q4 = exercice national réel (2020 R, Ex.2, SP confirmé). R1 = entraînement étiqueté. Ex.2 Q1 (2nd degré) → ch.06 (P1).*

## VRAIE — 2023N Ex2 (complexes : $a=\sqrt{2}+i\sqrt{2}$, rotation $\pi/4$)

🏷️ matière=Math · année=2023 · session=N · chapitre=M8 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
$a = 2(\cos\pi/4+i\sin\pi/4)$. $b-d = c$ ($c=\bar{b}$) ; $(\sqrt{2}+1)(b-a) = b-d$ → $(b-d)/(b-a) \in \mathbb{R}$ → $A,B,D$ alignés. $ac = 2b$ → $\arg b = \arg a + \arg c = \arg a - \arg b$ → $2\arg b = \pi/4$ $[2\pi]$. Rotation $R(O,\pi/4)$ : $z' = e^{i\pi/4}z = \frac{1}{2}az$ ; $R(C) = B$ ($b=\frac{1}{2}ac$), $R(A) = D$ ($\frac{1}{2}a^2 = 2i = d$). $(b-a)/(c-a) = \frac{\sqrt{2}-1}{2}a$ (facteur $>0$) → $(\overrightarrow{AC},\overrightarrow{AB}) = \arg a = \pi/4$.
🪤 *vraie : alignement via quotient RÉEL (pas de coordonnées !) ; $c = \bar{b}$ → args opposés.*
