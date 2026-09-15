> **Pointer** : `15_Pendule_pesant_et_torsion` → P4 (R1-R4 type-bac + R5 balançoire + R6 torsion-énergie) + 1 VRAIE (2025R Ex4-P2 torsion) → corrigés-types + pièges testés.
> Jumeau rectiligne (ressort) → `14_Pendule_elastique_horizontal`.
> 🏷️ Schéma de tags : `matière · année · session · chapitre · type (VRAIE/ENTRAÎNEMENT) · fidélité (verbatim/reconstitué-corrigé/n.a.) · type_question · niveau · compétence · barème`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Pendule pesant et torsion (P15)

## Méthode — pendule en 5 gestes 🧭

1. Identifier : simple ($l$/$g$), pesant ($J$/$mgd$), torsion ($J$/$C$) ?
2. $T_0 = 2\pi\sqrt{\text{inertie}/\text{rappel}}$ (inertie en HAUT !).
3. Petits angles exigés ($\sin\theta \approx \theta$).
4. $g$ : $g = 4\pi^2l/T_0^2$ ($g$ au NUMÉRATEUR !).
5. Résonance : exciter à $f_0$ !

## R1 — ENTRAÎNEMENT (pendule : Terre vs Lune)

🏷️ matière=PC · année=— · session=— · chapitre=P15 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=pendule-simple-g-variable · niveau=★ · compétence=formule+racine · barème=—

**Énoncé.** Pendule simple $l = 2{,}0$ m. a) $T_0$, $f_0$ sur Terre ? b) $T_0$ sur la Lune ($g = 1{,}6$) ?

**Corrigé-type.** a) $T_0 = 2\pi\sqrt{2{,}0/9{,}8} = \boxed{2{,}84\text{ s}}$, $f_0 = \boxed{0{,}352\text{ Hz}}$. b) $T_0 = 2\pi\sqrt{2{,}0/1{,}6} = \boxed{7{,}0\text{ s}}$ ($\times 2{,}5$ : $g$ au dénominateur !).
🪤 *Piège testé : b) $T_0$ « $\times 6$ » ($g$ $\div 6$) — RACINE : $T_0 \propto 1/\sqrt{g}$ → $\times\sqrt{6} = \times 2{,}45$ !*
🗣️ الخلاصة : الجاذبية تحت **الجذر** — ملي $g$ كتنقص، الدور كيكبر بالجذر ماشي بالتناسب المباشر.

## R2 — ENTRAÎNEMENT (mesurer $g$ : 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P15 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=mesure-g-graphique · niveau=★★ · compétence=formule+linéarisation · barème=—

**Énoncé.** Pendule simple $l = 0{,}990$ m, $T_0 = 2{,}00$ s mesurée. En déduire $g$. Pourquoi petits angles ?

**Corrigé-type — Méthode 1 (formule).** $g = 4\pi^2l/T_0^2 = 39{,}5\times0{,}990/4{,}00 = \boxed{9{,}77\text{ m/s}^2}$ ✓.

**Corrigé-type — Méthode 2 (pente graphique).** $T_0^2 = (4\pi^2/g)\,l$ : tracer $T_0^2 = f(l)$ → droite de pente $p = 4\pi^2/g$ → $g = 4\pi^2/p$. 1 point ($l = 0{,}990$, $T_0^2 = 4{,}00$) : $p = 4{,}00/0{,}990 = 4{,}04$ → $g = 39{,}5/4{,}04 = \boxed{9{,}77\text{ m/s}^2}$ ✓. (En TP : plusieurs $l$ → pente = précision !)
Petits angles : $T_0 = 2\pi\sqrt{l/g}$ exige $\sin\theta \approx \theta$ — à $30°$, $T$ augmente et $g$ serait SOUS-estimé !
🪤 *Piège testé : $g = l(T_0/2\pi)^2$ (formule inversée !) — $T_0 = 2\pi\sqrt{l/g}$ → $g = 4\pi^2l/T_0^2$ : $g$ au NUMÉRATEUR.*
🗣️ الخلاصة : باش تعبر $g$، ربع الدور وخط مستقيم — والميل ديالو كيعطيك $g$ بدقة أكثر من نقطة وحدة.

## R3 — ENTRAÎNEMENT (torsion : $J$ et $C$)

🏷️ matière=PC · année=— · session=— · chapitre=P15 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=torsion-J-C · niveau=★★ · compétence=RFD-rotation+formule · barème=—

