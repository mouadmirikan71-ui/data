---
chapitre: "28 - BONUS Satellites et planetes (hors programme)"
unite: "Physique S2 - Mécanique"
source: "Cours type-bac 2BAC SP (à recouper)"
date: "2026-09-15"
type: "summary"
niveau: "2BAC SP"
---

> **Pointer** : `28_BONUS_Satellites_et_planetes` → P4 (gravitation, Kepler, géostationnaire) →COURS + EXERCICES_TYPES.

# Satellites et planètes (P28) — ⚠️ BONUS hors programme officiel

> ⚠️ **Chapitre BONUS (hors-liste-officielle-2026)** : les satellites et planètes NE figurent PAS sur la liste officielle des 27 chapitres du national PC 2026. Contenu conservé comme culture/bonus (mécanique de Newton appliquée : gravitation, Kepler, géostationnaire) — NE PAS réviser en priorité ! Les 27 chapitres officiels : P01–P27.

## 1. Image réelle — le satellite qui tombe sans jamais tomber 🛰️

Imagine : tu lances une balle de plus en plus fort depuis une montagne. Elle tombe de plus en plus loin... À 8 km/s, elle tombe MAIS la Terre se courbe sous elle à la même vitesse — elle tombe **sans jamais toucher le sol**. C'est exactement ça, un satellite : **une chute libre permanente qui rate la Terre** (canon de Newton !).
GPS, météo, Starlink : tous « tombent » en ce moment même.

## 2. Gravitation : la seule force (référentiel géocentrique)

$$\boxed{F = G\frac{mM}{r^2}}$$
$G = 6,67\times10^{-11}$ SI, $M$ = masse de l'astre, $m$ = masse du satellite, $r$ = distance **entre les CENTRES** ($r = R_T + h$ !).
Direction : vers le centre de l'astre. Dans le référentiel géocentrique (centre Terre, axes vers étoiles lointaines), c'est la SEULE force → chute libre orbitale.

## 3. Orbite circulaire : uniforme, et $v$ ne dépend pas de $m$ !

PFD + repère de Frenet : $F = ma_n$ → $GmM/r^2 = mv^2/r$ → $m$ s'élimine (Galilée, encore !) :
$$\boxed{v = \sqrt{\frac{GM}{r}}} \qquad \boxed{T = \frac{2\pi r}{v} = 2\pi\sqrt{\frac{r^3}{GM}}}$$
- Mouvement **uniforme** ($v$ = cste) : la force est perpendiculaire à la vitesse → aucun travail → $v$ ne change, seule la DIRECTION tourne.
- Plus haut ($r$ grand) = plus LENT ($v \propto 1/\sqrt{r}$) — contre-intuitif mais c'est la clé du géostationnaire !
- **3e loi de Kepler démontrée** : $\boxed{T^2/r^3 = 4\pi^2/GM}$ = constante (pour un même astre).

## 4. Géostationnaire : fixe dans le ciel 📡

Conditions : **circulaire + équatoriale + même sens que la Terre + $T = 86164$ s** (jour SIDÉRAL, pas 86400 !).
Application : $r = \sqrt[3]{GMT^2/4\pi^2} = 42164$ km → $h = r - R_T = \boxed{35800\text{ km}}$, $v = 3,07$ km/s.
UN SEUL anneau possible (équatorial) — d'où les « places » orbitales limitées ! Météo, TV : géostat. GPS ($h \approx 20200$ km, $T \approx 12$ h), Starlink ($h \approx 550$ km) : NON géostat.

## 5. Les 3 lois de Kepler (énoncés)

