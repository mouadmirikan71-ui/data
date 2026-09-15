---
chapitre: "12 - Mouvements de projectiles"
unite: "Physique S2 - Mécanique"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituée (style national PC) + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 type-bac + 2e méthode + pièges (backfill verbatim PC prévu)"
---

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types + corrigés — Chapitre 12 (Mouvements de projectiles)

> **R1-R4 = type-bac reconstituées** (projectile, trajectoire, électron dans E, proton dans B). $g = 9,8\,m/s^2$.
> Unités SI partout. Banque verbatim prévue dès transcription.

## R1 — TYPE-BAC (projectile complet, 2 méthodes sur la portée !)

🏷️ matière=PC · année=— · session=— · chapitre=P12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Ballon frappé avec $v_0 = 20\,m/s$, $\alpha = 45°$ (origine au point de frappe). (a) Horaires + trajectoire.
(b) Portée (2 méthodes !). (c) Flèche + durée.

**Corrigé :**
(a) $v_{0x} = 20\cos45 = 14,1\,m/s$, $v_{0y} = 14,1\,m/s$. PFD : $a_x = 0$, $a_y = -g$.
$\boxed{x = 14,1t}$ ; $\boxed{y = -4,9t^2+14,1t}$ ; trajectoire : $\boxed{y = -0,0245x^2+x}$ (parabole ✔).
(b) **Méthode 1 : horaires.** $y = 0$ ($t\ne 0$) → $t = 2\times14,1/9,8 = 2,88\,s$ → $P = 14,1\times2,88 = \boxed{40,6\,m}$.
**Méthode 2 : formule.** $P = v_0^2\sin 2\alpha/g = 400\times1/9,8 = \boxed{40,8\,m}$. ✅ (Écart = arrondis.)
(c) $v_y = 0$ → $t = 14,1/9,8 = 1,44\,s$ → $\boxed{F = -4,9(1,44)^2+14,1(1,44) = 10,2\,m}$ ; durée $\boxed{2,9\,s}$.
> بالدارجة: القالب الكامل! (a) الشروط البدئية ($v_0\cos\alpha$, $v_0\sin\alpha$) ← المبدأ مسقط ← المعادلات! (b) المدى بطريقتين: **المعادلات** ($y = 0$ ← $t$ ← $x$) و**الصيغة** ($v_0^2\sin 2\alpha/g$) — التطابق = التحقق! (c) الذروة: $v_y = 0$! و$45°$ = المدى الأعظمي!

## R2 — TYPE-BAC (lire un mouvement depuis ses horaires)

🏷️ matière=PC · année=— · session=— · chapitre=P12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** $\overrightarrow{OM}(t) : x = 2,0t$, $y = 30-5,0t^2$ (SI). (a) $\vec{v}(t)$, $\vec{a}(t)$.
(b) $|\vec{v}|$ à $t = 1,0\,s$. (c) Nature du mouvement ?

**Corrigé :**
(a) $\boxed{\vec{v} = (2,0\,;\,-10t)}$ ; $\boxed{\vec{a} = (0\,;\,-10)}$ (m/s² — Portrait : $a_y\approx -g$ !).
(b) $|\vec{v}(1)| = \sqrt{4+100} = \boxed{10,2\,m/s}$.
(c) $a_x = 0$, $a_y = \text{Cte}$ → $\boxed{\text{projectile horizontal}}$ ($v_{0x} = 2,0\,m/s$, lancé depuis $y_0 = 30\,m$) ;
trajectoire : $t = x/2$ → $y = 30-1,25x^2$ (parabole ✔).
> بالدارجة: الحركة بالمقلوب: من المعادلات استنتج الطبيعة! اشتق ($v$ ← $a$): $a = (0,-10)$ ← **قذيفة أفقية** ($a_y \approx -g$)! والمسار: احذف $t$ ($t = x/2$) ← قطع مكافئ! هاد التمرين «المحقق» كيعلمك تقرا المعادلات!

## R3 — TYPE-BAC (électron dans $\vec{E}$ : la déflexion)

🏷️ matière=PC · année=— · session=— · chapitre=P12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Électron ($e = 1,6\times10^{-19}\,C$, $m = 9,1\times10^{-31}\,kg$) entre en $\vec{v}_0 = 2,0\times10^7\,m/s$
(⊥ à $\vec{E} = 1,0\times10^3\,V/m$) dans des plaques de longueur $L = 5,0\,cm$. Déviation $Y$ à la sortie ?
(Justifier poids négligé.)

**Corrigé :**
1. $mg\approx 10^{-29}\,N \ll eE = 1,6\times10^{-16}\,N$ → $\boxed{\text{poids négligé}}$ (rapport $10^{13}$ !).
2. $a_y = -eE/m$ (électron : opposé à $\vec{E}$ !) : $t_{sortie} = L/v_0 = 2,5\times10^{-9}\,s$.
3. $Y = \frac{1}{2}\frac{eE}{m}t^2 = \frac{1}{2}\times\frac{1,6\times10^{-16}}{9,1\times10^{-31}}\times(2,5\times10^{-9})^2$
$= \frac{1}{2}\times1,76\times10^{14}\times6,25\times10^{-18} = \boxed{5,5\times10^{-4}\,m}$ ($\approx 0,55\,mm$, côté $-\vec{E}$).
> بالدارجة: نفس رياضيات القذيفة ($g \to eE/m$)! (1) **برر الإهمال بالأرقام** ($10^{13}$ مرة أصغر!)! (2) الإلكترون كينحرف **عكس** $\vec{E}$ (شحنة سالبة)! (3) $Y = \frac{1}{2}at^2$ مع $t = L/v_0$! القوى العشرية ($10^{-31}$!) — انتبه للأسس!

