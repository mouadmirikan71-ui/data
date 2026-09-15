---
chapitre: "07 - Dipole RL"
unite: "Physique S1 - Électricité"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituée (style national PC) + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 type-bac + 2e méthode + pièges (backfill verbatim PC prévu)"
---

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types + corrigés — Chapitre 07 (Dipôle RL)

> **R1-R4 = type-bac reconstituées** (établissement, $\tau$, énergie+surtension, bobine réelle).
> Unités SI partout. Banque verbatim prévue dès transcription.

## R1 — TYPE-BAC (établissement complet)

🏷️ matière=PC · année=— · session=— · chapitre=P07 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Bobine idéale $L = 0,50\,H$ en série avec $R = 100\,\Omega$ et $E = 12\,V$ ($i(0) = 0$).
(a) EDP. (b) $I_0$, $\tau$, $i(t)$. (c) $u_L(t)$ et $u_L(0)$.

**Corrigé :**
(a) Mailles orientées : $E = Ri + L\frac{di}{dt}$ → $\boxed{L\frac{di}{dt}+Ri = E}$.
(b) $I_0 = E/R = \boxed{0,12\,A}$ ; $\tau = L/R = 0,50/100 = \boxed{5,0\times10^{-3}\,s}$ ;
$\boxed{i(t) = 0,12\left(1-e^{-t/0,005}\right)}$.
(c) $u_L = L\frac{di}{dt} = Ee^{-t/\tau} = \boxed{12e^{-t/0,005}\,V}$ → $\boxed{u_L(0) = 12\,V = E}$ (part du plafond !).
> بالدارجة: نفس وصفة RC: عقد ← شكل قياسي ← حل! $I_0 = E/R$ و$\tau = L/R$. والمفاجأة: $u_L(0) = E$ — **الوشيعة كتاخذ التوتر كامل فالبداية**! اللي رسمها طالعة من 0 غلط!

## R2 — TYPE-BAC ($\tau$ par 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P07 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Établissement vers $I_0 = 0,20\,A$ ($L = 0,80\,H$, $R = 100\,\Omega$). La courbe $i(t)$ est relevée.
Déterminer $\tau$ par deux méthodes indépendantes.

