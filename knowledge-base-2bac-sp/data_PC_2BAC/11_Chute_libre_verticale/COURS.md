---
chapitre: "11 - Chute libre verticale"
unite: "Physique S2 - Mécanique"
source: "Cours type-bac 2BAC SP (à recouper)"
date: "2026-09-15"
type: "summary"
niveau: "2BAC SP"
---

> **Pointer** : `11_Chute_libre_verticale` → P4 (chute libre + frottement + Archimède) →COURS + EXERCICES_TYPES.

# Chute libre verticale (P11)

## 1. Image réelle — la goutte de pluie qui ne tue pas 🌧️

Une goutte tombe de 2000 m. Sans air : $v = \sqrt{2gh} \approx 200$ m/s — une balle ! Pourtant elle arrive à ~20 km/h. C'est le **frottement de l'air** qui la sauve : plus elle va vite, plus l'air la freine, jusqu'à une **vitesse limite** qu'elle ne dépasse jamais.
Ce chapitre : chute libre (vide) → chute avec air → chute dans un liquide.

## 2. Chute libre (vide) : $a = g$, la masse disparaît

**Définition** : chute libre = **seul le poids** agit (vide, ou air négligeable).

PFD sur axe vertical descendant : $ma = mg$ → $\boxed{a = g}$ ($g = 9,8$ m/s²).
**La masse $m$ s'élimine !** Galilée avait raison : plume et marteau tombent ensemble (sur la Lune !).

Équations (axe $Oz$ **descendant**, $v_0 = 0$) :
$$\boxed{v = gt} \qquad \boxed{z = \tfrac{1}{2}gt^2} \qquad \boxed{v^2 = 2gz}$$

Si lancé vers le haut ($v_0$, axe ascendant) : $v = -gt + v_0$, $z = -\tfrac{1}{2}gt^2 + v_0t$. **Le signe dépend de l'axe choisi !**

## 3. Chute avec frottement : la vitesse limite

Dans un fluide : $\vec{P} + \vec{f} = m\vec{a}$ avec $f = kv$ (Stokes, lent) ou $kv^2$ (rapide).

Deux régimes : **transitoire** ($v$ croît, $a$ décroît) → **permanent** ($a = 0$, $v = v_{lim}$ = constante).

En régime permanent ($a = 0$) : $mg - kv_{lim} = 0$ →
$$\boxed{v_{lim} = \frac{mg}{k}}$$
(Stokes : $k = 6\pi\eta r$ → $v_{lim} = mg/6\pi\eta r$.)
Temps caractéristique : $\tau = m/k$ (63% de $v_{lim}$ atteints à $t = \tau$ ; régime permanent ≈ $5\tau$).

## 4. Chute dans un liquide : Archimède s'en mêle

Dans un liquide il faut ajouter la **poussée d'Archimède** $\Pi = \rho_{fluide} V g$ (vers le haut) :
$$m\vec{a} = \vec{P} + \vec{\Pi} + \vec{f}$$
Vitesse limite : $v_{lim} = mg(1 - \rho_f/\rho_s)/k$ (bille de masse volumique $\rho_s$).
**Si $\rho_s < \rho_f$ → la bille REMONTE** (bouchon !) — même formule, $v_{lim}$ négative.

## 5. Énergie : le raccourci

Chute libre sans $v_0$ : $\tfrac{1}{2}mv^2 = mgh$ → $\boxed{v = \sqrt{2gh}}$ (masse éliminée, encore !).
Avec frottement : $\tfrac{1}{2}mv^2 < mgh$ — l'écart = travail du frottement (dissipé en chaleur).

## 5.1. Équation différentielle + solution (modèle linéaire $f = kv$)

