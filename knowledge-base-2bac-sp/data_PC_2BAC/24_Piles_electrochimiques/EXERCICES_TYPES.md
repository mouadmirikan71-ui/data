> **Pointer** : `24_Piles_electrochimiques` → P4 (3 type-bac : anatomie, Nernst 2 méthodes, capacité) → corrigés-types + pièges testés.
> Spontanéité (redox, critère, $K$) → `23_Evolution_spontanee_systeme_chimique`. Envers → `25_Electrolyse`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Piles (P24)

## Méthode — piles en 5 gestes 🧭

1. Demi-éq + bilan ($e^-$ annulés !).
2. Anode(−) = oxydation ; cathode(+) = réduction.
3. $E = E(+) - E(-)$ (> 0 !).
4. Nernst : $E = E° - (0{,}06/n)\log Q_r$ ($n$ = $e^-$ !).
5. Capacité : $Q = n(e^-)F$ ($n(e^-) = \nu\times n$ !) + $Q = It$.

## R1 — TYPE-BAC (Daniell : anatomie complète)

🏷️ matière=PC · année=— · session=— · chapitre=P24 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Pile $Zn/Zn^{2+}(1M)\ ||\ Cu^{2+}(1M)/Cu$. Demi-éq, bilan, pôles, $e^-$, pont ?

**Corrigé-type.** $(-)Zn$ : $Zn \to Zn^{2+} + 2e^-$ (oxydation, rongé) ; $(+)Cu$ : $Cu^{2+} + 2e^- \to Cu$ (déposé, solution pâlit). Bilan : $Zn + Cu^{2+} \to Zn^{2+} + Cu$. $e^-$ : $Zn \to Cu$ (fil) ; courant : $Cu \to Zn$. Pont : $+$ → cathode, $-$ → anode.
🪤 *Piège testé : « $e^-$ : + vers − » — les $e^-$ partent du MOINS (anode, source) vers le PLUS ; c'est le COURANT qui va de + vers − !*

## R2 — TYPE-BAC (Nernst, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P24 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Daniell ($E° = 1{,}10$ V) avec $[Zn^{2+}] = 0{,}10$ M, $[Cu^{2+}] = 1{,}0$ M. $E$ ?

**Corrigé-type — Méthode 1 ($Q_r$ global).** $Q_r = 0{,}10/1{,}0 = 0{,}10$ → $E = 1{,}10-0{,}03\log(0{,}1) = 1{,}10 + 0{,}03 = \boxed{1{,}13\text{ V}}$.
**Corrigé-type — Méthode 2 (électrodes).** $E(Cu) = 0{,}34$ ; $E(Zn) = -0{,}76+0{,}03\log(0{,}1) = -0{,}79$ → $E = 0{,}34+0{,}79 = \boxed{1{,}13\text{ V}}$ ✓.
🪤 *Piège testé : $n = 1$ ($E = 1{,}16$ V) — $n = 2$ $e^-$ échangés : $0{,}06/2 = 0{,}03$ !*

## R3 — TYPE-BAC (pile : combien d'heures ?)

🏷️ matière=PC · année=— · session=— · chapitre=P24 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Pile Zn $6{,}5$ g ($0{,}10$ mol), $I = 0{,}20$ A. a) $Q$ ? autonomie ? b) Énergie ($E = 1{,}10$ V) ? c) Zn mangé en $1$ h ?

**Corrigé-type.** a) $Q = 0{,}10\times2\times96500 = \boxed{19300\text{ C}}$ → $t = 19300/0{,}20 = \boxed{96500\text{ s} \approx 26{,}8\text{ h}}$. b) $W = 1{,}10\times19300 = \boxed{21\text{ kJ}}$. c) $n(e^-) = 0{,}2\times3600/96500 = 7{,}46\times10^{-3}$ → $m(Zn) = 3{,}73\times10^{-3}\times65{,}4 = \boxed{0{,}24\text{ g}}$.
🪤 *Piège testé : $Q = 0{,}10\times96500$ (×1 !) — $n(e^-) = 2\times n(Zn)$ : UN Zn libère DEUX $e^-$ !*

## VRAIE — 2024R Ex1-Partie 1 (pile fer-zinc, 2,25 pts)

🏷️ matière=PC · année=2024 · session=R · chapitre=P24 · type=VRAIE · fidélité=reconstitué-corrigé · niveau=★★ · barème=Q1 0,5 · Q2 0,75 · Q3 1,0

> ⚠️ Énoncé **reconstitué** depuis les éléments de réponse officiels (correction provinciale Mohammedia : scribd 831498939 + bestcours 2024-07-12) — questions et barème Tier B ; formulation exacte du sujet et données $I$, $\Delta t$ non relues.
> Données (reconstituées) : pile constituée d'une électrode de fer plongeant dans $Fe^{2+}$ et d'une électrode de zinc dans $Zn^{2+}$ ; un ampèremètre indique $I > 0$, borne A du côté Fe.

**Q1.** Identifier l'électrode positive de la pile. Justifier. (0,25+0,25)
**Q2.** Écrire les demi-équations aux électrodes et l'équation bilan. (3×0,25)
**Q3.** Montrer que la masse de fer déposée vaut $\Delta m(Fe) = \frac{I\cdot\Delta t\cdot M(Fe)}{2F}$ (0,75). AN officielle : $\boxed{58\text{ mg}}$ (0,25).

**Corrigé-type :**
1. Le courant entre par la borne A → l'électrode de **Fe est le pôle $(+)$** (cathode), Zn le pôle $(-)$ (anode).
2. Anode (oxydation) : $\boxed{Zn(s) \to Zn^{2+} + 2e^-}$ ; cathode (réduction) : $\boxed{Fe^{2+} + 2e^- \to Fe(s)}$ ; bilan : $\boxed{Zn(s) + Fe^{2+} \to Zn^{2+} + Fe(s)}$.
3. $Q = I\Delta t = n(e^-)F$ avec $n(e^-) = 2x$ (2 $e^-$ par Fe déposé, cf. demi-éq) → $x = \frac{I\Delta t}{2F}$ ; $\Delta m = xM(Fe) = \boxed{\frac{I\Delta t M(Fe)}{2F}}$. AN (données du sujet) : $\boxed{58\text{ mg}}$.
🪤 *Piège testé : pôle $(+)$ = cathode = RÉDUCTION (ici Fe) — « anode $+$ » n'existe qu'en électrolyseur ! Et $n = 2$ (pas 1 !) dans $2F$.*
🗣️ الخلاصة : التيار كيدخل من A ← الحديد هو **القطب الموجب** (اختزال)! الزنك كيتأكسد (كيدوب) والحديد كيترسب! والكتلة: $Q = I\Delta t$ ← $n(e^-) = 2x$ ← $\Delta m = I\Delta t M/2F$ = **58 mg**! الـ 2 من زوج الإلكترونات — اللي نساها ضاعف النتيجة!

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $e^-$ + vers − | $e^-$ : − vers + |
| R2 | $n = 1$ | $e^-$ du bilan (2 !) |
| R3 | $n(e^-) = n(Zn)$ | $\times\nu$ ! |