**Énoncé.** Disque ($m = 0{,}50$ kg, $R = 10$ cm) suspendu à un fil de torsion ($C = 0{,}020$ N·m/rad). a) $J$ du disque ? b) $T_0$ ? c) On mesure $T_0 = 3{,}5$ s : retrouver $C$ ?

**Corrigé-type.** a) $J = \tfrac{1}{2}mR^2 = 0{,}5\times0{,}50\times0{,}10^2 = \boxed{2{,}5\times10^{-3}\text{ kg·m}^2}$. b) $T_0 = 2\pi\sqrt{2{,}5\times10^{-3}/0{,}020} = 2\pi\sqrt{0{,}125} = \boxed{2{,}2\text{ s}}$. c) $C = 4\pi^2J/T_0^2 = 39{,}5\times2{,}5\times10^{-3}/12{,}25 = \boxed{8{,}1\times10^{-3}\text{ N·m/rad}}$.
🪤 *Piège testé : $R = 10$ (cm !) → $J$ faux $\times 100$ — SI : $R = 0{,}10$ m AVANT $R^2$ (le carré AMPLIFIE l'erreur !).*
🗣️ الخلاصة : الليّ بحال النابض الدوّار — $J$ لفوق و $C$ لتحت، والوحدات **قبل** التربيع.

## R4 — ENTRAÎNEMENT (balançoire : résonance)

🏷️ matière=PC · année=— · session=— · chapitre=P15 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=résonance-pendule · niveau=★★ · compétence=raisonnement-phase · barème=—

**Énoncé.** Balançoire $T_0 = 2{,}0$ s. a) Longueur équivalente (pendule simple) ? b) Fréquence de poussée optimale ? c) Pousser à $1{,}0$ Hz ?

**Corrigé-type.** a) $l = gT_0^2/4\pi^2 = 9{,}8\times4{,}0/39{,}5 = \boxed{0{,}99\text{ m}}$. b) $f = f_0 = \boxed{0{,}50\text{ Hz}}$ (1 poussée / 2 s — RÉSONANCE). c) À $1{,}0$ Hz : une poussée sur deux arrive à CONTRE-TEMPS et freine — l'amplitude s'effondre !
🪤 *Piège testé : « pousser plus fort à n'importe quel rythme » — hors résonance, la force compense au lieu d'accumuler : le RYTHME bat la FORCE.*
🗣️ الخلاصة : الدفع القوي بلا إيقاع كيفرمل — **الإيقاع الصحيح** هو اللي كيكبّر الأرجوحة.

## R5 — ENTRAÎNEMENT (balançoire synchrone, esprit 2023N)

🏷️ matière=PC · année=— · session=— · chapitre=P15 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=pendule-pesant-synchrone · niveau=★★★ · compétence=RFD+pendule-synchrone · barème=—

**Énoncé.** Enfant + balançoire : $J_\Delta = 120$ kg·m², $m = 30$ kg, $d = 1{,}5$ m (G-axe). a) Établir l'EDL (petits angles) et $T_0$. b) Longueur du pendule simple synchrone ?

**Corrigé-type.** a) RFD : $-mgd\,\theta = J_\Delta\ddot\theta$ → $\boxed{\ddot\theta + (mgd/J_\Delta)\theta = 0}$. $T_0 = 2\pi\sqrt{120/(30\times9{,}8\times1{,}5)} = 2\pi\sqrt{0{,}272} = \boxed{3{,}28\text{ s}}$. b) Synchrone : $2\pi\sqrt{l/g} = T_0$ → $l = gT_0^2/4\pi^2 = 9{,}8\times10{,}76/39{,}5 = \boxed{2{,}67\text{ m}}$.
🪤 *Piège testé : $d$ = longueur des cordes — NON : $d$ = distance G-AXE (l'enfant n'est pas ponctuel !).*
🗣️ الخلاصة : الرقاص المتزامن هو **البسيط اللي عندو نفس الدور** — $d$ هي المسافة من G للمحور ماشي طول الحبل.

## R6 — ENTRAÎNEMENT (torsion énergétique, esprit 2025R)

🏷️ matière=PC · année=— · session=— · chapitre=P15 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=torsion-énergie-travail · niveau=★★★ · compétence=énergie+travail-couple · barème=—

**Énoncé.** Pendule de torsion : $J = 2{,}0\times10^{-3}$ kg·m², $C = 8{,}0\times10^{-2}$ N·m/rad, lâché à $\theta_m = 0{,}20$ rad sans vitesse. a) $E_m$ ? b) $\dot\theta_{max}$ ? c) Travail du couple de torsion entre $\theta_m$ et 0 ?

