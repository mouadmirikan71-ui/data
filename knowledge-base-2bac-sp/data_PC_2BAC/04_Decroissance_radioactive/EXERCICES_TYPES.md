> **Pointer** : `04_Decroissance_radioactive` → P4 (2 type-bac : Soddy, iode 2 méthodes) + 2 VRAIES (2021N Ex3, 2023N Ex2-P1) → corrigés-types + pièges testés.
> Masse-énergie ($E_L$, fission/fusion) → `05_Noyaux_masse_energie`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Décroissance radioactive (P04)

## Méthode — décroissance en 5 gestes 🧭

1. Équation : $A$/$Z$ des 2 côtés (Soddy ; $\beta$ : $A$ fixe !).
2. $t_{1/2} \leftrightarrow \lambda = \ln2/t_{1/2}$ (unités cohérentes : s !).
3. $t = n\,t_{1/2}$ → $1/2^n$ ; sinon $e^{-\lambda t}$.
4. Restant ($1/2^n$) vs désintégré ($1-1/2^n$) : relire la question !
5. Datation : $t = -\ln(N/N_0)/\lambda$.

## R1 — TYPE-BAC (Soddy : $\alpha$, $\beta^-$, $\beta^+$)

🏷️ matière=PC · année=— · session=— · chapitre=P4 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Écrire + vérifier : a) $\alpha$ de $^{238}_{92}U$ ; b) $\beta^-$ de $^{14}_6C$ ; c) $\beta^+$ de $^{22}_{11}Na$.

**Corrigé-type.** a) $^{238}_{92}U \to ^{234}_{90}Th + ^4_2He$ ($234+4 = 238$ ✓, $90+2 = 92$ ✓). b) $^{14}_6C \to ^{14}_7N + ^0_{-1}e$ ($A$ fixe ✓, $6+1 = 7$ ✓). c) $^{22}_{11}Na \to ^{22}_{10}Ne + ^0_{+1}e$ ($A$ fixe ✓, $11-1 = 10$ ✓).
🪤 *Piège testé : c) $^{22}_{12}Na$ (« $\beta$ = +1 toujours ») — $\beta^+$ : $p \to n$ : $Z-1$ ! Le signe de $\beta$ donne le sens.*

## R2 — TYPE-BAC ($^{131}I$ médical : 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P4 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $^{131}I$ : $t_{1/2} = 8{,}0$ j, $A_0 = 800$ MBq. a) $A$ après 24 j ? b) Au bout de combien de temps $A < 1$ MBq ?

**Corrigé-type — Méthode 1 (demi-vies entières).** a) $24/8 = 3$ demi-vies → $A = 800/2^3 = \boxed{100\text{ MBq}}$. b) $800/2^n < 1$ → $2^n > 800$ → $n = 10$ ($2^{10} = 1024$) → $\boxed{t = 80\text{ j}}$ (10 demi-vies).

**Corrigé-type — Méthode 2 (loi exacte).** $\lambda = \ln2/8 = 0{,}0866$ j$^{-1}$ ; $A = A_0e^{-\lambda t} = 1$ → $t = -\ln(1/800)/0{,}0866 = 6{,}685/0{,}0866 = \boxed{77{,}2\text{ j}}$. Même verdict que M1 ($80$ j en demi-vies entières — M2 affine à $77$ j).
🪤 *Piège testé : a) $800\times(1-3/8)$ ou règle de trois — la décroissance est EXPONENTIELLE : $1/2^n$, jamais linéaire !*

## VRAIE — 2021N Ex3 ($^{238}Pu$ : 88 ans)

🏷️ matière=PC · année=2021 · session=N · chapitre=P4 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

$^{238}_{94}Pu \to ^{234}_{92}U + ^4_2He$ (Soddy). $a_0 = 10^{11}$ Bq → $a(t_{1/2}) = 5\times10^{10}$ → lecture : $t_{1/2} = 88$ ans. $\lambda = \ln2/88 = 7{,}88\times10^{-3}$ an⁻¹. $N_0 = a_0/\lambda = 10^{11}/(7{,}88\times10^{-3}/(365\times24\times3600)) = 4\times10^{20}$. $t_{max}$ ($N = 0{,}7N_0$) : $t = -\ln0{,}7/\lambda = 45{,}3$ ans.
🪤 *vraie : $\lambda$ en s⁻¹ pour $N_0$ (convertir les ans !) ; lecture $t_{1/2}$ sur $a(t)$ (pas $N$ !).*

## VRAIE — 2023N Ex2-P1 (QCM + tritium $\beta^-$ + démo $t_{1/2}$)

🏷️ matière=PC · année=2023 · session=N · chapitre=P4 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé

QCM : C FAUX : à $t = 2t_{1/2}$ il RESTE 25 % → DÉSINTÉGRÉ = 75 % (pas 25 % !). Tritium : $^3_1H \xrightarrow{\beta^-} ^3_2He + ^0_{-1}e$ ($A$ fixe, $Z$ : $1+1 = 2$). Démo $t_{1/2} = \ln2/\lambda$ ($N_0/2 = N_0e^{-\lambda t}$ → $\ln$).
🪤 *vraie : « désintégré » = $1-1/2^n$ (restant = $1/2^n$ !) ; $\beta^-$ : $A$ inchangé.*

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | $\beta^+$ : $Z+1$ | signe de $\beta$ = sens de $Z$ |
| R2 | décroissance linéaire | $1/2^n$ ! (M2 : $e^{-\lambda t}$) |
| 2021N | $\lambda$ en an⁻¹ pour $N_0$ | $\lambda$ en s⁻¹ (Bq = s⁻¹ !) |
| 2023N | désintégré = 25 % | désintégré = $1-1/2^n$ = 75 % |
