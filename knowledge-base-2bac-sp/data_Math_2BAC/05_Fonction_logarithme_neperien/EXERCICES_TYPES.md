> **Pointer** : `05_Fonction_logarithme_neperien` → P4 (3 vraies 2020R+2020N + 3 type-bac) → corrigés-types recoupés + R1 en 2 méthodes.

# Exercices types — Logarithme népérien (M05)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Données 2020R + 2020N (énoncés réels SP)

**2020R Problème** : $g(x) = e^{1-x} + 1/x - 2$ ; $f(x) = (1-x)e^{1-x} - x^2 + 5x - 3 - 2\ln x$ sur $]0, +\infty[$. **2020N Ex.3** : $g(x) = 2\sqrt{x} - 2 - \ln x$ sur $]0, +\infty[$. Sources : etude-generale (2020R rattrapage + 2020N normale, SP) ; corrections Problème/Ex.3 non publiées sur-page → corrigés-types prof recoupés par calcul.

## Q1 — VRAIE (2020 R, Problème partie I)

🏷️ matière=Math · année=2020 · session=R · chapitre=M5 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « Montrer que $g'(x) < 0$ sur $]0, +\infty[$ » ; « Signe de $g$ ($g(1) = 0$) ».

**Corrigé-type.** $g'(x) = -e^{1-x} - 1/x^2 < 0$ (somme de négatifs) → $g$ strictement décroissante ; $g(1) = 0$ → $\boxed{g > 0\text{ sur }]0,1[}$, $\boxed{g < 0\text{ sur }]1,+\infty[}$.
🪤 *Piège testé : chercher un piège dans $g'$ — $e^{(\dots)} > 0$ toujours : $-e^{(\dots)} < 0$ toujours. Évident = réponse.*

## Q2 — VRAIE (2020 R, Problème partie II)

🏷️ matière=Math · année=2020 · session=R · chapitre=M5 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « $\lim_{0^+} f = +\infty$ + interpréter » ; « $\lim_{+\infty} f = -\infty$ » ; « $\lim_{+\infty} f/x = -\infty$ + interpréter » ; « $f'(x) = (x-2)g(x)$ » ; « variations ».

**Corrigé-type.** **Limites** : $0^+$ → $e - 3 + \infty = \boxed{+\infty}$ (**AV** $x = 0$) ; $+\infty$ → $0 - \infty - \infty = \boxed{-\infty}$ ; $f/x \to -x \to \boxed{-\infty}$ (**branche parabolique** $(Oy)$). **Dérivée** : $[(1-x)e^{1-x}]' = (x-2)e^{1-x}$ ; $(-x^2+5x-3-2\ln x)' = -2x+5-2/x$ ; $(x-2)g = (x-2)e^{1-x} - 2x+5-2/x$ ✓ → $\boxed{f' = (x-2)g}$. **Variations** (signe $(x-2)g$, Q1) : $\boxed{\text{↓ }]0,1]\text{, ↑ }[1,2]\text{, ↓ }[2,+\infty[}$.
🪤 *Piège testé : $f/x$ via L'Hôpital — diviser terme à terme ($-x^2/x = -x$ suffit).*

## Q3 — VRAIE (2020 N, Ex.3 Q1a–Q1d : $\ln$ par encadrement)

🏷️ matière=Math · année=2020 · session=N · chapitre=M5 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « $g'(x) = (\sqrt{x}-1)/x$ » ; « $g$ croissante sur $[1,+\infty[$ » ; « $0 \leq \ln x \leq 2\sqrt{x}$ sur $[1,+\infty[$ » ; « $0 \leq (\ln x)^3/x^2 \leq 8/\sqrt{x}$ + $\lim_{+\infty} = 0$ ».

**Corrigé-type.** $g' = 1/\sqrt{x} - 1/x = \boxed{(\sqrt{x}-1)/x} \geq 0$ sur $[1,+\infty[$ → $g$ croissante ; $g(1) = 0$ → $g \geq 0$ → $\ln x \leq 2\sqrt{x} - 2 \leq 2\sqrt{x}$ (et $\ln x \geq 0$ sur $[1,+\infty[$) → $\boxed{0 \leq \ln x \leq 2\sqrt{x}}$. Au cube ($\uparrow$) : $0 \leq (\ln x)^3 \leq 8x^{3/2}$ → $/x^2$ : $\boxed{0 \leq (\ln x)^3/x^2 \leq 8/\sqrt{x}} \to 0$ (gendarme) → $\boxed{\lim = 0}$ (CC par encadrement !).
🪤 *Piège testé : passer au cube sans vérifier la positivité — ici OK ($\geq 0$), mais le réflexe « signe d'abord » est vital.*

## R1 — TYPE-BAC (la classique $(\ln x)/x$, 2 méthodes !)

**Énoncé.** $f(x) = (\ln x)/x$ sur $]0, +\infty[$. a) Limites. b) Dérivée, variations, extremum.

