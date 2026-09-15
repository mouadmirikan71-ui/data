> **Pointer** : `14_Pendule_elastique_horizontal` → P4 (3 type-bac : EDP, 2 méthodes, vertical) → corrigés-types + pièges testés.
> Jumeau angulaire (pesant, torsion, résonance) → `15_Pendule_pesant_et_torsion`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Pendule élastique horizontal (P14)

## Méthode — élastique en 5 gestes 🧭

1. **SI !** (kg, m, N/m — convertir g, cm).
2. PFD : $-kx = m\ddot{x}$ → $\ddot{x} + (k/m)x = 0$.
3. $T_0 = 2\pi\sqrt{m/k}$ ($m$ en haut !).
4. $v_{max} = \omega_0X_m$ OU énergie ($\tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv^2$).
5. $\varphi$ depuis les initiales (lâché → 0).

## R1 — TYPE-BAC (établir l'EDP + $T_0$)

🏷️ matière=PC · année=— · session=— · chapitre=P14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Masse $m = 100$ g, ressort $k = 10$ N/m, horizontal sans frottement. a) Établir l'équation différentielle. b) $T_0$ et $f_0$ ? c) On l'écarte de $4{,}0$ cm et on lâche sans vitesse : écrire $x(t)$.

**Corrigé-type.** a) PFD : $-kx = m\ddot{x}$ → $\boxed{\ddot{x} + 100x = 0}$ ($k/m = 10/0{,}10 = 100$). b) $T_0 = 2\pi\sqrt{0{,}10/10} = 2\pi(0{,}10) = \boxed{0{,}63\text{ s}}$, $f_0 = \boxed{1{,}6\text{ Hz}}$. c) $X_m = 0{,}040$ m, $\varphi = 0$ → $\boxed{x = 0{,}040\cos(10t)}$ (SI : m, s).
🪤 *Piège testé : $m = 100$ (g !) → $k/m = 0{,}1$ — convertir EN PREMIER : $100$ g $= 0{,}10$ kg, $4$ cm $= 0{,}04$ m.*

## R2 — TYPE-BAC ($v_{max}$, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $m = 0{,}20$ kg, $k = 20$ N/m, $X_m = 5{,}0$ cm. $T_0$ ? $v_{max}$ ?

**Corrigé-type.** $T_0 = 2\pi\sqrt{0{,}20/20} = \boxed{0{,}63\text{ s}}$. **Méthode 1 (cinématique)** : $\omega_0 = \sqrt{20/0{,}20} = 10$ rad/s → $v_{max} = 10\times0{,}050 = \boxed{0{,}50\text{ m/s}}$. **Méthode 2 (énergie)** : $\tfrac{1}{2}\times20\times0{,}050^2 = \tfrac{1}{2}\times0{,}20\times v^2$ → $v = \boxed{0{,}50\text{ m/s}}$ ✓ ($E = 0{,}025$ J).
🪤 *Piège testé : $X_m = 5{,}0$ (cm !) → $v = 50$ m/s — TOUT en SI : $5{,}0$ cm $= 0{,}050$ m AVANT de calculer.*

## R3 — TYPE-BAC (ressort vertical)

🏷️ matière=PC · année=— · session=— · chapitre=P14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Même ressort ($k = 20$ N/m) vertical, masse $m = 0{,}20$ kg. a) Allongement à l'équilibre ? b) $T_0$ des oscillations autour de l'équilibre ? c) Pourquoi identique à l'horizontal ?

**Corrigé-type.** a) Équilibre : $k\Delta l = mg$ → $\Delta l = 0{,}20\times9{,}8/20 = \boxed{9{,}8\text{ cm}}$. b) $\boxed{T_0 = 0{,}63\text{ s}}$ (même $m$, même $k$ !). c) Le poids CONSTANT décale l'équilibre ; autour de celui-ci : $\ddot{X} + (k/m)X = 0$ identique — $g$ ne figure pas dans $T_0$.
🪤 *Piège testé : « le poids s'ajoute au rappel → $T_0$ change » — le poids est CONSTANT : seules les forces VARIABLES pilotent la dynamique !*

## R4 — ENTRAÎNEMENT (style 2026N Ex4-P2 : énergie + raideur)

🏷️ matière=PC · année=— · session=— · chapitre=P14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★ · barème=—

> ⚠️ PAS une VRAIE : entraînement d'ambiance « 2026N Ex4-P2 » (partie oscillateur repérée : descripteur $E_m$, $K$ — sujet 2026N non relu : PDF sur Google Drive, illisibles depuis la sandbox). Upgrade en VRAIE dès relecture du sujet.
> Données : solide $m = 0,50$ kg sur plan horizontal sans frottement, ressort $K = 20$ N/m, énergie mécanique $E_m = 6,0$ J.

**Énoncé.** (a) Amplitude $X_m$ des oscillations. (b) Vitesse maximale $v_{max}$ (2 méthodes). (c) Période propre $T_0$.
**Corrigé-type :** (a) $E_m = \frac{1}{2}KX_m^2$ → $X_m = \sqrt{2E_m/K} = \sqrt{12/20} = \boxed{0,77\text{ m}}$. (b) **M1 énergie :** $E_m = \frac{1}{2}mv_{max}^2$ → $v_{max} = \sqrt{2E_m/m} = \sqrt{24} = \boxed{4,9\text{ m/s}}$. **M2 cinématique :** $v_{max} = X_m\omega_0 = X_m\sqrt{K/m} = 0,775\times\sqrt{40} = \boxed{4,9\text{ m/s}}$ ✔. (c) $T_0 = 2\pi\sqrt{m/K} = 2\pi\sqrt{0,025} = \boxed{1,0\text{ s}}$.
🪤 *Piège testé : $v_{max} = X_m/T_0$ (« vitesse = distance/temps » — FAUX en sinusoïdal : $v_{max} = X_m\omega_0$ !).*
🗣️ الخلاصة : الطاقة كتعطي كلشي: $X_m = \sqrt{2E_m/K} = 0,77$ m! والسرعة القصوى بجوج طرق (الطاقة ولا $X_m\omega_0$) = $4,9$ m/s! والدور $T_0 = 1,0$ s! الفخ: $v_{max}$ ماشي $X_m/T_0$ (هادي للحركة المنتظمة ماشي الجيبية)!

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | g/cm dans formules | SI d'abord ! |
| R2 | $X_m$ en cm | $0{,}050$ m avant calcul |
| R3 | poids → $T_0$ change | constant = décor, pas dynamique |
