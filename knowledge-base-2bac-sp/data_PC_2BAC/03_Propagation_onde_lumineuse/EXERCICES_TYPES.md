> **Pointer** : `03_Propagation_onde_lumineuse` → P4 (4 type-bac : diffraction, Young, prisme, éclair) → corrigés-types + R2 en 2 méthodes.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Ondes lumineuses (P03)

## Méthode — lumière en 5 gestes 🧭

1. **Compter les fentes** (1 → tache $L$ ; 2 → franges $i$).
2. Identifier $a$ (largeur ? distance ?).
3. **TOUT en SI** (m ! rad !).
4. $L = 2\lambda D/a$ ou $i = \lambda D/a$ (ou inversées !).
5. Ordre de grandeur ($\lambda$ ~ nm, $i$ ~ mm ?).

## R1 — TYPE-BAC (diffraction : tache)

🏷️ matière=PC · année=— · session=— · chapitre=P3 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Fente $a = 0,10$ mm, laser $\lambda = 650$ nm, écran $D = 2,0$ m. a) $\theta$ ? b) Largeur $L$ de la tache centrale ?

**Corrigé-type.** SI : $a = 10^{-4}$ m, $\lambda = 6,5\times10^{-7}$ m. a) $\theta = \lambda/a = 6,5\times10^{-3}$ rad $= \boxed{6,5\text{ mrad}}$. b) $L = 2\lambda D/a = 2\times6,5\times10^{-7}\times2/10^{-4} = \boxed{2,6\text{ cm}}$.
🪤 *Piège testé : $L = 1,3$ cm (oublier le 2) — TACHE centrale = 2 côtés : $L = 2\lambda D/a$, toujours !*

## R2 — TYPE-BAC (Young : $\lambda$ en 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P3 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Young : $a = 0,50$ mm, $D = 2,0$ m. On mesure $i = 2,4$ mm (et $x_5 = 12$ mm pour la 5ᵉ frange brillante). Déterminer $\lambda$.

**Corrigé-type — Méthode 1 ($i$ direct).** $\lambda = ia/D = 2,4\times10^{-3}\times0,5\times10^{-3}/2 = \boxed{6,0\times10^{-7}\text{ m} = 600\text{ nm}}$.

**Corrigé-type — Méthode 2 (ordre 5).** $x_5 = 5\lambda D/a$ → $\lambda = x_5a/(5D) = 12\times10^{-3}\times0,5\times10^{-3}/10 = \boxed{600\text{ nm}}$. Même $\lambda$ (M2 souvent plus précise : $x_5$ grand !).
🪤 *Piège testé : $\lambda = 6,0\times10^{-4}$ m (mm non convertis) — $i$(m) $\times$ $a$(m) $/$ $D$(m) : tout en MÈTRES ou tout est faux.*

## R3 — TYPE-BAC (prisme : rouge vs bleu)

🏷️ matière=PC · année=— · session=— · chapitre=P3 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Prisme : $n_{rouge} = 1,51$, $n_{bleu} = 1,53$. a) Lequel est le plus dévié ? Pourquoi ? b) Incidence $i = 45$° (air→verre) : calculer $r_{rouge}$ et $r_{bleu}$.

**Corrigé-type.** a) Le BLEU ($n$ plus grand → réfraction plus forte → plus dévié). b) Snell : $\sin r = \sin45°/n$. Rouge : $0,7071/1,51 = 0,4683$ → $r = \boxed{27,9°}$. Bleu : $0,7071/1,53 = 0,4622$ → $r = \boxed{27,5°}$. Écart $0,4$° → séparation (spectre !).
🪤 *Piège testé : « rouge + dévié (couleur chaude = énergie ?) » — NON : $n_{bleu} > n_{rouge}$, le bleu dévie TOUJOURS plus (mémoriser !).*

## R4 — TYPE-BAC (éclair + tonnerre : $c$ vs $v_{son}$)

🏷️ matière=PC · année=— · session=— · chapitre=P3 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Éclair vu, tonnerre entendu $6,0$ s après. a) Distance de l'orage ? b) Montrer que le retard lumineux est négligeable.

**Corrigé-type.** a) $d = v_{son}\Delta t = 340\times6,0 = \boxed{2040\text{ m} \approx 2,0\text{ km}}$ (son à $v$ finie, lumière quasi-instantanée). b) $t_{lum} = d/c = 2040/(3\times10^8) \approx 7\times10^{-6}$ s $\ll 6$ s → $\boxed{\text{négligeable}}$ (×1 million !).
🪤 *Piège testé : $d = c\Delta t$ (appliquer $c$ au SON) — le retard vient du SON (lent) : $d = v_{son}\Delta t$, $c$ ne sert qu'en b).*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $L$ sans le 2 | tache = $2\lambda D/a$ |
| R2 | mm non convertis | SI (m) AVANT de calculer |
| R3 | rouge + dévié | $n_b > n_r$ : bleu + dévié |
| R4 | $d = c\Delta t$ | retard = SON : $d = v_{son}\Delta t$ |

## VRAIE — 2021N Ex2 (prisme + diffraction + cheveu)

🏷️ matière=PC · année=2021 · session=N · chapitre=P3 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
QCM : blanche = polychromatique. Prisme : $\nu_j = c/589\text{nm} = 5,09\times10^{14}$ Hz ; $v_j = 355\text{nm}\times\nu_j = 1,81\times10^8$ m/s $< v_r = 1,85\times10^8$ → dispersion ($v$ dépend de $\nu$). Diffraction : $L = 2\lambda D/a$ ; pente $K = \Delta L/\Delta D = 2\times10^{-2}$ → $\lambda = aK/2 = 0,06\text{mm}\times0,02/2 = 600$ nm. Cheveu : $d = 2\lambda D_2/L_1 = 2\times6\times10^{-7}\times2/3\times10^{-2} = 80$ μm.
🪤 *vraie : $\lambda$ via PENTE (pas un point !) ; cheveu = fente (Babinet) ; $v_j < v_r$ ($n$ plus grand pour jaune !).*
