---
chapitre: "13 - Rotation solide axe fixe"
unite: "Physique S2 - Mécanique"
source: "Cours type-bac 2BAC SP (à recouper)"
date: "2026-09-15"
type: "summary"
niveau: "2BAC SP"
---

> **Pointer** : `13_Rotation_solide_axe_fixe` → P4 (angles, moments, J, Ec rotation) →COURS + EXERCICES_TYPES.

# Rotation d'un solide autour d'un axe fixe (P13)

## 1. Image réelle — la patineuse et la porte ⛸️

La patineuse tourne bras ouverts, puis serre les bras... et accélère FORT. Même patineuse, même énergie — mais la masse s'est rapprochée de l'axe : elle tourne plus vite. C'est le **moment d'inertie** : en rotation, ce qui compte n'est pas (seulement) la masse, mais OÙ elle se trouve.
Et la porte : tu pousses près des gonds ? impossible. Au bout ? facile. Même force, effet différent : c'est le **moment**.

## 2. Cinématique : $\theta$, $\omega$ — et le radian est ROI

- Abscisse angulaire $\theta$ (rad), vitesse angulaire $\omega = d\theta/dt$ (**rad/s**), $v = R\omega$ en un point à distance $R$ de l'axe.
- MCU (uniforme) : $\omega$ = cste, $\theta = \omega t + \theta_0$, période $T = 2\pi/\omega$, accélération **centripète** $a_n = v^2/R = R\omega^2$ (vers le centre — oui, il y a une accélération même si $v$ = cste !).
- **TOUT en radians** : $\omega$ en rad/s, jamais en °/s ni en tr/min (convertir : $1$ tr/min $= 2\pi/60 = 0,105$ rad/s).

## 3. Moment d'une force : $M = F \times d$

$$\boxed{M = F \cdot d}$$
$d$ = **bras de levier** = distance (perpendiculaire !) entre l'axe et la droite d'action de $F$. Unité : N·m (pas des joules !).
Signe : + si ça tourne dans le sens choisi, − sinon. Une force qui passe PAR l'axe : $d = 0$ → moment nul (elle ne fait pas tourner !).

## 4. RFD en rotation : $\Sigma M = J\cdot\ddot{\theta}$

L'équivalent de $F = ma$ pour la rotation autour d'un axe fixe :
$$\boxed{\sum M = J\ddot{\theta}}$$
$J$ = moment d'inertie (kg·m², dépend de la RÉPARTITION de la masse — admis) :
| Solide | $J$ |
|---|---|
| Cerceau/anneau ($m$, $R$) | $mR^2$ |
| Cylindre plein/disque | $\tfrac{1}{2}mR^2$ |
| Sphère pleine | $\tfrac{2}{5}mR^2$ |
| Tige (milieu, longueur $L$) | $\tfrac{1}{12}mL^2$ |
Le cerceau ($mR^2$) > le disque ($\tfrac{1}{2}mR^2$) : masse loin de l'axe = plus dur à lancer (patineuse bras ouverts !).

## 5. Énergie cinétique de rotation

$$\boxed{E_c = \tfrac{1}{2}J\omega^2} \qquad (\omega \text{ en rad/s !})$$
Théorème de l'$E_c$ : $\Delta E_c = \sum W$ (travaux des moments). Roulement sans glissement : $E_c = \tfrac{1}{2}mv^2 + \tfrac{1}{2}J\omega^2$ (translation + rotation — la voiture !).

## 6. Unités SI — non négociable 📏

$\theta$ : rad. $\omega$ : rad/s. $J$ : kg·m². $M$ : N·m. $E_c$ : J. Conversions : tr/min → rad/s ($\times 2\pi/60$), tours → rad ($\times 2\pi$).

## 7. Darija — الشرح 🇲🇦

الدوران عندو نفس قوانين الحركة المستقيمة غير بالأسماء مبدلة : الكتلة $m$ ولات $J$ (عزم القصور)، القوة $F$ ولات $M$ (العزم)، السرعة $v$ ولات $\omega$.
العزم $M = F\times d$ : القوة مضروبة فالبعد على المحور — **البعد العمودي !** القوة اللي دايزة من المحور ما كدور والو ($d = 0$).
$J$ كيعتمد على **فين كاينة الكتلة** : الطوق ($mR^2$) صعيب يدور من القرص ($\frac{1}{2}mR^2$) حيت الكتلة بعيدة — بحال المتزلجة : يدين محلولين = بطيئة، يدين مسدودين = سريعة !
**الراديان إجباري** : $\omega$ بالراديان/ثانية، اللي حسب بالدرجات ولا الدورات كلشي غالط.