1. **Orbites** : ellipses, Soleil/astre à un foyer (cercle = cas particulier).
2. **Aires** : le rayon balaye des aires égales en des temps égaux (→ plus vite près de l'astre !).
3. **Périodes** : $T^2/a^3$ = cste ($a$ = demi-grand axe ; $= T^2/r^3$ si cercle).
Vérification Lune : $T = 27,3$ j, $r = 384400$ km → $T^2/r^3 = 9,8\times10^{-14} \approx 4\pi^2/GM_T = 9,9\times10^{-14}$ ✓ (la Lune obéit !).

## 6. Unités SI — non négociable 📏

$r, h, R_T$ : **mètres** dans les formules ($R_T = 6,38\times10^6$ m) ! $T$ : secondes. $M_T = 5,97\times10^{24}$ kg, $M_S = 1,99\times10^{30}$ kg. $G$ : N·m²/kg². $v$ : m/s.

## 7. Darija — الشرح 🇲🇦

الساتل راه غير كيطيح ! كيطيح باستمرار ولكن الأرض كتحنّي تحت منو بنفس السرعة — كيطيح وما كيوصلش للأرض أبدا. هادي هي الفكرة ديال نيوتن.
القوة الوحيدة هي الجاذبية $F = GmM/r^2$، وكتعطي $v = \sqrt{GM/r}$ — **كتلة الساتل كتمشي بحالها !** ساتل صغير وكبير فنفس المدار عندهم نفس السرعة.
الثابت بالنسبة للأرض (géostationnaire) : خاصو يكون فوق خط الاستواء، $T = 86164$ ثانية (اليوم النجمي ماشي 86400 !)، والعلو $h = 35800$ كلم.
**الفخ الكبير : $r = R_T + h$** — نصف قطر المدار = نصف قطر الأرض + العلو ! اللي كينسى $R_T$ كلشي عندو غالط.

## 8. How to understand this chapter the easy way 🗣️

D'abord, grave ça : satellite = chute qui rate la Terre. Tout le reste suit.
Ensuite : UNE force (gravité), UNE formule de vitesse ($v = \sqrt{GM/r}$), et $m$ qui disparaît — comme Galilée au P11.
Le réflexe géostat : équatorial + $T = 86164$ s + $h = 35800$ km. Trois mots : « équateur, sidéral, 36 mégamètres ».
Et LE piège du siècle : $r = R_T + h$. À chaque exo, première ligne : convertir $h$ en $r$. Fais ça et tu as déjà la moitié des points.

## 9. Pourquoi c'est comme ça (le deep « why ») 🔬

- **Pourquoi $m$ s'élimine (encore) ?** Même raison qu'au P11 : la gravité tire ∝ $m$, l'inertie résiste ∝ $m$. Un éléphant et une plume orbitent à la même vitesse. C'est le principe d'équivalence, partout.
- **Pourquoi uniforme ?** $\vec{F} \perp \vec{v}$ → puissance $P = \vec{F}\cdot\vec{v} = 0$ → aucun travail → $E_c$ constante → $v$ constante. La force ne fait que TOURNER le vecteur vitesse (accélération centripète $v^2/r$). **Lien P13** : c'est le même $v^2/r$ qu'en rotation !
- **Pourquoi équatorial pour géostat ?** Le centre de l'orbite DOIT être le centre de la Terre (la force pointe vers lui). Un satellite « fixe » au-dessus de Paris décrirait un cercle dont le centre n'est pas le centre Terre → impossible. Seul l'équateur marche.
- **Pourquoi 86164 et pas 86400 ?** Le satellite doit tourner avec la Terre par rapport aux ÉTOILES (référentiel géocentrique) : jour sidéral = 23h56min4s. 86400 s, c'est par rapport au Soleil (la Terre a avancé sur son orbite entre-temps).

## 10. Les confusions qui tuent ⚠️

1. **$r$ vs $h$** → $h$ = altitude (donnée), $r = R_T + h$ = ce qui va dans les formules. Ce qui clique : la gravité part du CENTRE de la Terre, pas de sa surface — elle ne sait pas où est le sol !
2. **86400 vs 86164** → 86400 = jour solaire (Soleil), 86164 = jour sidéral (étoiles) = celui du géostat. Ce qui clique : le satellite s'en fiche du Soleil, il tourne avec la TERRE face aux étoiles fixes.
3. **« Plus haut = plus vite »** → FAUX : $v = \sqrt{GM/r}$ DÉCROÎT avec $r$. Ce qui clique : la Lune (loin) met 27 jours, l'ISS (près) 90 minutes — les proches sont les pressés !

## 11. Signaux adaptatifs 🧭

- **Prérequis** : P10 (PFD + repère de Frenet — $a_n = v^2/r$), puissances de 10 (ordres astro !), P11 (chute libre = même physique).
- **Si Frenet bloque** (angle de secours) : admets « la gravité courbe la trajectoire sans changer $v$ » + $v = \sqrt{GM/r}$ par cœur — 80% des exos (géostat, Kepler, comparaisons) se font sans Frenet.
- **Test 30 s** : 2 satellites, $r_2 = 4r_1$ — rapport des périodes ? ($T \propto r^{3/2}$ → $T_2 = 8T_1$ ✓.)
