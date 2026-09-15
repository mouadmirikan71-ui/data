> **Pointer** : `11_Chute_libre_verticale` → P4 (R1-R4 type-bac + R5 Euler + R6 quadratique) + 3 VRAIES (2021N Ex5, 2026N Ex4-P1, 2024N bille) → corrigés-types + R2 en 2 méthodes.
> 🏷️ Schéma de tags : `matière · année · session · chapitre · type (VRAIE/ENTRAÎNEMENT) · fidélité (verbatim/reconstitué-corrigé/n.a.) · type_question · niveau · compétence · barème`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Chute libre verticale (P11)

## Méthode — chute en 6 gestes 🧭

1. Axe DESSINÉ + $v_0$ noté (signes !).
2. Libre : $v = gt$, $z = \tfrac{1}{2}gt^2$, $v^2 = 2gz$.
3. Fluide : $v_{lim}$ via équilibre ($a = 0$), pas besoin de l'équa diff !
4. Liquide : Archimède ($\times(1-\rho_f/\rho_s)$).
5. Flèche/hauteur : énergie = raccourci royal.
6. EDL insoluble ($v^2$) : droite $dv/dt = f(v^2)$ + Euler pas à pas.

## R1 — ENTRAÎNEMENT (chute libre : 80 m)

🏷️ matière=PC · année=— · session=— · chapitre=P11 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=chute-libre · niveau=★ · compétence=cinématique · barème=—

**Énoncé.** Objet lâché sans vitesse de $h = 80$ m ($g = 9,8$). $v$ d'arrivée ? durée ?

**Corrigé-type.** $t = \sqrt{2h/g} = \sqrt{160/9,8} = \boxed{4,0\text{ s}}$ ; $v = gt = \boxed{40\text{ m/s} \approx 143\text{ km/h}}$.
🪤 *Piège testé : $v = 9,8\times80$ (oublier $\sqrt{}$) — $v = gt$ avec $t = \sqrt{2h/g}$, PAS $v = gh$ !*
🗣️ الخلاصة : السقوط الحر = $z = \frac{1}{2}gt^2$ — الوقت هو **الجذر** ماشي القسمة المباشرة.

## R2 — ENTRAÎNEMENT (flèche, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P11 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=lancer-vertical-flèche · niveau=★★ · compétence=cinématique+énergie · barème=—

**Énoncé.** Balle lancée vers le haut, $v_0 = 15$ m/s. Hauteur max ? durée de montée ?

**Corrigé-type — Méthode 1 (cinématique).** $v^2 = v_0^2 - 2gz = 0$ → $h = v_0^2/2g = 225/19,6 = \boxed{11,5\text{ m}}$.
**Corrigé-type — Méthode 2 (énergie).** $\tfrac{1}{2}mv_0^2 = mgh$ → $h = v_0^2/2g$ — $m$ éliminée, même $\boxed{11,5\text{ m}}$, 1 ligne ! Montée : $t = v_0/g = \boxed{1,5\text{ s}}$.
🪤 *Piège testé : $v = +gt + v_0$ (axe ascendant !) — avec $Oz$ vers le haut, $g$ est NÉGATIF : $v = -gt + v_0$.*
🗣️ الخلاصة : الطاقة كتعطي الارتفاع فسطر واحد — والقانون كيحتارم **اتجاه المحور** اللي رسمتي.

## R3 — ENTRAÎNEMENT (TP bille dans l'huile : Stokes)

🏷️ matière=PC · année=— · session=— · chapitre=P11 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=Stokes+Archimède · niveau=★★ · compétence=PFD+régime-permanent · barème=—

**Énoncé.** Bille acier $r = 2,0$ mm, $\rho_s = 7800$ kg/m³, dans huile $\eta = 0,10$ Pa·s, $\rho_f = 900$ kg/m³. a) $m$ ? b) $v_{lim}$ sans puis avec Archimède ? c) $\tau$ ?

**Corrigé-type.** a) $m = \rho_s\tfrac{4}{3}\pi r^3 = 7800\times3,35\times10^{-8} = \boxed{2,6\times10^{-4}\text{ kg}}$. $k = 6\pi\eta r = \boxed{3,8\times10^{-3}\text{ kg/s}}$.
b) Sans $\Pi$ : $v = mg/k = 0,68$ m/s ; avec $\Pi$ : $\boxed{v_{lim} = 0,68\times(1-900/7800) = 0,60\text{ m/s}}$ (−12% !). c) $\tau = m/k = \boxed{69\text{ ms}}$ → permanent dès $\approx 0,35$ s.
🪤 *Piège testé : oublier Archimède (−12% = réponse fausse au bac) — dans un LIQUIDE, $\Pi$ n'est jamais négligeable !*
🗣️ الخلاصة : فالسائل نقص **دافعة أرخميدس** قبل ما تحسب — الجسم «كيفقد» من وزنو.

## R4 — ENTRAÎNEMENT (la goutte sauvée par l'air)

🏷️ matière=PC · année=— · session=— · chapitre=P11 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=vitesse-limite-air · niveau=★★ · compétence=équilibre+énergie · barème=—

