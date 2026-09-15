> **Pointer** : `09_Transmission_information_modulation_demodulation` → P4 (4 type-bac : Shannon, dB, fibre, débit) → corrigés-types + R2 en 2 méthodes.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Transmission d'informations (P09)

## Méthode — transmission en 5 gestes 🧭

1. Identifier : émetteur / canal / récepteur.
2. Numérique : Shannon $f_e \geq 2f_{max}$.
3. dB : $\times10$/$+10$, $\times2$/$+3$ — décomposer !
4. Fibre : $\sin i_c = n_2/n_1$ ($n_1 > n_2$).
5. Débit : bits ÷ bit/s — BIT vs OCTET d'abord !

## R1 — TYPE-BAC (Shannon : téléphone + CD)

🏷️ matière=PC · année=— · session=— · chapitre=P9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** a) Voix téléphonique $f_{max} = 4$ kHz : $f_e$ min ? b) CD : $f_e = 44,1$ kHz, 16 bits, stéréo : débit ? c) Fichier 3 min mono 8 kHz 8 bits : taille ?

**Corrigé-type.** a) $f_e \geq 2\times4 = \boxed{8\text{ kHz}}$. b) $D = 44100\times16\times2 = \boxed{1,41\text{ Mbit/s}}$. c) $180\times8000\times8 = 1,15\times10^7$ bits $= \boxed{1,44\text{ Mo}}$.
🪤 *Piège testé : c) « 11,5 Mo » (bits lus comme octets) — ÷8 : 1 bit n'est pas 1 octet !*

## R2 — TYPE-BAC (atténuation, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** $P_e = 50$ mW, $P_s = 0,50$ mW. a) $A$ en dB ? b) Longueur de fibre équivalente ($0,20$ dB/km) ?

**Corrigé-type.** a) **Méthode 1 (formule)** : $A = 10\log(50/0,5) = 10\log 100 = \boxed{20\text{ dB}}$. **Méthode 2 (décomposition)** : $\times100 = \times10\times10$ → $+10+10 = \boxed{20\text{ dB}}$, sans calculatrice ! b) $L = 20/0,20 = \boxed{100\text{ km}}$ (un relais !).
🪤 *Piège testé : $A = 10\times(50/0,5) = 1000$ dB (log oublié !) — dB = TOUJOURS un log.*

## R3 — TYPE-BAC (fibre : $i_c$ + 2 rayons)

🏷️ matière=PC · année=— · session=— · chapitre=P9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Fibre $n_1 = 1,48$, $n_2 = 1,46$. a) $i_c$ ? b) Rayon $i = 75°$ : sort ou piégé ($r$ ?) ? c) $i = 85°$ ?

**Corrigé-type.** a) $\sin i_c = 1,46/1,48 = 0,9865$ → $\boxed{i_c = 80,6°}$. b) $75 < 80,6$ → SORT : $\sin r = (1,48/1,46)\sin75° = 0,979$ → $r = 78,3°$. c) $85 > 80,6$ → $\boxed{\text{réflexion totale, piégé}}$ ✓.
🪤 *Piège testé : $\sin i_c = 1,48/1,46 = 1,014$ → « erreur calculatrice » — $\sin > 1$ impossible : $i_c$ part du DENSE ($n_1$ en BAS).*

## R4 — TYPE-BAC (téléchargement : DVD)

🏷️ matière=PC · année=— · session=— · chapitre=P9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Film DVD $4,7$ Go. Durée à $100$ Mbit/s ? à $1$ Gbit/s (fibre) ?

**Corrigé-type.** $Q = 4,7\times8 = 37,6$ Gbit $= 37600$ Mbit. ADSL : $t = 37600/100 = \boxed{376\text{ s} \approx 6,3\text{ min}}$ ; fibre : $t = 37600/1000 = \boxed{37,6\text{ s}}$.
🪤 *Piège testé : $t = 4,7/100$ (Go ÷ Mbit/s mélangés !) — convertir en MÊME unité (bits) AVANT de diviser.*

## R5 — TYPE-BAC (démodulation : détecteur d'enveloppe, 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P9 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—

**Énoncé.** Signal AM : $F_p = 100$ kHz, $f_s = 1,0$ kHz. Détecteur : diode + $R = 10$ k$\Omega$, $C = 10$ nF. a) Rôle de chaque étage ? b) La démodulation est-elle bonne (2 méthodes !) ? c) On remplace $C$ par $1,0$ $\mu$F : quel défaut ?