**Corrigé-type.** a) $E_m = \tfrac12C\theta_m^2 = 0{,}5\times8{,}0\times10^{-2}\times0{,}04 = \boxed{1{,}6\times10^{-3}\text{ J}}$. b) Au passage par 0 : $E_m = \tfrac12J\dot\theta_{max}^2$ → $\dot\theta_{max} = \sqrt{2E_m/J} = \sqrt{3{,}2/2{,}0} = \boxed{1{,}26\text{ rad/s}}$. c) $W_C = \Delta E_c = E_m - 0 = \boxed{1{,}6\times10^{-3}\text{ J}}$ (moteur : le couple fait tourner !).
🪤 *Piège testé : $W_C = -\Delta E_p$ avec signe faux — $W_C = +\Delta E_c$ (moteur quand $\theta$ diminue vers 0) ; shunter par $E_m$ = cste !*
🗣️ الخلاصة : الطاقة محفوظة = **اختصار ذهبي** — السرعة العظمى والشغل بلا معادلات تفاضلية.

## VRAIE — 2025R Ex4-P2 (pendule de torsion : $T_0$, $C$, $E_m$, $W$)

🏷️ matière=PC · année=2025 · session=R · chapitre=P15 · type=VRAIE · fidélité=reconstitué-corrigé · type_question=torsion-complet-RFD-énergie · niveau=★★★ · compétence=RFD+graphique+énergie · barème=~2,75/5,5 (P1 = skieur P12)

> Reconstitué d'après les éléments de réponse officiels (direction provinciale Mohammedia, via scribd) — structure, questions et valeurs fidèles ; énoncé exact à recouper sur le PDF officiel.
**RFD.** Système {pendule} : $\vec P$ (moment nul sur l'axe), $\vec R$ (nul), couple de torsion $-C\theta$ → $\boxed{\ddot\theta + (C/J_\Delta)\theta = 0}$.
**Solution.** $\theta(t) = \theta_m\cos(2\pi t/T_0 + \varphi)$ ; $T_0 = 2\pi\sqrt{J_\Delta/C}$. Graphique : $\boxed{T_0 = 4{,}0\text{ s}}$ (lu) ; $J_\Delta = CT_0^2/4\pi^2 = 7{,}97\times10^{-2}\times16/39{,}48 = \boxed{3{,}23\times10^{-2}\text{ kg·m}^2}$ (déduit : $J$ et $\dot\theta_m$ graphique non relus) ; $\dot\theta_m = \sqrt{2E_m/J_\Delta} = \boxed{0{,}22\text{ rad/s}}$ → $\theta_m = T_0\dot\theta_m/2\pi = \boxed{0{,}14\text{ rad}}$ (⚠️ CORRIGÉ le 2026-09-15 : 0,17 incohérent avec $C$/$E_m$/$W_C$). D'où $\boxed{C = 7{,}97\times10^{-2}\text{ N·m/rad}}$ (lu).
**Énergie.** $E_m$ conservée : $E_m = \tfrac12J_\Delta\dot\theta_m^2 = \boxed{8{,}07\times10^{-4}\text{ J}}$. Travail du couple : $W_C = \Delta E_c = \tfrac{J_\Delta}{2}[\dot\theta^2(t_2) - \dot\theta^2(t_1)] = \boxed{7{,}99\times10^{-4}\text{ J}}$ (lu ; $\dot\theta$ : 0 → 0,22 rad/s — $t_2$ ≈ passage à l'équilibre, écart 0,8 % = arrondis).
🪤 *vraie : $\theta_m$ via $\dot\theta_m$ GRAPHIQUE ($\theta_m = T_0\dot\theta_m/2\pi$) ; $C$ depuis $T_0$ (pas l'inverse !) ; $W_C$ = $\Delta E_c$ directement.*
🗣️ الخلاصة : الوطني 2025 عطى الليّ **كامل** — المعادلة، الدور من المنحنى، الثابتة $C$، الطاقة، والشغل : 5 أسئلة فسلسلة وحدة.

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $T_0 \propto 1/g$ | racine : $\times\sqrt{}$ |
| R2 | $g$ inversé | $g = 4\pi^2l/T^2$ (M2 : pente !) |
| R3 | cm dans $R^2$ | SI avant le carré ! |
| R4 | force > rythme | résonance = phase ! |
| R5 | $d$ = cordes | $d$ = G-axe ! |
| R6 | signe de $W_C$ | $W_C = \Delta E_c$ (moteur) |
| 2025R | $\theta_m$ direct | $\theta_m = T_0\dot\theta_m/2\pi$ |