## R4 — TYPE-BAC (proton dans $\vec{B}$ : le cercle)

🏷️ matière=PC · année=— · session=— · chapitre=P12 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Proton ($m = 1,67\times10^{-27}\,kg$, $q = e$) à $v = 1,0\times10^6\,m/s$ (⊥ $\vec{B} = 0,50\,T$).
(a) Nature + $R$ ? (b) $T$ ? Commenter.

**Corrigé :**
(a) $\vec{F}\perp\vec{v}$ → $|\vec{v}|$ Cte → $\boxed{\text{circulaire uniforme}}$.
$qvB = mv^2/R$ → $R = mv/qB = \frac{1,67\times10^{-27}\times10^6}{1,6\times10^{-19}\times0,50} = \boxed{2,1\times10^{-2}\,m}$ ($\approx 2,1\,cm$).
(b) $T = 2\pi R/v = 2\pi m/qB = \boxed{1,3\times10^{-7}\,s}$ — $\boxed{\text{indépendante de } v}$ (secret du cyclotron !).
> بالدارجة: $\vec{B}$: القوة عمودية ← السرعة ثابتة ← **دائري منتظم**! $R = mv/qB$ مباشرة (منعكس الدائري)! والدور $T = 2\pi m/qB$ **مستقل على السرعة** — الأسرع دائرة أكبر بنفس الدور! هادا هو مبدأ السيكلوترون!

## VRAIE — 2025R Ex4-Partie I (skieur : projectile + réception, 2 pts)

🏷️ matière=PC · année=2025 · session=R · chapitre=P12 · type=VRAIE · fidélité=reconstitué-corrigé · niveau=★★★ · barème=Q1 0,5 · Q2 0,5 · Q3 1,0

> ⚠️ Énoncé **reconstitué** depuis les éléments de réponse officiels (correction provinciale Mohammedia, scribd 889488300, Tier B). Angle $\alpha$ de la piste de réception (figure du sujet) non relu ; résultat $OE$ officiel conservé.
> Données (reconstituées) : skieur quittant un tremplin à $v_0 = 30$ m/s horizontalement ($O$ origine, $Ox$ horizontal, $Oy$ vertical ascendant) ; $g = 10$ m/s² ; vol libre puis réception en $E$ sur une piste inclinée de $\alpha$.

**Q1.** Établir les équations horaires $x(t)$, $y(t)$. (0,25+0,25)
**Q2.** En déduire l'équation de la trajectoire. (0,5)
**Q3.** Déterminer la distance de réception $OE$. (0,75+0,25)

**Corrigé-type :**
1. Système : skieur, seule force $\vec{P}$ → $\vec{a} = \vec{g}$ : $a_x = 0$, $a_y = -g$. CI : $x(0) = y(0) = 0$, $v_x(0) = 30$, $v_y(0) = 0$ → $\boxed{x(t) = 30t}$ ; $\boxed{y(t) = -5t^2}$.
2. $t = x/30$ dans (2) : $y = -5(x/30)^2 = \boxed{y = -5,56\times 10^{-3}\,x^2}$ (parabole !).
3. $E$ sur la piste : $x_E = OE\cos\alpha$, $y_E = -OE\sin\alpha$ ; $E$ sur la trajectoire : $-OE\sin\alpha = -5,56\times 10^{-3}(OE\cos\alpha)^2$ → $OE = \frac{\sin\alpha}{5,56\times 10^{-3}\cos^2\alpha} = \boxed{47,44\text{ m}}$ (AN officielle).
🪤 *Pièges testés : $v_y(0) = 0$ (départ HORIZONTAL — pas de $v_0\sin\alpha$ !) ; trajectoire : éliminer $t$ (pas de $t$ dans la réponse !) ; $E$ vérifie DEUX équations (piste + parabole) — une seule = bloqué.*
🗣️ الخلاصة : المتزحلق مقذوف ($v_0 = 30$ أفقي!): $x = 30t$ و$y = -5t^2$! المسار: حيّد $t$ ← قطع مكافئ ($y = -5,56\times 10^{-3}x^2$)! والوصول $E$: كيحقق **جوج** معادلات (المنحدر + المسار) ← $OE = 47,44$ m! الفخ: $v_y(0) = 0$ (الانطلاق أفقي!) ماشي $v_0\sin$!

## 🪤 Pièges testés par question
- **R1** : $v_{0x} = v_0\sin\alpha$ ❌ ; $y = 0$ donnant $t = 0$ gardé (c'est le DÉPART !) ❌ ; $P$ en $s$ (unités !) ❌.
- **R2** : dérivation de $30-5t^2$ en $-5t$ ($-10t$ !) ❌ ; $|\vec{v}| = v_x+v_y$ ❌ (Pythagore !) ; « MRU » ($a_y\ne 0$ !) ❌.
- **R3** : poids non négligé sans justification ❌ ; déviation côté $+\vec{E}$ (électron : $-\vec{E}$ !) ❌ ; puissances de 10 ($10^{-31}$ !) ❌.
- **R4** : $R = mv^2/qB$ ❌ ; $T$ « proportionnelle à $v$ » ❌ (indépendante !) ; trajectoire parabolique ($B$ = cercle !) ❌.

---
*R1-R4 = entraînement. VRAIE 2025R Ex4-Partie I (skieur, reconstituée-corrigé, Part 19). Upgrade verbatim dès transcription du sujet intégral.*