**Énoncé.** Goutte $r = 1,0$ mm ($m = 4,2\times10^{-6}$ kg) tombe de 2000 m, $v_{lim} = 5,6$ m/s mesurée. a) $k$ (modèle $f = kv$) ? b) $E_c$ d'arrivée vs chute libre ?

**Corrigé-type.** a) $k = mg/v_{lim} = 4,2\times10^{-6}\times9,8/5,6 = \boxed{7,3\times10^{-6}\text{ kg/s}}$. b) Avec air : $E_c = \tfrac{1}{2}mv^2 = 6,6\times10^{-5}$ J ; chute libre : $v = \sqrt{2gh} = 198$ m/s → $E_c = 0,082$ J, soit **1250× plus** — sans air, la pluie serait une mitrailleuse !
🪤 *Piège testé : $k$ en N·s/m « bizarre » — $kv$ = N donc $k$ = N·s/m = kg/s : analyse dimensionnelle systématique !*
🗣️ الخلاصة : السرعة الحدية هي **التوازن** بين الوزن والاحتكاك — ملي $a = 0$ سالات الحكاية.

## R5 — ENTRAÎNEMENT (Euler pas à pas, esprit 2026N)

🏷️ matière=PC · année=— · session=— · chapitre=P11 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=Euler-quadratique · niveau=★★★ · compétence=EDL+Euler · barème=—

**Énoncé.** Chute avec $dv/dt + 0,010\,v^2 = 9,8$ (SI), $v_0 = 0$, $\Delta t = 0,20$ s. Calculer $v_1$, $v_2$ par Euler. Que vaut $v_{lim}$ ?

**Corrigé-type.** $a_0 = 9,8 - 0,010\times0 = 9,8$ → $v_1 = 0 + 9,8\times0,20 = \boxed{1,96\text{ m/s}}$. $a_1 = 9,8 - 0,010\times1,96^2 = 9,762$ → $v_2 = 1,96 + 9,762\times0,20 = \boxed{3,91\text{ m/s}}$. $v_{lim} = \sqrt{9,8/0,010} = \boxed{31,3\text{ m/s}}$ (contrôle : $v_2 \ll v_{lim}$ ✓, on est en tout début de chute).
🪤 *Piège testé : recalculer $a$ avec l'ANCIENNE vitesse — Euler = toujours la vitesse FRAÎCHE ($a_1$ depuis $v_1$ !).*
🗣️ الخلاصة : أويلر = حسب، زيد، **عاود بالجديد** — الغلطة الشائعة هي تعاود تستعمل السرعة القديمة.

## R6 — ENTRAÎNEMENT (parachute quadratique, esprit 2021N)

🏷️ matière=PC · année=— · session=— · chapitre=P11 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=frottement-v²+palier · niveau=★★★ · compétence=lecture-courbe+PFD · barème=—

**Énoncé.** Parachutiste 90 kg : $v(t)$ monte puis palier à $6,0$ m/s. a) Modèle : $mg - \mu v^2 = ma$. Déterminer $\mu$. b) Montrer que la phase initiale ($v \approx 20t$) est une chute libre.

**Corrigé-type.** a) Palier : $a = 0$ → $\mu = mg/v_{lim}^2 = 90\times9,8/36 = \boxed{24,5\text{ kg/m}}$. b) $v \approx 20t$ → pente $a \approx 20$ ? Non : $v = 20t$ donne $a = 20 \neq g$… **refaire** : si la tangente à l'origine a pour pente $9,8$ m/s², alors $a = g$ → seul le poids agit → chute libre ✓. (Moralité : c'est la PENTE qui parle, pas l'allure !)
🪤 *Piège testé : « ça monte droit donc c'est libre » — NON : il faut $a = g$ NUMÉRIQUEMENT (pente = 9,8).*
🗣️ الخلاصة : البالي = $a = 0$ كيعطيك $\mu$ — والبداية المستقيمة بميل $g$ كتثبت السقوط الحر.

## VRAIE — 2021N Ex5 (parachute : 5 m/s, 400 m)

🏷️ matière=PC · année=2021 · session=N · chapitre=P11 · type=VRAIE · fidélité=verbatim · type_question=chute-libre-puis-quadratique+distances · niveau=★★★ · compétence=PFD+lecture-courbe · barème=Ex5/5

