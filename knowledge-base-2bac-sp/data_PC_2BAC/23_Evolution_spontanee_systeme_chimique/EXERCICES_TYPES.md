> **Pointer** : `23_Evolution_spontanee_systeme_chimique` → P4 (3 type-bac : bilan, K depuis E°, attaque 2 méthodes) → corrigés-types + pièges testés.
> Piles (Daniell, fém, Nernst, capacité) → `24_Piles_electrochimiques`. Forcer l'inverse → `25_Electrolyse`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Évolution spontanée (P23)

## Méthode — spontanéité en 5 gestes 🧭

1. Demi-éq (atomes PUIS charges !) + bilan ($e^-$ annulés !).
2. $Q_r$ : solides EXCLUS (métaux dehors !).
3. $K$ : $\log K = n\Delta E°/0{,}06$ ($n$ = $e^-$ du bilan !).
4. $Q_{r,i}$ (INITIALES !) vs $K$ → sens (P20 !).
5. Inverse : $K' = 1/K$ (sens unique !).

## R1 — TYPE-BAC (demi-éq + bilan : Daniell)

🏷️ matière=PC · année=— · session=— · chapitre=P23 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Couples $Zn^{2+}/Zn$ et $Cu^{2+}/Cu$. Écrire les demi-équations (sens spontané) et le bilan.

**Corrigé-type.** Oxydation (Zn, réducteur) : $\boxed{Zn \to Zn^{2+} + 2e^-}$ ; réduction ($Cu^{2+}$, oxydant) : $\boxed{Cu^{2+} + 2e^- \to Cu}$. Bilan : $\boxed{Zn + Cu^{2+} \to Zn^{2+} + Cu}$ (les $2e^-$ s'annulent !).
🪤 *Piège testé : bilan avec $e^-$ restants ($Zn + Cu^{2+} + 2e^- \to$…) — les $e^-$ DOIVENT s'annuler (multiplier les demi-éq si $n$ diffèrent !).*

## R2 — TYPE-BAC ($K$ depuis $E°$ : totale !)

🏷️ matière=PC · année=— · session=— · chapitre=P23 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $E°(Cu^{2+}/Cu) = +0{,}34$ V, $E°(Zn^{2+}/Zn) = -0{,}76$ V. $K$ de $Zn + Cu^{2+} \to Zn^{2+} + Cu$ ? Conclusion ?

**Corrigé-type.** $n = 2$ ($2e^-$ échangés !) → $\log K = 2\times(0{,}34+0{,}76)/0{,}06 = 2\times1{,}10/0{,}06 = 36{,}7$ → $\boxed{K = 4{,}6\times10^{36} \gg 10^4}$ : réaction quasi-TOTALE (va au bout !).
🪤 *Piège testé : $n = 1$ ($\log K = 18{,}3$) — $n$ = $e^-$ du BILAN (2 !) : un seul Zn libère DEUX $e^-$.*

## R3 — TYPE-BAC (attaque : Zn OUI, Cu NON — 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P23 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** a) Lame Zn dans $Cu^{2+}$ $0{,}01$ M + $Zn^{2+}$ $1{,}0$ M : attaquée ? b) Lame Cu dans $Zn^{2+}$ $0{,}01$ M + $Cu^{2+}$ $1{,}0$ M ?

**Corrigé-type — Méthode 1 ($Q_{r,i}$ vs $K$).** a) $Q_{r,i} = 1{,}0/0{,}01 = 100 \ll K = 4{,}6\times10^{36}$ → $\boxed{\text{DIRECT : Zn attaqué, Cu déposé}}$ ✓. b) Sens $Cu + Zn^{2+} \to$ : $K' = 1/K = 2{,}2\times10^{-37}$, $Q'_{r,i} = 100 \gg K'$ → $\boxed{\text{RIEN : Cu intact}}$ ✓.

**Corrigé-type — Méthode 2 (signe de $E$).** $E = (0{,}06/n)\log(K/Q_{r,i})$ : a) $\log(4{,}6\times10^{36}/100) = 34{,}7 > 0$ → $E > 0$ → $\boxed{\text{spontané DIRECT}}$ ✓. b) $E' = (0{,}06/2)\log(K'/Q') = 0{,}03\times(-38{,}7) < 0$ → $\boxed{\text{non spontané : RIEN}}$ ✓. Même verdict par le signe de $E$.
🪤 *Piège testé : b) « symétrique donc attaque » — $K' = 1/K$ : le sens inverse est IMPOSSIBLE ($K' \approx 0$) : la spontanéité a UN sens !*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $e^-$ restants au bilan | annuler (multiplier si besoin !) |
| R2 | $n = 1$ | $e^-$ du bilan (2 !) |
| R3 | sens symétrique | $K' = 1/K$ (M2 : signe de $E$ !) |
