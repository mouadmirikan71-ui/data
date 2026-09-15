---
chapitre: "09 - Transmission information modulation demodulation"
unite: "Physique S0 - Ondes"
source: "Cours type-bac 2BAC SP (à recouper)"
date: "2026-09-15"
type: "summary"
niveau: "2BAC SP"
---

> **Pointer** : `09_Transmission_information_modulation_demodulation` → P4 (chaîne, analog/num, fibre, dB, débit) →COURS + EXERCICES_TYPES.

# Transmission d'informations (P09)

## 1. Image réelle — la lumière qui téléphone 💡

Un appel Casa–Dakar voyage dans une fibre de verre fine comme un cheveu, à 200 000 km/s, sans AUCUNE perte aux parois : la lumière y est **piégée par réflexion totale** — elle rebondit sans jamais sortir. Et ta voix ? Découpée en 0 et 1, régénérée à chaque relais : c'est pour ça qu'elle arrive intacte.
Ce chapitre : la chaîne complète — signal → propagation → réception.

## 2. Chaîne de transmission : émetteur → canal → récepteur

- **Émetteur** : convertit l'info en signal (micro → électrique, laser → lumineux).
- **Canal** : libre (air : wifi, 4G) ou **guidé** (câble, fibre optique).
- **Récepteur** : reconvertit (haut-parleur, photodiode).
- Ennemis : **atténuation** (signal affaibli) et **bruit** (parasites). Le numérique résiste au bruit, l'analogique non (§9 !).

## 3. Analogique vs numérique : Shannon