## 8. How to understand this chapter the easy way 🗣️

Retiens le tableau magique translation ↔ rotation : $m \leftrightarrow J$, $F \leftrightarrow M$, $v \leftrightarrow \omega$, $F = ma \leftrightarrow \Sigma M = J\ddot{\theta}$, $\tfrac{1}{2}mv^2 \leftrightarrow \tfrac{1}{2}J\omega^2$. Tout ce que tu sais en translation se TRANSPOSE.
Ensuite : $M = F\cdot d$ — la porte : loin des gonds = facile. Et $d$ perpendiculaire, force par l'axe = moment nul.
Le réflexe unités : dès que tu vois tr/min ou tours, CONVERTIS en rad/s et rad en première ligne. 50% des erreurs du chapitre meurent ici.
Dernier : $J$ par cœur (4 formules) — cerceau > disque > sphère, dans cet ordre ($1 > 1/2 > 2/5$).

## 9. Pourquoi c'est comme ça (le deep « why ») 🔬

- **Pourquoi $J$ dépend de la répartition ?** $J = \sum m_ir_i^2$ : chaque gramme compte ∝ $r^2$. À $\omega$ donnée, un gramme à $2R$ va 2× plus vite donc a 4× plus d'$E_c$ ($\tfrac{1}{2}mv^2$) : il « coûte » 4× plus cher à lancer. La patineuse qui serre les bras diminue son $J$ → à moment cinétique conservé, $\omega$ explose.
- **Pourquoi $M = F\cdot d$ ?** Le travail d'une force en rotation : $W = F \times$ (arc) $= F\cdot d\cdot\theta = M\cdot\theta$. Le moment, c'est « combien de travail par radian » — l'exact analogue de $W = F\cdot x$.
- **Pourquoi N·m $\neq$ J ?** Même dimension ($ML^2T^{-2}$) mais sens différent : le joule = énergie (scalaire, travail EFFECTUÉ), le N·m = moment (capacité à faire tourner). On ne les mélange jamais.
- **Lien P28** : satellite = rotation autour de la Terre, $a_n = v^2/r$ des deux côtés. **Lien P14/P15** : le pendule = rotation oscillante ($\Sigma M = J\ddot{\theta}$ avec $M = -mgd\sin\theta$ !).

## 10. Les confusions qui tuent ⚠️

1. **Degrés/tours au lieu de radians** → $v = R\omega$, $E_c = \tfrac{1}{2}J\omega^2$ exigent des RADIANS. Ce qui clique : le radian est « sans unité » ($arc/R$) — c'est pour ça que les formules marchent avec lui et pas avec les degrés !
2. **$d$ = n'importe quelle distance** → NON : $d$ = distance PERPENDICULAIRE axe–droite d'action. Ce qui clique : seule la composante perpendiculaire fait tourner ; pousse une porte vers les gonds, elle ne bouge pas !
3. **« MCU = pas d'accélération »** → FAUX : $a_n = v^2/R$ vers le centre (la DIRECTION change !). Ce qui clique : en voiture dans un virage à vitesse constante, tu es plaqué — c'est cette accélération que ton corps sent.

## 11. Signaux adaptatifs 🧭

- **Prérequis** : P10 (PFD — à transposer), dérivation ($\omega = \dot{\theta}$), trigonométrie de base.
- **Si $\Sigma M = J\ddot{\theta}$ bloque** (angle de secours) : passe par l'ÉNERGIE ($\tfrac{1}{2}J\omega^2$) — la moitié des exos (vitesses, hauteurs) se résolvent sans jamais écrire l'équation différentielle.
- **Test 30 s** : disque VS cerceau mêmes $m$, $R$, lâchés sur un plan incliné (roulement) — qui arrive en bas en premier ? (Disque : $J$ plus petit → moins d'énergie « volée » par la rotation → translation plus rapide ✓.)
