> **Pointer** : `14_Probabilites` → P4 (1 vraie 2025N Ex.3 + 4 type-bac) → corrigés-types + R2 en 2 méthodes.

# Exercices types — Probabilités (M14)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Données 2025N (Ex.3, 2.5 pts — urne + binomiale)

Urne : 4 blanches $(0,1,1,1)$ + 2 noires $(0,1)$. Tirage simultané de 2 boules. $A$ : « deux numéros 1 » ; $B$ : « même couleur ». Répétition $3\times$ : $X$ = nombre de réalisations de $A$. Source : etude-generale (2025 Normale SP, énoncés réels ; corrigés-types prof recoupés).

## Q1 — VRAIE (2025 N, Ex.3 Q1+Q2)

🏷️ matière=Math · année=2025 · session=N · chapitre=M14 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

**Énoncés :** « $P(A) = ?$, $P(B) = 7/15$, $A$ et $B$ indépendants ? » ; « $X$ : loi ($P(X=0) = 27/125$ donné) + $E(X)$ ».

**Corrigé-type.** $card\Omega = C_6^2 = 15$. Quatre boules portent « 1 » → $cardA = C_4^2 = 6$ → $\boxed{P(A) = 6/15 = 2/5}$ (⚠️ page : « 2/15 » — coquille confirmée : $2/15$ exigerait $cardA = 2$, et $P(X=0) = 27/125 = (3/5)^3$ impose $p = 2/5$ ✓). $cardB = C_4^2+C_2^2 = 7$ → $\boxed{P(B) = 7/15}$ ✓. $A\cap B$ : deux « 1 » même couleur : $C_3^2 + C_1^2 = 3+0 = 3$ → $P = 3/15 = 1/5 \neq (2/5)(7/15) = 14/75$ → $\boxed{\text{NON indépendants}}$. $X \sim B(3, 2/5)$ (répétitions i.i.d.) : $P(X=0) = 27/125$ ✓, $P(X=1) = 3(2/5)(3/5)^2 = 54/125$, $P(X=2) = 36/125$, $P(X=3) = 8/125$ (somme $125/125$ ✓) ; $E(X) = 3\times2/5 = \boxed{6/5}$.
🪤 *Piège testé : $A\cap B = A$ (« deux 1 » toujours même couleur ? NON : 3 blancs + 1 noir portent 1 → tirage mixte possible) — dénombrer, pas deviner.*

## R1 — TYPE-BAC (l'urne : mêmes comptes, quotient !)

🏷️ matière=Math · année=— · session=— · chapitre=M14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Urne M13-R1 (3B+3V+4R, 3 simultanées) : $p(0R)$, $p(3B$ ou $3V)$, $p(1R$ exact$)$, $p(\geq2R)$ ?

**Corrigé-type.** $card\Omega = 120$ : $\boxed{1/6}$, $\boxed{1/60}$, $\boxed{1/2}$, $\boxed{1/3}$ (comptes M13-R1).
🪤 *Piège testé : modèles mixtes haut/bas — tout $C$ ou tout $A$.*

## R2 — TYPE-BAC (conditionnelle : zoom, 2 méthodes !)

**Énoncé.** 18 filles, 12 garçons ; lunettes : 10F, 4G. $p(\text{fille} \mid \text{lunettes})$ ?

**Corrigé-type — M1 (restriction).** $\Omega' = 14$ porteurs, 10 filles → $\boxed{5/7}$. **M2 (formule).** $(10/30)/(14/30) = \boxed{5/7}$.
🪤 *Piège testé : $10/30$ — « sachant » : diviser par $p(A)$.*

## R3 — TYPE-BAC (arbre + totales : l'usine)

🏷️ matière=Math · année=— · session=— · chapitre=M14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** M1 : 60 %, 2 % défauts ; M2 : 40 %, 5 % défauts. $p(D)$ ?

**Corrigé-type.** $0,6\times0,02+0,4\times0,05 = \boxed{0,032}$ (produit/chemin, somme/chemins).
🪤 *Piège testé : moyenne $0,035$ — pondérer par la production !*

## R4 — TYPE-BAC (binomiale : pièce $5\times$)

🏷️ matière=Math · année=— · session=— · chapitre=M14 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** $X$ = Piles sur 5 lancers. a) Loi ? b) $p(X=3)$ ? c) $p(X\geq1)$ ? d) $E(X)$ ?

**Corrigé-type.** a) $\boxed{B(5,1/2)}$. b) $\boxed{5/16}$. c) $1-(1/2)^5 = \boxed{31/32}$. d) $\boxed{2,5}$.
🪤 *Piège testé : $p(X\geq1) = p(X=1)$ — complémentaire $1-p(X=0)$ !*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| Q1 | $A\cap B = A$ | dénombrer : $C_3^2+C_1^2 = 3$ |
| R1 | modèles mixtes | tout $C$ ou tout $A$ |
| R2 | $10/30$ | sachant = zoom |
| R3 | moyenne $0,035$ | pondérer |
| R4 | $p(X\geq1) = p(X=1)$ | $1-p(X=0)$ |

## VRAIE — 2023N Ex3 (2 urnes + transfert : $X = ab$)

🏷️ matière=Math · année=2023 · session=N · chapitre=M14 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
$U_1$ : 2×0, 3×1, 1×2 ; $U_2$ : 3×1, 2×2 ; on tire $a$ ($U_1$), on l'ajoute à $U_2$, on tire $b$. $P(A) = 3/6 = 1/2$ ($a=1$). $P(B) = (3/6)(2/6)+(1/6)(3/6) = 9/36 = 1/4$ ($ab=2$ : $1\times2$ ou $2\times1$ !). $P(A|B) = (1/6)/(1/4) = 2/3$. Loi de $X=ab$ : $P(0)=1/3$, $P(1)=(3/6)(4/6)=1/3$, $P(2)=1/4$, $P(4)=(1/6)(3/6)=1/12$ (somme $=1$ ✓). $N$ (pair non nul) : $1/4+1/12 = 1/3 = P(M)$ → équiprobables.
🪤 *vraie : $U_2$ change selon $a$ (conditionner !) ; $ab=2$ = 2 cas ($1\times2$ ET $2\times1$).*
