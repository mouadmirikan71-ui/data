> **Pointer** : `10_Equations_differentielles` → P4 (4 type-bac : ordre 1, équilibre, ordre 2, pont PC) → corrigés-types + R1 en 2 méthodes.

# Exercices types — Équations différentielles (M10)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Méthode — les 3 pas 🧭

1. **Normaliser** : mettre sous forme $y' + ay = \dots$ (ou $y'' + \omega^2 y = 0$) et lire $a$/$\omega$ **avec le signe**.
2. **Formule** : $Ce^{-ax}$ (+ $b/a$ si second membre) ou $A\cos\omega x + B\sin\omega x$.
3. **CI puis VÉRIFIER** : déterminer $C$ (ou $A, B$), redériver, réinjecter dans l'équation.

## R1 — TYPE-BAC (ordre 1, 2 méthodes !)

**Énoncé.** Résoudre sur $\mathbb{R}$ : $y' + 2y = 0$ avec $y(0) = 3$.

**Corrigé-type — Méthode 1 (formule).** Type 1, $a = 2$ → $y = Ce^{-2x}$. CI : $y(0) = C = 3$ → $\boxed{y = 3e^{-2x}}$. Vérification : $y' = -6e^{-2x}$ ; $y' + 2y = -6e^{-2x} + 6e^{-2x} = 0$ ✓ et $y(0) = 3$ ✓.

**Corrigé-type — Méthode 2 (deviner + unicité).** On devine (lien M07 : $(e^{-2x})' = -2e^{-2x}$) que $3e^{-2x}$ est solution : $y' + 2y = 0$ ✓, $y(0) = 3$ ✓. Par unicité admise (une CI = une seule solution), c'est **la** solution : $\boxed{y = 3e^{-2x}}$.
🪤 *Piège testé : $a = -2$ (« $y' = -2y$ donc $a = -2$ ») — non, la forme $y' + 2y = 0$ donne $a = +2$.*

## R2 — TYPE-BAC (avec second membre : l'équilibre)

🏷️ matière=Math · année=— · session=— · chapitre=M10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Résoudre sur $\mathbb{R}$ : $y' - 3y = 6$ avec $y(0) = 1$.

**Corrigé-type.** Forme $y' + ay = b$ avec $a = -3$, $b = 6$. Équilibre : $y_p = b/a = 6/(-3) = -2$. Général : $y = Ce^{-(-3)x} - 2 = Ce^{3x} - 2$. CI : $C - 2 = 1$ → $C = 3$ → $\boxed{y = 3e^{3x} - 2}$. Vérification : $y' = 9e^{3x}$ ; $y' - 3y = 9e^{3x} - 9e^{3x} + 6 = 6$ ✓.
🪤 *Piège testé : $e^{-3x}$ au lieu de $e^{+3x}$ — $a = -3$ donc $-ax = +3x$. Normaliser d'abord, toujours.*

## R3 — TYPE-BAC (ordre 2 : l'oscillateur)

🏷️ matière=Math · année=— · session=— · chapitre=M10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Résoudre sur $\mathbb{R}$ : $y'' + 4y = 0$ avec $y(0) = 1$ et $y'(0) = 0$.

**Corrigé-type.** $\omega^2 = 4$ → $\omega = 2$ → $y = A\cos 2x + B\sin 2x$ ; $y' = -2A\sin 2x + 2B\cos 2x$. CI : $y(0) = A = 1$ ; $y'(0) = 2B = 0$ → $B = 0$. Donc $\boxed{y = \cos 2x}$. Vérification : $y'' = -4\cos 2x$ ; $y'' + 4y = 0$ ✓.
🪤 *Piège testé : $\omega = 4$ (« je recopie le 4 ») — non, $\omega = \sqrt{4} = 2$. L'équation porte $\omega^2$, la solution porte $\omega$.*

## R4 — TYPE-BAC (pont PC : la radioactivité)

🏷️ matière=Math · année=— · session=— · chapitre=M10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé (lien P04).** Le nombre $N(t)$ de noyaux radioactifs vérifie $N' = -\lambda N$ ($\lambda > 0$) avec $N(0) = N_0$. a) Exprimer $N(t)$. b) Exprimer la demi-vie $t_{1/2}$ (instant où $N = N_0/2$) en fonction de $\lambda$.

**Corrigé-type.** a) $N' + \lambda N = 0$, $a = \lambda$ → $N = Ce^{-\lambda t}$ ; $N(0) = C = N_0$ → $\boxed{N(t) = N_0 e^{-\lambda t}}$. b) $N_0 e^{-\lambda t_{1/2}} = N_0/2$ → $e^{-\lambda t_{1/2}} = 1/2$ → $-\lambda t_{1/2} = -\ln 2$ → $\boxed{t_{1/2} = \ln 2 / \lambda}$.
🪤 *Piège testé : résoudre $e^{-\lambda t} = 1/2$ « à la calculatrice » — non, passer au $\ln$ (M05) : $-\lambda t = \ln(1/2) = -\ln 2$.*

## R5 — ENTRAÎNEMENT (ordre 2 : 2 CI non nulles + période)

🏷️ matière=Math · année=— · session=— · chapitre=M10 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★★ · barème=—

**Énoncé.** Résoudre $y'' + 9y = 0$ avec $y(0) = 2$ et $y'(0) = 3$. Donner la période $T$ des solutions.
**Corrigé-type.** $\omega^2 = 9$ → $\omega = 3$ → $y = A\cos 3x + B\sin 3x$ ; $y' = -3A\sin 3x + 3B\cos 3x$. CI : $A = 2$ ; $3B = 3$ → $B = 1$. Donc $\boxed{y = 2\cos 3x + \sin 3x}$, de période $\boxed{T = 2\pi/3}$. Vérification : $y'' = -18\cos 3x - 9\sin 3x = -9y$ ✓.
> بالدارجة: $\omega^2 = 9$ ← $\omega = 3$ (**الجذر** ماشي 9)! $A = 2$ من $y(0)$ و$B = 1$ من $y'(0) = 3B$! والدور $T = 2\pi/\omega = 2\pi/3$! والتحقق إجباري: اشتق جوج مرات وعوض!

> ⚠️ ED : **aucune VRAIE identifiée** (Ex standalone disparu ~2016, Tier A 2020–2026 : 0 occurrence). R1–R5 = entraînement pur (pont PC : RC/RL/radioactivité/oscillateurs).

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | signe de $a$ | normaliser : $y' + 2y = 0$ → $a = +2$ |
| R2 | exposant $-3x$ vs $+3x$ | $a = -3$ → $-ax = +3x$ |
| R3 | $\omega = 4$ | $\omega = \sqrt{4} = 2$ |
| R4 | $e^{-\lambda t} = 1/2$ bloqué | appliquer $\ln$ des deux côtés |
| R5 | $B$ depuis $y(0)$ (c'est $A$ !) ; $T = 2\pi\times 3$ | $B$ vient de $y'(0) = 3B$ ; $T = 2\pi/\omega$ (diviser !) |