**Corrigé — Méthode 1 : calcul.** $\tau = L/R = 0,80/100 = \boxed{8,0\times10^{-3}\,s}$.
**Corrigé — Méthode 2 : 63 % graphique.** $0,63I_0 = 0,126\,A$ → abscisse sur la courbe : $t \approx \boxed{8,0\,ms}$. ✅
(Variante : tangente à l'origine → coupe $i = I_0$ à $t = \tau$.) Concordance = vérification.
> بالدارجة: **الحساب** ($L/R$) و**المنحنى** (63 % ولا المماس) — التطابق = التحقق! نفس التقنية ديال RC بالضبط: إلا ضبطتيها تماك، هنايا مجانية!

## R3 — TYPE-BAC (énergie + surtension à la rupture)

🏷️ matière=PC · année=— · session=— · chapitre=P07 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** $L = 0,20\,H$ parcourue par $I_0 = 1,5\,A$ (établis sous $E = 12\,V$). On ouvre sur $R' = 50\,\Omega$
(diode de roue libre). (a) Énergie stockée. (b) $i(t)$ à la rupture. (c) Pic de tension — commenter.

**Corrigé :**
(a) $E_m = \frac{1}{2}LI_0^2 = \frac{1}{2}\times0,20\times2,25 = \boxed{0,225\,J}$.
(b) $\tau' = L/R' = 0,20/50 = \boxed{4,0\,ms}$ ; $\boxed{i(t) = 1,5e^{-t/0,004}}$ ($i$ continu : part de $1,5\,A$ ✔).
(c) $u_L(0^+) = -R'I_0 = -50\times1,5 = \boxed{-75\,V}$ : **6× le générateur !** Sans diode, ce pic claque l'air
(étincelle) ou détruit les composants — d'où la protection.
> بالدارجة: الطاقة $\frac{1}{2}Li^2 = 0,225\,J$ **خاصها تمشي لشي بلاصة**! التيار متصل (كيبدا من 1,5A) ولكن التوتر كينقز لـ $-75V$ — **ستة أضعاف المولد**! هادي هي الشرارة: الطاقة اللي ما لقاتش الطريق!

## R4 — TYPE-BAC (bobine réelle + régime permanent)

🏷️ matière=PC · année=— · session=— · chapitre=P07 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Bobine ($L = 0,40\,H$, $r = 10\,\Omega$) en série avec $R = 90\,\Omega$ et $E = 6,0\,V$.
(a) $R_{tot}$, $I_0$, $\tau$. (b) Tension de la bobine en régime permanent. (c) Énergie stockée.

**Corrigé :**
(a) $R_{tot} = R+r = \boxed{100\,\Omega}$ ; $I_0 = E/R_{tot} = \boxed{6,0\times10^{-2}\,A}$ ;
$\tau = L/R_{tot} = 0,40/100 = \boxed{4,0\,ms}$.
(b) Permanent : $\frac{di}{dt} = 0$ → $u_b = rI_0 = 10\times0,060 = \boxed{0,60\,V}$ (pas 0 : bobine RÉELLE !).
(c) $E_m = \frac{1}{2}\times0,40\times(0,060)^2 = \boxed{7,2\times10^{-4}\,J}$.
> بالدارجة: الحقيقية = زيد $r$ فكلشي ($R_{tot}$)! وفالدائم الوشيعة الحقيقية كيبقى فيها $rI_0 = 0,6V$ — **ماشي صفر**! (الصفر غير للمثالية.) هاد الفرق $r$ هو اللي كيصيد!

## VRAIE — 2025R Ex3-Partie I (RL : établissement + rupture, ≈3,5 pts)

🏷️ matière=PC · année=2025 · session=R · chapitre=P07 · type=VRAIE · fidélité=reconstitué-corrigé · niveau=★★★ · barème=voir questions

> ⚠️ Énoncé **reconstitué** depuis les éléments de réponse officiels (correction provinciale Mohammedia, scribd 889488300, Tier B : questions, valeurs, barème). Formulation exacte non relue.
> Données (reconstituées) : $E = 10$ V, $R = 100\ \Omega$, bobine idéale d'inductance $L$ ; courbe $u_R(t)$ fournie ; à la rupture on branche $R_1 = 1000\ \Omega$ aux bornes de la bobine.

**1-1.** Établir l'équation différentielle vérifiée par $u_R$ à l'établissement. (0,5)
**1-2.** Déterminer graphiquement $\tau$ et $u_R(\infty)$ ; en déduire $I_0$. (0,25+0,5)
**1-3.** Vérifier que $L = 0,10$ H. (0,5)
**1-4.** $u_b$ et l'énergie emmagasinée en régime permanent. (0,25+0,5)
**2-1/2/3.** À la rupture ($t = 0$) : $i(0^+)$, $u_{R1}(0^+)$, $u_b(0^+)$. (3×0,25)

**Corrigé-type :**
1. $u_R + u_b = E$, $i = u_R/R$, $u_b = L\frac{di}{dt}$ → $\boxed{\frac{du_R}{dt} + \frac{R}{L}u_R = \frac{R}{L}E}$.
2. $\boxed{\tau = 1,0\text{ ms}}$, $\boxed{u_R(\infty) = 10\text{ V}}$ → $I_0 = u_R(\infty)/R = \boxed{0,10\text{ A}}$.
3. $L = \tau R = 10^{-3}\times 100 = \boxed{0,10\text{ H}}$.
4. $\boxed{u_b(\infty) = 0}$ ($I_0$ constant !) ; $E_m = \frac{1}{2}LI_0^2 = \frac{1}{2}\times 0,1\times 0,01 = \boxed{5,0\times 10^{-4}\text{ J}}$.
5. Continuité : $\boxed{i(0^+) = I_0 = 0,10\text{ A}}$ → $u_{R1}(0^+) = R_1I_0 = \boxed{100\text{ V}}$ → maille : $\boxed{u_b(0^+) = -100\text{ V}}$ (surtension ×10 !).
> Bonus lu (pont P08) : avec $C = 1\ \mu$F, $N_0 = 1/(2\pi\sqrt{LC}) = \boxed{503\text{ Hz}}$.
🪤 *Pièges testés : $\tau$ lu à 63 % de 10 V (pas « fin de la montée » !) ; $u_b(\infty) = E$ (c'est 0 : bobine = fil !) ; rupture : $i$ ne saute PAS mais $u_b$ explose ($-100$ V !).*
🗣️ الخلاصة : المعادلة: $u_R + \frac{L}{R}\dot{u_R} = E$! $\tau = 1$ ms من المنحنى ← $L = \tau R = 0,1$ H! الدائم: الوشيعة = سلك ($u_b = 0$, $E_m = 5\times 10^{-4}$ J)! والقطع: التيار ما كيقفزش ($0,1$ A) ولكن التوتر كينفاجر (**$-100$ V** — عشرة المرات $E$)! هادي هي الـ surtension!

## 🪤 Pièges testés par question
- **R1** : $u_L(0) = 0$ ❌ (vaut $E$ !) ; $\tau = L\times R$ ❌ ; $i(t)$ de rupture pour un établissement ❌.
- **R2** : 63 % de $E$ au lieu de $I_0$ ❌ ; tangente pas à l'origine ❌ ; $ms$ lus comme $s$ ❌.
- **R3** : $i$ qui « saute à 0 » à l'ouverture ❌ (continu !) ; pic $= +R'I_0$ (signe : $-R'I_0$ !) ❌ ; surtension non comparée à $E$ ❌.
- **R4** : $r$ oubliée dans $R_{tot}$ ❌ ; $u_b = 0$ en permanent (bobine réelle !) ❌ ; $E_m$ avec $I$ en $mA$ non converti ❌.

---
*R1-R4 = entraînement. VRAIE 2025R Ex3-Partie I (RL, reconstituée-corrigé, Part 19). Upgrade verbatim dès transcription du sujet intégral.*