Phase 1 (fermé) : $v = at$ linéaire → MRUV ; $a = \Delta v/\Delta t = 20/2 = 10 = g$ → chute libre ✓. Phase 2 (ouvert) : $mg - \alpha v^2 = ma$ → $dv/dt + (\alpha/m)v^2 = g$. $v_\ell = \sqrt{gm/\alpha} = 5$ m/s (palier) → $\alpha = gm/v_\ell^2 = 10\times100/25 = 40$ kg/m. Distances : $d_1 = \frac{1}{2}g\Delta t_1^2 = 80$ m ($\Delta t_1 = 4$ s) ; $d' = v_\ell\Delta t' = 180$ m ($\Delta t' = 36$ s) ; $d = h - d_1 - d' = 660-80-180 = 400$ m.
🪤 *vraie : chute libre à PROUVER ($a = g$ via pente !) ; $\alpha$ via $v_\ell$ ; découpage $d_1/d/d'$ (3 morceaux !).*
🗣️ الخلاصة : الوطني كيطلب **البرهان** ماشي الزعم — الميل $= g$ هو الدليل، والمسافة كتتقطع 3 طراف.

## VRAIE — 2026N Ex4-P1 (cascadeur sans parachute : Euler !)

🏷️ matière=PC · année=2026 · session=N · chapitre=P11 · type=VRAIE · fidélité=verbatim · type_question=chute-libre-vs-frottement+Euler · niveau=★★★ · compétence=PFD+EDL+Euler+esprit-critique · barème=4,25/5,5 (reste = P14)

Données : $H = 7620$ m, filet à $h = 70$ m, $m = 80$ kg, axe descendant, $v_0 = 0$, $v_{lim}$ réelle 200 km/h.
**Cas 1 (libre).** PFD : $a = g$ → $\boxed{z(t) = \tfrac12gt^2}$. $d = 7550$ m → $t_f = \sqrt{2d/g} = \boxed{39{,}25\text{ s}}$. $v_f = gt_f = 384{,}65$ m/s $= \boxed{1385\text{ km/h}}$ — très au-delà des 200 km/h réels → **modèle invalide** (frottement prépondérant).
**Cas 2 ($f = \mu v^2$).** $m\,dv_z/dt = mg - \mu v_z^2$ → $\boxed{dv_z/dt + (\mu/m)v_z^2 = g}$. Droite $dv_z/dt = f(v_z^2)$ : $v_{lim}^2 = 3120$ → $\boxed{v_{lim} = 55{,}9\text{ m/s}}$ ; $\mu = mg/v_{lim}^2 = 80\times9{,}8/3120 = \boxed{0{,}251\text{ kg/m}}$. $v_{lim} = 201$ km/h ≈ 200 ✓ → **modèle validé**.
**Euler** ($\Delta t = 0{,}5$ s, $\mu/m = 3{,}125\times10^{-3}$) : $v_1 = \boxed{4{,}9}$, $a_1 = \boxed{9{,}725}$, $v_2 = \boxed{9{,}763}$ m/s.
🪤 *vraie : conclusion « le modèle n'explique PAS la réalité » (comparer 1385 vs 200 !) ; $\mu$ via $v_{lim}$ GRAPHIQUE ; Euler avec la vitesse fraîche.*
🗣️ الخلاصة : الوطني 2026 كيسولك **واش النموذج صحيح** — الجواب بالأرقام : 1385 ضد 200، النموذج الأول غالط والثاني صحيح.

## VRAIE — 2024N (bille en chute dans un fluide : Archimède + $\mu$)

🏷️ matière=PC · année=2024 · session=N · chapitre=P11 · type=VRAIE · fidélité=reconstitué-corrigé · type_question=Stokes+Archimède+EDL · niveau=★★★ · compétence=PFD+EDL · barème=partie de l'Ex méca

> Énoncé reconstitué d'après la correction détaillée (RAFIK, scribd) — structure et questions fidèles, valeurs exactes à recouper sur le PDF officiel.
Système {bille} : $\vec P$ + poussée $\vec\Pi$ + frottement $\vec f = -\mu\vec v$. PFD projeté : $m\,dv_z/dt = mg - \Pi - \mu v_z$ → EDL $\boxed{dv_z/dt + (\mu/m)v_z = g(1-\rho_f/\rho_s)}$. Régime permanent : $\boxed{v_{lim} = mg(1-\rho_f/\rho_s)/\mu}$ (avec $\mu = 5{,}0\times10^{-2}$ kg/s d'après le corrigé). Sans Archimède on surestime $v_{lim}$ de $\rho_f/\rho_s$ (≈ 10-15 % dans l'eau) — l'écart qui fait perdre le point.
🪤 *vraie : le bilan à 3 forces (oublier $\Pi$ = EDL fausse dès la 1re ligne) ; $\mu$ en kg/s vs kg/m selon le modèle.*
🗣️ الخلاصة : 3 قوى ماشي 2 — **أرخميدس** كاين فالسائل، واللي نساه مشا ليه التمرين كامل.

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $v = gh$ | $v = gt$, $t = \sqrt{2h/g}$ |
| R2 | signe de $g$ | axe dessiné AVANT équations |
| R3 | Archimède oublié | liquide → $\Pi$ toujours ! |
| R4 | unités de $k$ | $kv$ = N → $k$ = kg/s |
| R5 | Euler avec $v$ ancienne | toujours la vitesse FRAÎCHE |
| R6 | « droit = libre » | pente $= g$ numériquement ! |
| 2021N | découpage distances | 3 morceaux : $d_1/d/d'$ |
| 2026N | pas de conclusion modèle | comparer prédiction vs mesure |
| 2024N | bilan à 2 forces | $\vec P + \vec\Pi + \vec f$ |