Bilan (axe descendant, liquide) : $m\frac{dv}{dt} = mg - \Pi - kv$ avec
$\Pi = \rho_f V g$. En divisant par $m$ :
$$\boxed{\frac{dv}{dt} + \frac{k}{m}v = g\left(1 - \frac{\rho_f}{\rho_s}\right)} \qquad \tau = \frac{m}{k}$$
**Solution** (lâché sans vitesse, $v_0 = 0$) :
$$\boxed{v(t) = v_{lim}\left(1 - e^{-t/\tau}\right)} \qquad v_{lim} = \frac{mg}{k}\left(1-\frac{\rho_f}{\rho_s}\right)$$
**Lecture graphique** (question la plus rentable du chapitre !) : sur $v(t)$,
l'**asymptote horizontale** = $v_{lim}$ ; la **tangente à l'origine** coupe
l'asymptote à $t = \tau$ (VRAIE 2021N : on prouve la chute libre par la PENTE
$a = \Delta v/\Delta t = g$ en phase 1 !). Sur $a(t)$ : part de $g$ (ou
$g(1-\rho_f/\rho_s)$), tend vers 0.

## 5.2. Modèle quadratique $f = \mu v^2$ (rapide : parachute, cascadeur)

À grande vitesse on pousse le fluide : $f = \mu v^2$ ($\mu$ en **kg/m** —
vérifier : $\mu v^2$ = N ✓). EDL :
$$\boxed{\frac{dv}{dt} + \frac{\mu}{m}v^2 = g} \qquad \boxed{v_{lim} = \sqrt{\frac{mg}{\mu}}}$$
Pas de solution exponentielle exigible : on exploite la **courbe**
($dv/dt = f(v^2)$ est une DROITE : ordonnée à l'origine $g$, abscisse à
l'origine $v_{lim}^2$ — VRAIE 2026N : $v_{lim}^2 = 3120$ → $v_{lim} = 55{,}9$ m/s)
ou la **méthode d'Euler** (§5.3). Dans l'air, $\Pi$ est négligeable.

## 5.3. Méthode d'Euler (exigible — tombée 2026N !)

Quand l'EDL ne se résout pas à la main, on avance **pas à pas** :
$$a_i = g - \frac{\mu}{m}v_i^2 \qquad \longrightarrow \qquad v_{i+1} = v_i + a_i \cdot \Delta t$$
Recette : ① $a_0$ depuis $v_0$ ; ② $v_1 = v_0 + a_0\Delta t$ ; ③ $a_1$ depuis
$v_1$ ; ④ $v_2 = v_1 + a_1\Delta t$… (VRAIE 2026N : $\Delta t = 0{,}5$ s,
$\mu/m = 3{,}125\times10^{-3}$ → $v_1 = 4{,}9$, $a_1 = 9{,}725$, $v_2 = 9{,}763$ m/s.)
🗣️ Darija : أويلر = **خطوة بخطوة** : حسب التسارع من السرعة الحالية، زيد
$a\times\Delta t$ باش تلقى السرعة الجاية، وعاود. ما تحفظش — **طبق الجدول**.

## 5.4. Tableau de bord — quel modèle, quel réflexe ?

| Situation | Modèle | $v_{lim}$ | Outil |
|---|---|---|---|
| Vide / air négligeable | libre | — ($v = gt$) | $z = \tfrac12gt^2$, $v^2 = 2gz$ |
| Bille lente (huile, eau) | $f = kv$ (+ $\Pi$ si liquide) | $mg(1-\rho_f/\rho_s)/k$ | EDL + $v(t)$ expo + tangente |
| Rapide (parachute, cascadeur) | $f = \mu v^2$ | $\sqrt{mg/\mu}$ | droite $dv/dt = f(v^2)$, Euler |

**Question-type « prouver la chute libre »** (2021N) : on ne l'affirme jamais —
on **mesure** $a = $ pente de $v(t)$ en phase 1 et on montre $a = g$.
**Question-type « ce modèle explique-t-il la réalité ? »** (2026N) : comparer
la prédiction ($v_f = 1385$ km/h en chute libre !) à la mesure (200 km/h) —
écart énorme = modèle invalide, il manque le frottement.

## 6. Unités SI — non négociable 📏

$v$ : m/s (÷3,6 depuis km/h !). $g$ : m/s². $k$ : kg/s (linéaire) ou kg/m (quadratique — vérifier par analyse dimensionnelle !). $\eta$ : Pa·s. $\tau$ : s.

## 7. Darija — الشرح 🇲🇦

السقوط الحر = غير الوزن كاين، الهوا والو. القانون كيعطي $a = g$ — **الكتلة كتمشي بحالها من المعادلة !** الريشة والمطرقة كيطيحو بنفس السرعة (فالقمر حيت ما كاين هوا).
فالهوا ولا الزيت كاين الاحتكاك : كلما زدتي فالسرعة زاد الفرملة، حتى كتثبت السرعة — **السرعة الحدية** $v_{lim} = mg/k$. بحال الباراشوت : كتسرع شوية ومن بعد كتنزل بسرعة ثابتة.
فالسائل زيد **دافعة أرخميدس** لفوق : إذا الجسم خفيف على السائل كيطلع ماشي كيهبط !

## 8. How to understand this chapter the easy way 🗣️

Écoute-moi bien. D'abord : dans le vide, tout tombe pareil — oublie « lourd = vite », c'est FAUX, c'est l'air qui trompe.
Ensuite : avec l'air, deux phases — ça accélère PUIS ça se stabilise. La vitesse limite, c'est quand le poids et le frottement s'annulent : $a = 0$, équilibre !
Erreur qui tue : le signe. Axe vers le bas : $v = +gt$. Axe vers le haut : $v = -gt + v_0$. Dessine ton axe AVANT d'écrire.
Dernier truc : la bille dans l'huile (TP classique) — Stokes + Archimède + vitesse limite : c'est LE sujet qui tombe.

## 9. Pourquoi c'est comme ça (le deep « why ») 🔬

- **Pourquoi $m$ s'élimine ?** Le poids ($mg$) est la CAUSE, l'inertie ($m$) la RÉSISTANCE — les deux proportionnelles à $m$ : double masse = double force mais double résistance → même $a$. C'est le principe d'équivalence (Einstein en a fait la relativité générale !).
- **Pourquoi une limite ?** $f$ croît avec $v$ mais $P$ est constant : à un moment $f = P$ → $a = 0$ → $v$ figée. C'est un **équilibre dynamique** (comme le thermostat : §3 de chimie-cinétique P18 !).
- **Pourquoi $f = kv$ ou $kv^2$ ?** Lent = frottement visqueux (couches de fluide, Stokes) ; rapide = il faut POUSSER le fluide (traînée aérodynamique ∝ $v^2$). La goutte de pluie : $kv^2$. La bille dans l'huile : $kv$.
- **Lien P10** : tout est PFD ($\Sigma F = ma$) avec des forces différentes. **Lien P28** : un satellite = une chute permanente qui « rate » la Terre !

## 10. Les confusions qui tuent ⚠️

1. **« Lourd tombe plus vite »** → FAUX dans le vide ; dans l'air c'est le RAPPORT poids/frottement ($v_{lim} = mg/k$) qui compte, pas $m$ seule. Ce qui clique : la feuille froissée tombe plus vite que la feuille plate — MÊME masse, $k$ différent !
2. **Signes selon l'axe** → $v = gt$ SEULEMENT si axe descendant + $v_0 = 0$. Axe ascendant : $v = -gt + v_0$. Ce qui clique : l'équation ne sait pas où est « le bas » — c'est TON axe qui décide ; dessine-le toujours.
3. **Archimède oublié dans les liquides** → dans l'huile/eau, $\Pi$ n'est PAS négligeable (elle peut valoir 10-20% de $P$). Ce qui clique : « dans un liquide, tout objet perd du poids » — c'est ce poids PERDU qu'il faut soustraire.

## 11. Signaux adaptatifs 🧭

- **Prérequis** : P10 (PFD — indispensable), dérivation/intégration ($a \to v \to z$), équations différentielles ($v' + v/\tau = C$ — voir maths M10).
- **Si l'équa diff bloque** (angle de secours) : pour $v_{lim}$ tu n'en as PAS besoin — régime permanent = équilibre = $a = 0$ → $mg = kv_{lim}$ directement. L'équa diff ne sert que pour $v(t)$ complet.
- **Test 30 s** : bille acier VS bille bois même taille dans l'huile — laquelle a la plus grande $v_{lim}$ ? (Acier : même $k$, $m$ plus grand → $v_{lim} = mg/k$ plus grand ✓.)
