> **Pointer** : `02_Ondes_mecaniques_progressives_periodiques` → P4 (4 type-bac : corde, phase 2 méthodes, son, cuve) → corrigés-types + pièges testés.
> Socle propagation ($v$, $\tau$, sonar, séisme) → `01_Ondes_mecaniques_progressives`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Ondes périodiques (P02)

## Méthode — périodicité en 4 gestes 🧭

1. **SI !** (m, s, Hz — convertir km, ms, cm).
2. $\lambda = v/f$ (ou $vT$).
3. Phase : $\Delta x/\lambda$ → entier = phase, $+1/2$ = opposition (idem $\tau/T$).
4. Graphes : axe temps → $T$ ; axe espace → $\lambda$ ; mesurer sur $n$ motifs.

## R1 — TYPE-BAC (corde : $\lambda$, retard, phase)

🏷️ matière=PC · année=— · session=— · chapitre=P2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Corde : source $f = 50$ Hz, $v = 10$ m/s. a) $\lambda$ ? b) Retard en $x = 0{,}50$ m ? c) Ce point vibre-t-il en phase avec la source ?

**Corrigé-type.** a) $\lambda = v/f = 10/50 = \boxed{0{,}20\text{ m}}$. b) $\tau = x/v = 0{,}50/10 = \boxed{0{,}050\text{ s}}$ ($= 2{,}5T$ : $T = 0{,}020$ s). c) $x/\lambda = 0{,}50/0{,}20 = 2{,}5 = 2+1/2$ → $\boxed{\text{opposition de phase}}$.
🪤 *Piège testé : « $\tau = 0{,}05$ s, grand → en phase » — le retard ABSOLU ne dit rien : seul $x/\lambda$ (ou $\tau/T$) tranche.*

## R2 — TYPE-BAC (phase : 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Même corde. Deux points $M_1$, $M_2$ distants de $0{,}30$ m : comparer leurs mouvements.

**Corrigé-type — Méthode 1 (espace).** $\Delta x/\lambda = 0{,}30/0{,}20 = 1{,}5 = 1+1/2$ → $\boxed{\text{opposition}}$ (mouvements contraires).

**Corrigé-type — Méthode 2 (temps).** $\tau = 0{,}30/10 = 0{,}030$ s ; $\tau/T = 0{,}030/0{,}020 = 1{,}5$ → demi-période excédentaire → $\boxed{\text{opposition}}$. Même verdict par le temps.
🪤 *Piège testé : $1{,}5 \approx 1$ ou $2$ (« presque entier ») — NON : $1{,}5 = 1+1/2$ EXACT = opposition parfaite. L'exactitude compte !*

## R3 — TYPE-BAC (son : $\lambda$ + phase)

🏷️ matière=PC · année=— · session=— · chapitre=P2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Diapason $f = 440$ Hz ($v_{son} = 340$ m/s). a) $\lambda$ ? b) Deux points distants de $1{,}55$ m sur l'axe de propagation : en phase ?

**Corrigé-type.** a) $\lambda = 340/440 = \boxed{0{,}773\text{ m}}$. b) $\Delta x/\lambda = 1{,}55/0{,}773 = 2{,}005 \approx 2$ → $\boxed{\text{en phase}}$ (mêmes mouvements).
🪤 *Piège testé : $2{,}005 \ne 2$ « donc pas en phase » — ici l'écart vient des ARRONDIS ($0{,}773$ tronqué) : $2{,}005 \approx 2$ à $0{,}2$ % près → en phase. Distinguer arrondi de calcul ($2{,}005$) et vraie demi-période ($1{,}5$ !).*

## R4 — TYPE-BAC (cuve à ondes : mesure de $\lambda$)

🏷️ matière=PC · année=— · session=— · chapitre=P2 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Cuve à ondes ($f = 20$ Hz) : sur une photo, 5 interfranges consécutifs occupent $10{,}0$ cm. a) $\lambda$ ? b) Célérité des ondes à la surface de l'eau ?

**Corrigé-type.** a) 5 motifs → $5\lambda = 10{,}0$ cm → $\lambda = \boxed{2{,}00\text{ cm} = 0{,}0200\text{ m}}$. b) $v = \lambda f = 0{,}0200 \times 20 = \boxed{0{,}400\text{ m/s}}$.
🪤 *Piège testé : $\lambda = 10$ cm (prendre le tout pour un motif) — compter les MOTIFS ($n$), diviser par $n$ : mesurer large puis diviser = précision !*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | retard absolu = phase | $x/\lambda$ (ou $\tau/T$) seul tranche |
| R2 | $1{,}5 \approx$ entier | $1+1/2$ exact = opposition |
| R3 | $2{,}005 \ne 2$ | arrondi de calcul ≠ demi-période |
| R4 | tout = un motif | compter $n$, diviser par $n$ |
