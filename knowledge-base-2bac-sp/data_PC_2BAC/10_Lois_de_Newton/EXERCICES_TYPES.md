---
chapitre: "10 - Lois de Newton"
unite: "Physique S2 - Mécanique"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituée (style national PC) + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 type-bac + 2e méthode + pièges (backfill verbatim PC prévu)"
---

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types + corrigés — Chapitre 10 (Newton)

> **R1-R4 = type-bac reconstituées** (plan incliné, chute libre, frottement, poulie). $g = 9,8\,m/s^2$.
> Unités SI partout. Banque verbatim prévue dès transcription.

## R1 — TYPE-BAC (plan incliné sans frottement)

🏷️ matière=PC · année=— · session=— · chapitre=P10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Bloc lâché sans vitesse sur une pente $\alpha = 30°$ (sans frottement). (a) $a$ ? (b) $v$ après $d = 2,0\,m$ ?

**Corrigé :**
1. Système {bloc}, référentiel terrestre supposé galiléen. Bilan : $\vec{P} = m\vec{g}$, $\vec{N}$ (⊥ pente).
2. PFD projeté sur $x$ (le long de la pente, vers le bas) : $mg\sin\alpha = ma$ → $\boxed{a = g\sin\alpha = 4,9\,m/s^2}$.
3. $v^2 = v_0^2+2ad = 0+2\times4,9\times2,0 = 19,6$ → $\boxed{v \approx 4,4\,m/s}$.
> بالدارجة: الوصفة: جملة + مرجع + جرد (رسم!) + مبدأ + **إسقاط**! $P_x = mg\sin\alpha$ (تحقق: $\alpha = 0$ ← صفر ✔)! ومن بعد $v^2 = 2ad$ (بلا زمن — مباشرة!). اللي نسى الإسقاط ما عندو والو!

## R2 — TYPE-BAC (chute libre, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Objet lâché ($v_0 = 0$) d'une hauteur $h = 20\,m$ (air négligé). Vitesse à l'arrivée ? Durée ?

**Corrigé — Méthode 1 : PFD + primitivation.**
1. PFD : $m\vec{g} = m\vec{a}$ → $a = g$ (les $m$ se simplifient !).
2. $v = gt$, $y = \frac{1}{2}gt^2$ → $t = \sqrt{2h/g} = \sqrt{40/9,8} = \boxed{2,0\,s}$ ; $v = gt = \boxed{20\,m/s}$ (19,8).

**Corrigé — Méthode 2 : énergie (bonus, chapitre à venir !).**
1. $E_m$ conservée (poids seul) : $\frac{1}{2}mv^2 = mgh$ → $v = \sqrt{2gh} = \sqrt{392} = \boxed{20\,m/s}$. ✅
2. Durée via M1 ($t = v/g$) — l'énergie donne $v$ mais PAS $t$ directement !
> بالدارجة: جوج طرق! **المبدأ** (كامل: $a \to v \to y$ — كيعطي كلشي بما فيها الزمن) و**الطاقة** ($\frac{1}{2}mv^2 = mgh$ — أسرع للسرعة ولكن بلا زمن!). الطاقة من فصل جاي (bonus!) — ولكن شوف كيفاش الفيزياء وحدة: بجوج عطاو $20\,m/s$!

## R3 — TYPE-BAC (frottement : la force qu'on oublie)

🏷️ matière=PC · année=— · session=— · chapitre=P10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Bloc $m = 2,0\,kg$ tiré par $F = 15\,N$ horizontale, frottement $\mu = 0,30$ (glissement). $a$ ?

**Corrigé :**
1. Bilan : $\vec{P}$ ($mg = 19,6\,N$), $\vec{N}$ ($= mg$ : pas d'accélération verticale), $\vec{F}$, $\vec{f}$ ($= \mu N$, opposé au mouvement).
2. PFD sur $x$ : $F-f = ma$ → $a = (15-0,30\times19,6)/2,0 = (15-5,88)/2,0 = \boxed{4,6\,m/s^2}$.
> بالدارجة: الجرد الكامل: الثقل + العمودية + القوة + **الاحتكاك** ($f = \mu N$ ضد الحركة)! اللي نسى الاحتكاك حسب $a = 7,5$ (غلط!). والعمودية $N = mg$ (بلا تسارع عمودي)! الترتيب: $N$ أولاً ← $f$ ← المبدأ!

## R4 — TYPE-BAC (poulie : deux corps, une accélération)

🏷️ matière=PC · année=— · session=— · chapitre=P10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** $m_1 = 1,0\,kg$ sur table (sans frottement) reliée par un fil (poulie idéale) à $m_2 = 2,0\,kg$ suspendue.
$a$ du système ? Tension $T$ ?

**Corrigé :**
1. Fil inextensible → MÊME $a$ (et même $T$ des deux côtés, poulie idéale).
2. PFD sur $m_2$ (vertical) : $m_2g-T = m_2a$ ; sur $m_1$ (horizontal) : $T = m_1a$.
3. Addition : $m_2g = (m_1+m_2)a$ → $\boxed{a = \frac{2,0}{3,0}\times9,8 = 6,5\,m/s^2}$ ; $\boxed{T = m_1a = 6,5\,N}$.
4. Vérifier : $m_2g-T = 19,6-6,5 = 13,1 = m_2a$ ✔.
> بالدارجة: البكرة: **نفس $a$ ونفس $T$** (الخيط ما كيتمططش والبكرة مثالية)! مبدأ لكل جسم ($m_2g-T = m_2a$ و$T = m_1a$) ← جمع المعادلتين ($T$ كتمشي!) ← $a = \frac{m_2}{m_1+m_2}g$! وتحقق بالتعويض!

## 🪤 Pièges testés par question
- **R1** : $P_x = mg\cos\alpha$ ❌ (tester $\alpha = 0$ !) ; $\vec{N}$ projetée sur $x$ ($= 0$ : ⊥ !) ❌ ; $v$ sans $v_0 = 0$ ❌.
- **R2** : $a$ dépend de $m$ ❌ (les $m$ se simplifient !) ; M2 utilisée pour $t$ ❌ (l'énergie ne donne pas le temps !) ; $y_0$/$v_0$ oubliés ❌.
- **R3** : $\vec{f}$ oubliée ❌ ; $f = \mu F$ (c'est $\mu N$ !) ❌ ; sens de $\vec{f}$ avec le mouvement ❌.
- **R4** : deux $a$ différents ❌ (fil inextensible !) ; $T = m_2g$ ($T < m_2g$ car $m_2$ accélère vers le bas !) ❌ ; $m_1$ avec $m_1g$ sur l'horizontale ❌.

---
*Banque d'entraînement étiquetée type-bac. Backfill : questions Newton verbatim du national PC dès transcription (sessions 2023-2025 prioritaires).*
