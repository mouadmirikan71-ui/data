> **Pointer** : `28_BONUS_Satellites_et_planetes` → P4 (4 type-bac : ISS, géostat, GPS, Lune) → corrigés-types + R2 en 2 méthodes.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Satellites et planètes (P28)

## Méthode — orbite en 5 gestes 🧭

1. Première ligne : $r = R_T + h$ (en MÈTRES !).
2. $v = \sqrt{GM/r}$, $T = 2\pi r/v$.
3. Géostat : équatorial + $T = 86164$ s.
4. Kepler : $T^2/r^3$ = cste (comparaisons sans $G$ ni $M$ !).
5. Ordre de grandeur : ISS ~8 km/s ~90 min ; géostat 3 km/s 24 h.

## R1 — TYPE-BAC (ISS : 400 km)

🏷️ matière=PC · année=— · session=— · chapitre=P28 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** ISS : $h = 400$ km. $v$ ? $T$ ? ($R_T = 6380$ km, $GM_T = 3,98\times10^{14}$ SI.)

**Corrigé-type.** $r = 6,78\times10^6$ m. $v = \sqrt{3,98\times10^{14}/6,78\times10^6} = \boxed{7,66\text{ km/s}}$ ; $T = 2\pi r/v = \boxed{5,56\times10^3\text{ s} \approx 93\text{ min}}$.
🪤 *Piège testé : $r = 400$ km (oublier $R_T$ → $v = 31$ km/s, absurde !) — première ligne TOUJOURS : $r = R_T + h$.*

## R2 — TYPE-BAC (géostat, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P28 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Retrouver $h$ de l'orbite géostationnaire ($T = 86164$ s).

**Corrigé-type — Méthode 1 (directe).** $r = \sqrt[3]{GMT^2/4\pi^2} = \sqrt[3]{3,98\times10^{14}\times7,42\times10^9/39,5} = 4,22\times10^7$ m → $h = r - R_T = \boxed{35800\text{ km}}$.
**Corrigé-type — Méthode 2 (Kepler via la Lune !).** $r = r_L(T/T_L)^{2/3} = 384400\times(86164/2360448)^{2/3} = 384400\times0,110 = 42294$ km → $h = \boxed{35900\text{ km}}$ (écart 0,3% : orbite lunaire pas parfaitement circulaire — et zéro $G$ utilisé !).
🪤 *Piège testé : $T = 86400$ s → $h$ faux de ~100 km — géostat = jour SIDÉRAL 86164 s, pas solaire !*

## R3 — TYPE-BAC (GPS : 12 h)

🏷️ matière=PC · année=— · session=— · chapitre=P28 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** GPS : $T = 11$ h $58$ min $= 43080$ s. Altitude $h$ ?

**Corrigé-type.** $r = \sqrt[3]{3,98\times10^{14}\times(4,308\times10^4)^2/39,5} = 2,66\times10^7$ m → $h = 26550 - 6380 = \boxed{20200\text{ km}}$ (2 tours/jour : $T \approx T_{sidéral}/2$ ✓).
🪤 *Piège testé : « $T$ = moitié du géostat donc $h$ = moitié » — $T \propto r^{3/2}$ : $T/2$ → $r/2^{2/3} = r/1,59$, PAS $r/2$ !*

## R4 — TYPE-BAC (la Lune obéit à Kepler)

🏷️ matière=PC · année=— · session=— · chapitre=P28 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Lune : $T = 27,32$ j, $r = 384400$ km. Vérifier $T^2/r^3 = 4\pi^2/GM_T$.

**Corrigé-type.** $T = 2,360\times10^6$ s → $T^2/r^3 = 5,57\times10^{12}/5,68\times10^{25} = 9,8\times10^{-14}$ ; $4\pi^2/GM_T = 39,5/3,98\times10^{14} = 9,9\times10^{-14}$. Écart 1% : $\boxed{\text{la Lune vérifie Kepler 3}}$ ✓.
🪤 *Piège testé : jours non convertis ($T = 27,32$ dans $T^2/r^3$ avec $r$ en km — unités incohérentes !) — TOUT en SI avant de calculer.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $r = h$ | $r = R_T + h$, 1re ligne |
| R2 | 86400 s | géostat = 86164 s |
| R3 | $T/2$ → $r/2$ | $T \propto r^{3/2}$ |
| R4 | jours + km mélangés | tout en SI d'abord |
