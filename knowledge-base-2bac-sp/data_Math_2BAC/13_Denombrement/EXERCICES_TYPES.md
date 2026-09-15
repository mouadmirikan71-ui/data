> **Pointer** : `13_Denombrement` → P4 (4 type-bac : urne, comité, Newton, codes) → corrigés-types + R2 en 2 méthodes.

# Exercices types — Dénombrement (M13)

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

## Méthode — compter en 5 gestes 🧭

1. Souligner simultané/successif/remise.
2. **Test d'échange** (ordre ?) + répétition ? → case ($A$, $C$, $n^p$, $n!$).
3. « Au moins/au plus » → **complémentaire** ?
4. Écrire la formule AVANT les nombres.
5. Calculer en **simplifiant** ($n!$) ; valider sur mini-cas si doute.

## R1 — TYPE-BAC (l'urne canon : 3B+3V+4R, tirage simultané de 3)

🏷️ matière=Math · année=— · session=— · chapitre=M13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** Urne : 3 blanches, 3 vertes, 4 rouges (indiscernables). On tire 3 boules simultanément. Dénombrer : a) tous les tirages ; b) 0 rouge ; c) 3B ou 3V ; d) exactement 1 rouge ; e) au moins 2 rouges.

**Corrigé-type.** Simultané → $C$ partout. a) $\boxed{C_{10}^3 = 120}$. b) 3 parmi les 6 non-rouges : $\boxed{C_6^3 = 20}$. c) $C_3^3 + C_3^3 = \boxed{2}$ (disjoints : $+$). d) $C_4^1 \times C_6^2 = 4 \times 15 = \boxed{60}$ (1 rouge ET 2 autres : $\times$). e) (2R,1NR) ou (3R) : $C_4^2C_6^1 + C_4^3 = 36 + 4 = \boxed{40}$.
🪤 *Piège testé : d) $C_4^1 + C_6^2$ (additionner au lieu de multiplier) — « 1 rouge ET 2 autres » = 2 cases successives = $\times$.*

## R2 — TYPE-BAC (comité « au moins 1 femme », 2 méthodes !)

**Énoncé.** Comité de 4 parmi 6 hommes et 4 femmes. Combien de comités avec au moins 1 femme ?

**Corrigé-type — Méthode 1 (direct).** 1F : $C_4^1C_6^3 = 80$ ; 2F : $C_4^2C_6^2 = 90$ ; 3F : $C_4^3C_6^1 = 24$ ; 4F : $C_4^4 = 1$. Total : $80+90+24+1 = \boxed{195}$.

**Corrigé-type — Méthode 2 (complémentaire).** Total $-$ « 0 femme » : $C_{10}^4 - C_6^4 = 210 - 15 = \boxed{195}$. Même résultat, 2 opérations.
🪤 *Piège testé : $C_4^1 \times C_9^3$ (« choisir LA femme puis compléter ») $= 336$ — FAUX : chaque comité à $k$ femmes compté $k$ fois (double compte !).*

## R3 — TYPE-BAC (Newton : développer + extraire)

🏷️ matière=Math · année=— · session=— · chapitre=M13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** a) Développer $(x+2)^3$. b) Coefficient de $x^2$ dans $(x-1)^5$ ?

**Corrigé-type.** a) $\sum C_3^k x^{3-k}2^k = x^3 + 3\cdot2x^2 + 3\cdot4x + 8 = \boxed{x^3+6x^2+12x+8}$. b) $(x+(-1))^5$ : terme en $x^2$ : $C_5^3x^2(-1)^3 = 10x^2(-1)$ → $\boxed{-10}$.
🪤 *Piège testé : a) $x^3+6x^2+4x+8$ (oublier $2^2 = 4$ dans $C_3^2\times4$) — Newton : les DEUX bases portent des puissances.*

## R4 — TYPE-BAC ($A$ vs $n^p$ : podium et codes)

🏷️ matière=Math · année=— · session=— · chapitre=M13 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=voir énoncé

**Énoncé.** a) Podium (or, argent, bronze) parmi 8 athlètes : combien d'arrivées ? b) Codes à 4 chiffres (répétitions autorisées) : combien ?

**Corrigé-type.** a) Ordre + sans répétition → $\boxed{A_8^3 = 8\times7\times6 = 336}$. b) Ordre + répétition → $\boxed{10^4 = 10000}$ (p-liste).
🪤 *Piège testé : b) $A_{10}^4 = 5040$ — « code » seul n'interdit PAS les répétitions ( Tashkent 7777 existe !) : sans « chiffres distincts », c'est $n^p$.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $+$ au lieu de $\times$ (cases successives) | ET = $\times$, OU = $+$ |
| R2 | $C_4^1\times C_9^3$ (double compte) | au moins = total $-$ aucun |
| R3 | $2^k$ oublié dans Newton | $a^{n-k}b^k$ : 2 puissances |
| R4 | code sans remise imposée | « distincts » absent → $n^p$ |