**Corrigé-type.** a) Diode : supprime les alternances négatives (redressement) ; RC : charge vite (diode passante) + décharge lentement ($R$) → suit l'ENVELOPPE = l'info.
b) $T_p = 10$ $\mu$s, $T_s = 1,0$ ms, $RC = 10^4 \times 10^{-8} = 0,10$ ms. **Méthode 1 (double inégalité)** : $10$ $\mu$s $\ll 100$ $\mu$s $\ll 1000$ $\mu$s → $\boxed{T_p \ll RC \ll T_s}$ ✔ bonne démodulation. **Méthode 2 (rapports)** : $RC/T_p = 10$ (lisse la HF ✔) et $T_s/RC = 10$ (suit l'enveloppe ✔) — les deux marges $\geq 10$ ✔.
c) $RC = 10$ ms $> T_s = 1,0$ ms → $RC$ TROP GRAND → $\boxed{\text{écrêtage}}$ (descentes plates : la décharge ne suit plus !).
🪤 *Piège testé : « $RC = 0,10$ ms $< T_s$ donc bon » (UNE seule inégalité vérifiée !) — il faut LES DEUX côtés ($T_p \ll RC$ ET $RC \ll T_s$) : $RC = 1$ $\mu$s passerait le 2e test mais pas le 1er (ondulation !).*

## VRAIE — 2025R Ex3-Partie II (modulation AM : $F$, $f$, $A$, $m$)

🏷️ matière=PC · année=2025 · session=R · chapitre=P9 · type=VRAIE · fidélité=reconstitué-corrigé · niveau=★★ · barème=Q1 0,5 · Q2 0,75

> ⚠️ **Reconstituée** depuis les éléments de réponse officiels (correction provinciale Mohammedia, scribd 889488300, Tier B). $F$ et $m$ : AN source illisibles, valeurs **recalculées** (à recouper) ; $f$, $A$, conclusion : lues.
> Données (reconstituées) : signal modulé en amplitude observé à l'oscilloscope ($T_s$ porteuse, $T_m$ enveloppe, $U_{max}$/$U_{min}$).

**Q1.** Déterminer la fréquence $F$ de la porteuse et $f$ du signal modulant. (2×0,25)
**Q2.** Déterminer $A$ et le taux de modulation $m$. La modulation est-elle bonne ? (3×0,25)
**Corrigé-type :**
1. $F = 1/T_s$ ($T_s = 5\ \mu$s lus) → $\boxed{F \approx 2\times 10^5\text{ Hz}}$ (recalculé) ; $f = 1/T_m$ ($T_m = 0,6$ ms) → $\boxed{f = 1667\text{ Hz}}$.
2. $U_{max} = A(1+m)$, $U_{min} = A(1-m)$ → $A = (U_{max}+U_{min})/2 = \boxed{1\text{ V}}$ ; $m = (U_{max}-U_{min})/(U_{max}+U_{min}) \approx \boxed{0,45}$ (à recouper). $\boxed{\text{Bonne modulation}}$ : $m < 1$ ET $F > 10f$ ($2\times 10^5 \gg 16670$ ✔).
🪤 *Piège testé : $T_s$ confondue avec $T_m$ (porteuse = petites oscillations rapides !) ; $m$ sans les 2 conditions (m<1 SEUL ne suffit pas !).*
🗣️ الخلاصة : الحاملة سريعة ($F \approx 200$ kHz!) والمعدِّلة بطيئة ($f = 1667$ Hz)! $A = 1$ V و$m \approx 0,45$! والتضمين **مزيان**: $m < 1$ **و** $F > 10f$ (بجوج الشروط!)!

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | bits = octets | ÷8 systématique |
| R2 | log oublié | dB = $10\log$ ! |
| R3 | $n_1$/$n_2$ inversés | dense en bas ($\sin<1$) |
| R4 | Go ÷ Mbit/s | tout en bits d'abord |
| R5 | 1 seule inégalité | $T_p \ll RC \ll T_s$ : LES DEUX ! |
| R5 | écrêtage/ondulation inversés | grand $RC$ = paresseux (écrête) |
| 2025R | $T_s \leftrightarrow T_m$ | porteuse = rapide ; $m<1$ ET $F>10f$ |

## VRAIE — 2021N Ex4-III (modulation AM : 1500/125 Hz)

🏷️ matière=PC · année=2021 · session=N · chapitre=P9 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
Définition : l'amplitude de la porteuse (haute $f$) varie avec le modulant (basse $f$ = l'info). Porteuse : $12T_p = 4\text{div}\times2\text{ms}$ → $F_p = 1500$ Hz. Modulante : $T_s = 4\text{div}\times2\text{ms} = 8$ ms → $f_s = 125$ Hz. $S_m = (U_M-U_m)/2 = 0,5$ V ; $U_0 = (U_M+U_m)/2 = 1,5$ V. $\tau = S_m/U_0 = 0,33 < 1$ + $F_p \geq 10f_s$ ($1500 \geq 1250$ ✓) → bonne qualité.
🪤 *vraie : 12 périodes sur 4 div (compter les oscillations !) ; 2 conditions ($\tau<1$ ET $F_p\geq10f_s$).*
