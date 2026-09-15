> **Pointer** : `04_Fonctions_primitives` → P4 (1 vraie 2020N Ex.3-2 + 4 type-bac) → corrigés-types + R2 en 2 méthodes.

# Exercices types — Primitives (M04)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Méthode — primitiver en 4 gestes 🧭

1. **Repérer** : usuelle directe ? forme $u$ ($u'u^n$, $u'/u$, $u'e^u$) ? primitive à VÉRIFIER (dériver !) ?
2. **Identifier $u$ et $u'$** : $u'$ présent → formule ; $u' = $ constante $a$ → compenser $\times 1/a$.
3. **$+C$ obligatoire** (sauf condition imposée → $C$ unique).
4. **VÉRIFIER en dérivant** : retrouver $f$ (chasse les erreurs de coefficients).

## Q1 — VRAIE (2020 N, Ex.3 Q2a+Q2b)

🏷️ matière=Math · année=2020 · session=N · chapitre=M4 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « Montrer que $G(x) = x(-1 + \frac{4}{3}\sqrt{x} - \ln x)$ est une primitive de $g(x) = 2\sqrt{x} - 2 - \ln x$ sur $]0, +\infty[$ » ; « Calculer $\int_1^4 g(x)\,dx$ ».

**Corrigé-type.** $G(x) = -x + \frac{4}{3}x^{3/2} - x\ln x$ → $G'(x) = -1 + \frac{4}{3}\cdot\frac{3}{2}\sqrt{x} - (\ln x + 1) = -1 + 2\sqrt{x} - \ln x - 1 = \boxed{g(x)}$ ✓. Donc $\int_1^4 g = G(4) - G(1) = 4(-1+\frac{8}{3}-\ln 4) - (-1+\frac{4}{3}) = \frac{20}{3} - 4\ln 4 - \frac{1}{3} = \boxed{\frac{19}{3} - 8\ln 2}$ (≈ $0,79 > 0$ ✓ cohérent : $g \geq 0$ sur $[1,4]$, voir M05-Q3).
🪤 *Piège testé : dériver $x\ln x$ en $\ln x$ (oublier le $+1$ du produit : $(x\ln x)' = \ln x + 1$) — $G' \neq g$ et tout s'écroule.*

## R1 — TYPE-BAC (l'arsenal usuelles)

🏷️ matière=Math · année=— · session=— · chapitre=M4 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Déterminer une primitive sur l'intervalle indiqué : a) $f(x) = 3x^2 - 2x + 5$ sur $\mathbb{R}$ ; b) $f(x) = (2x+1)^3$ sur $\mathbb{R}$ ; c) $f(x) = e^{3x+1}$ sur $\mathbb{R}$ ; d) $f(x) = 1/(2x+1)$ sur $]-1/2, +\infty[$.

**Corrigé-type.** a) $\boxed{x^3 - x^2 + 5x + C}$. b) $u = 2x+1$, $u' = 2$ → $\boxed{(2x+1)^4/8 + C}$. c) $\boxed{e^{3x+1}/3 + C}$. d) $\boxed{\frac{1}{2}\ln(2x+1) + C}$. Vérifications par dérivation ✓ (voir méthode).
🪤 *Piège testé : $1/u' = 1/2$ oublié en b) et d) — intérieur affine → on divise par $a$.*

## R2 — TYPE-BAC (primitive de $(x+1)e^x$, 2 méthodes !)

**Énoncé.** Déterminer les primitives sur $\mathbb{R}$ de $f(x) = (x+1)e^x$.

**Corrigé-type — Méthode 1 (deviner + identifier).** $F = (ax+b)e^x$ → $F' = (ax+a+b)e^x = (x+1)e^x$ → $a = 1$, $b = 0$ → $\boxed{xe^x + C}$. Contrôle : $(xe^x)' = (x+1)e^x$ ✓.

**Corrigé-type — Méthode 2 (IPP, outil M09).** $u = x+1$, $v' = e^x$ → $(x+1)e^x - \int e^x = \boxed{xe^x + C}$.
🪤 *Piège testé : primitiver le produit facteur par facteur — FAUX, le produit ne se primitive pas en morceaux !*

## R3 — TYPE-BAC (primitive + condition : $C$ unique)

🏷️ matière=Math · année=— · session=— · chapitre=M4 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Déterminer LA primitive $F$ de $f(x) = 2x/(x^2+1)$ sur $\mathbb{R}$ vérifiant $F(0) = 0$.

**Corrigé-type.** $u = x^2+1$, $u' = 2x$ → $F = \ln(x^2+1) + C$ ; $F(0) = C = 0$ → $\boxed{\ln(x^2+1)}$.
🪤 *Piège testé : garder $+C$ malgré la condition — une condition = $C$ déterminée.*

## R4 — TYPE-BAC (pont M05 : primitive de $\frac{\ln x}{x}$)

🏷️ matière=Math · année=— · session=— · chapitre=M4 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Déterminer les primitives sur $]0, +\infty[$ de $f(x) = (\ln x)/x$.

**Corrigé-type.** $u = \ln x$, $u' = 1/x$ → $f = u'u$ → $\boxed{(\ln x)^2/2 + C}$ (application : $\int_1^e = 1/2$, voir M05-R3).
🪤 *Piège testé : $u = x$ au lieu de $u = \ln x$ — demander « qui est $u$ ? qui est $u'$ ? ».*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| Q1 | $(x\ln x)' = \ln x$ | produit : $\ln x + 1$ ! |
| R1 | $1/u'$ oublié (intérieur affine) | diviser par $a$ |
| R2 | produit primitivé en morceaux | deviner $(ax+b)e^x$ ou IPP |
| R3 | $+C$ gardé malgré $F(0) = 0$ | condition → $C$ unique |
| R4 | $u$ mal choisi | $u = \ln x$, vérifier en dérivant |