- **Analogique** : varie continûment (voix, thermomètre).
- **Numérique** : 0/1 (échantillons quantifiés). Conversion : **CAN** (échantillonnage + quantification).
- **Shannon** : $\boxed{f_e \geq 2f_{max}}$ — échantillonner ≥ 2× la fréquence max du signal (CD audio : $f_e = 44,1$ kHz $> 2\times20$ kHz ✓).
- Sous-échantillonné = info perdue à jamais (roues de cinéma qui tournent à l'envers !).

## 4. Fibre optique : la réflexion totale

Cœur ($n_1$) + gaine ($n_2 < n_1$) : un rayon assez rasant est **totalement réfléchi** (zéro perte !).
Condition : aller du PLUS réfringent vers le MOINS ($n_1 > n_2$) + incidence $i > i_c$ :
$$\boxed{\sin i_c = n_2/n_1}$$
Ex. : $n_1 = 1,48$, $n_2 = 1,46$ → $\sin i_c = 0,9865$ → $i_c = 80,6°$ (rasant !). Avantages fibre : débit énorme, insensible aux parasites, légère.

## 5. Atténuation (dB) et débit binaire

- **Atténuation** : $\boxed{A = 10\log(P_e/P_s)}$ en décibels (dB). Réflexes : $\times10$ = $+10$ dB, $\times2$ ≈ $+3$ dB, $\div2$ ≈ $-3$ dB.
- Ex. : $100$ mW → $25$ mW : $A = 10\log 4 = 6,0$ dB.
- **Débit** $D$ (bit/s) : durée $t = Q/D$ ($Q$ = quantité en bits). Ex. : photo $1920\times1080\times24 = 49,8$ Mbit à $10$ Mbit/s → $t = 5,0$ s.
- Fibre monomode : atténuation ~0,2 dB/km (relais tous les ~100 km !).

## 5bis. Modulation d'amplitude (AM) 📡

- **Principe** : l'info basse fréquence $s(t) = S_m\cos(2\pi f_s t)$ (voix : $f_s \sim$ kHz) ne peut pas être émise directement (antenne géante ! §9). On l'inscrit sur l'AMPLITUDE d'une porteuse haute fréquence $p(t) = U_0\cos(2\pi F_p t)$ : $\boxed{u_m(t) = [U_0 + S_m\cos(2\pi f_s t)]\cos(2\pi F_p t)}$ — l'enveloppe de $u_m$ = l'info !
- **Taux de modulation** : $\boxed{\tau = S_m/U_0}$ (sans unité !). Mesure sur oscillogramme : $\boxed{S_m = (U_M-U_m)/2}$, $\boxed{U_0 = (U_M+U_m)/2}$ ($U_M$/$U_m$ = enveloppes max/min !).
- **Bonne modulation (2 conditions !)** : $\boxed{\tau < 1}$ (pas de surmodulation : l'enveloppe ne s'annule jamais !) ET $\boxed{F_p \geq 10f_s}$ (porteuse ≫ modulante : l'enveloppe est bien définie !).
- **Spectre** : 3 raies — $F_p$ (porteuse) + $F_p - f_s$ et $F_p + f_s$ (bandes latérales = l'info !). Largeur occupée : $2f_s$.

## 5ter. Démodulation : le détecteur d'enveloppe 📻

- **But** : récupérer $s(t)$ (l'enveloppe) à partir de $u_m(t)$ — c'est le circuit du poste radio ! 2 étages :
  1. **Diode** : supprime les alternances négatives (redressement — on ne garde que le haut, là où vit l'enveloppe !).
  2. **RC parallèle** : le condensateur se charge VITE (via diode passante, $R_{diode} \approx 0$) et se décharge LENTEMENT dans $R$ → la tension suit l'ENVELOPPE (le haut des oscillations HF est « rempli » !).
- **Condition de bonne démodulation (double inégalité !)** : $\boxed{T_p \ll RC \ll T_s}$ ($T_p = 1/F_p$, $T_s = 1/f_s$) — $RC \gg T_p$ : lisse la HF (pas d'ondulation résiduelle !) ; $RC \ll T_s$ : suit les descentes de l'enveloppe (pas d'écrêtage !).
- **2 défauts (diagnostic d'oscillogramme !)** : $RC$ TROP PETIT → **ondulation résiduelle** (résidu HF visible : le lissage est incomplet) ; $RC$ TROP GRAND → **écrêtage** (les descentes sont coupées/plates : la décharge ne suit plus l'enveloppe !).

## 6. Unités — non négociable 📏

Bit (b) vs octet (o = 8 bits) — 10 Mo = 80 Mb ! Débit : bit/s (Mbit/s). $A$ : dB (sans dimension, log !). $f_e$ : Hz. $n$ : sans unité.

## 7. Darija — الشرح 🇲🇦

المعلومة كتسافر : المرسل → القناة → المستقبل. القناة حرة (الهوا : الويفي) ولا موجهة (الكابل، الفايبر).
الإشارة تماثلية (مستمرة : الصوت) ولا رقمية (0/1). التحويل رقمي خاصو **شانون** : $f_e \geq 2f_{max}$ — خاصك تقطع الإشارة على الأقل ضعف التردد ديالها.
الفايبر : الضو محبوس بالانعكاس الكلي — **صفر ضياع !** الشرط : من الوسط الكثيف للخفيف + زاوية كبيرة ($\sin i_c = n_2/n_1$).
التوهين بالديسيبيل : $A = 10\log(P_e/P_s)$ — $\times10$ هي $+10$ dB، $\times2$ هي $+3$ dB. حفظ هاد الجوج وضمن النقط !
التضمين السعوي AM : المعلومة (تردد صغير $f_s$) كتركب على **سعة** حاملة (تردد كبير $F_p$) — الغلاف هو المعلومة ! شرط الجودة : $\tau = S_m/U_0 < 1$ و$F_p \geq 10f_s$. إزالة التضمين (**كاشف الغلاف**) : **ديود** (كيحيد السالب) + **RC** (كيشحن بسرعة وكيفرغ بشوية ← كيتبع الغلاف !). الشرط المزدوج : $T_p \ll RC \ll T_s$ — $RC$ صغير بزاف ← **تموج باقي** ؛ $RC$ كبير بزاف ← **قص** (ما كيتبعش النزلات) !

## 8. How to understand this chapter the easy way 🗣️

D'abord : 3 boîtes — émetteur, canal, récepteur. Tout exo commence par les identifier.
Ensuite : 2 nombres magiques — Shannon ($f_e \geq 2f_{max}$) et le dB ($\times10$/$+10$, $\times2$/$+3$). Avec eux, 80% des questions tombent.
La fibre : UNE formule ($\sin i_c = n_2/n_1$) + UNE condition ($n_1 > n_2$, du dense vers le rare). Dessine le rayon rasant.
Et le piège eternal : bit vs octet. 10 Mo/s $\neq$ 10 Mb/s — facteur 8 ! Lis l'unité AVANT de diviser.

## 9. Pourquoi c'est comme ça (le deep « why ») 🔬

- **Pourquoi le numérique bat l'analogique ?** Bruit de 0,2 V sur un signal analogique 0–5 V = info corrompue à jamais. Sur du numérique (seuil à 2,5 V), le relais **régénère** : au-dessus → 1 parfait, en dessous → 0 parfait. Le bruit est EFFACÉ à chaque relais. C'est pour ça que la TV analogique neigeait et que la TNT est parfaite... ou absente (effet falaise !).
- **Pourquoi réflexion TOTALE (zéro perte) ?** Au-delà de $i_c$, Snell-Descartes exigerait $\sin r > 1$ — impossible : le rayon réfracté n'existe plus, TOUTE l'énergie repart en réflexion. Pas « presque tout » : tout. D'où 100 km sans relais.
- **Pourquoi des dB (log) ?** Les puissances vont de $10^{-12}$ à $10^3$ W : le log compresse 15 ordres de grandeur en ~150 dB, et les atténuations en cascade S'ADDITIONNENT (au lieu de se multiplier). **Lien maths M05** : $\log(ab) = \log a + \log b$.
- **Lien P03** : Snell-Descartes ($n_1\sin i_1 = n_2\sin i_2$) = la mère de $i_c$. **Lien P01/P02** : porteuse modulée = onde (P01/P02) transportant l'info.

## 10. Les confusions qui tuent ⚠️

1. **Bit vs octet** → $1$ o $= 8$ b. « 80 Mb à 10 Mo/s » : $t = 80/(10\times8) = 1$ s, pas 8 s ! Ce qui clique : l'octet est un PAQUET de 8 bits — divise les paquets, pas les bits.
2. **Sens de $i_c$** → $\sin i_c = n_2/n_1$ avec $n_1 > n_2$ (départ du MILIEU DENSE). Ce qui clique : on ne peut être « piégé » que dans le milieu dense — le rayon essaie de sortir vers le rare et échoue.
3. **dB : $\times2$ = $+6$ dB ?** → NON : $10\log 2 = 3,0$ dB ($+6$ dB = $\times4$ ; $+10$ dB = $\times10$). Ce qui clique : $10\log(2\times2) = 3+3 = 6$ — les dB s'additionnent, les rapports se multiplient.

## 11. Signaux adaptatifs 🧭

- **Prérequis** : P01/P02 (ondes), P03 (Snell-Descartes — indispensable pour la fibre), log décimal (maths M05).
- **Si les dB bloquent** (angle de secours) : ne retiens que 3 couples — ($\times10$/$+10$), ($\times2$/$+3$), ($\div2$/$-3$) — et décompose : $\times40$ $=$ $\times10\times2\times2$ → $+10+3+3 = +16$ dB. Zéro calculatrice !
- **Test 30 s** : signal divisé par 100 en puissance — atténuation ? ($10\log 100 = 20$ dB ✓.)