**Corrigé-type.** a) $0^+$ → $-\infty$ ; $+\infty$ : **M1 (CC)** $\to 0^+$ ; **M2 ($X = \ln x$)** : $X/e^X \to 0^+$ (miroir $\exp$). b) $f' = (1-\ln x)/x^2$ → ↑ $]0,e]$, ↓ $[e,+\infty[$, **max** $\boxed{1/e}$.
🪤 *Piège testé : $\lim_{+\infty} = +\infty$ — CC : le dénominateur gagne.*

## R2 — TYPE-BAC (équation : le domaine tranche)

🏷️ matière=Math · année=— · session=— · chapitre=M5 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Résoudre : $\ln(2x+1) + \ln(x-1) = \ln 7$.

**Corrigé-type.** Domaine $x > 1$ → $(2x+1)(x-1) = 7$ → $x = \frac{1\pm\sqrt{65}}{4}$, négative rejetée → $\boxed{S = \{\frac{1+\sqrt{65}}{4}\}}$ (contrôle : $\frac{65-9}{8} = 7$ ✓).
🪤 *Piège testé : garder les deux racines — une toujours hors domaine.*

## R3 — TYPE-BAC (pont M04/M09 : $\int_1^e (\ln x)/x\,dx$)

🏷️ matière=Math · année=— · session=— · chapitre=M5 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Calculer $I = \int_1^e \frac{\ln x}{x}\,dx$ (M04-R4).

**Corrigé-type.** $F = (\ln x)^2/2$ → $I = \boxed{1/2}$.
🪤 *Piège testé : $\ln(\ln x)$ (« faux $u'/u$ ») — c'est $u'u \to u^2/2$.*

## R4 — ENTRAÎNEMENT (log décimal + pH, pont PC)

🏷️ matière=Math · année=— · session=— · chapitre=M5 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=★ · barème=—

**Énoncé.** On donne $\log 2 \approx 0,30$. (a) Calculer $\log(2\times 10^{-3})$. (b) Une solution a $[H_3O^+] = 2\times 10^{-3}$ mol/L : son pH ? (c) Résoudre $\log x = -2$.
**Corrigé :** (a) $\log(2\times 10^{-3}) = \log 2 + \log 10^{-3} = \boxed{0,30 - 3 = -2,70}$. (b) pH $= -\log[H_3O^+] = \boxed{2,70}$ (acide !). (c) $x > 0$ et $x = 10^{-2} = \boxed{0,01}$ ✓ (domaine OK).
> بالدارجة: $10^{-3}$ كتخرج من الـ log بـ $-3$! $\log(2\times 10^{-3}) = 0,30-3 = -2,70$! والـ pH = ناقص الـ log ← $2,70$ (حمضي)! والمعادلة: $\log x = -2$ ← $x = 10^{-2}$ (موجب ✓)!

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| Q1 | $g'$ cru compliqué | $-e^{(\dots)} - 1/x^2 < 0$ évident |
| Q2 | $f/x$ via L'Hôpital | terme à terme : $-x$ domine |
| Q3 | cube sans signe | positivité d'abord, gendarme ensuite |
| R1 | $\lim_{+\infty}(\ln x)/x = +\infty$ | CC : $\ln$ perd → $0$ |
| R2 | racine hors domaine gardée | domaine AVANT, rejet APRÈS |
| R3 | $\ln(\ln x)$ | $u'u \to u^2/2$ |
| R4 | $\log(2\times 10^{-3}) = \log 2 \times (-3)$ | somme : $\log 2 + (-3)$ ; pH = $-\log$ (le $-$ !) |

## VRAIE — 2023N Problème-Q1 ($f = 2-2/x+(1-\ln x)^2$ : le $t=\sqrt{x}$ !)

🏷️ matière=Math · année=2023 · session=N · chapitre=M5 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
$\lim_{x\to0^+}x(\ln x)^2 = 0$ : poser $t = \sqrt{x}$ ($x = t^2$) → $\lim_{t\to0^+}(2t\ln t)^2 = 0$ (car $t\ln t \to 0$). $\lim_{x\to+\infty}(\ln x)^2/x = 0$ (croissances comparées : $\ln \ll x$ !). Forme unique : $f(x) = (3x-2-2x\ln x+x(\ln x)^2)/x$.
🪤 *vraie : $(\ln x)^2$ en $0^+$ → $t = \sqrt{x}$ (ramener à $t\ln t$ !) ; en $+\infty$ → comparées direct.*
