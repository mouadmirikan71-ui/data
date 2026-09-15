---
chapitre: "29 - Méthodologie de l'épreuve de Physique-Chimie au national"
unite: "Transverse (tous chapitres)"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Cadre de référence examen national + annales 2015-2025 + synthèse prof"
date_collecte: "2026-09-14"
type: "methodology"
langues: "FR + Darija + LaTeX"
---

# Méthodologie — Réussir l'épreuve de PC au national (2BAC SP)

## 1. La démarche universelle (80 % des exercices de physique)

Tout exercice « système en mouvement / circuit / réaction » se traite avec le même plan — l'apprendre une fois, l'appliquer partout :

1. **Système + Référentiel** : « Système : {solide S} ; Référentiel terrestre supposé galiléen. »
2. **Bilan / schéma** : forces (poids, réaction, tension, frottement, électrique, magnétique...) avec un **schéma propre et orienté** ; en électricité : schéma + flèches $u$, $i$ + loi des mailles ; en chimie : équation + tableau d'avancement.
3. **Loi** : PFD $\sum\vec{F} = m\vec{a}$ / loi des mailles / conservation... **écrite en toutes lettres avant projection**.
4. **Projection + équation différentielle** : projeter sur les axes, obtenir l'EDP, vérifier homogénéité (unités !).
5. **Solution** : forme proposée ou intégration + **conditions initiales** (position/vitesse à $t = 0$, $u_C(0)$, $i(0)$...).
6. **Application numérique** : calcul + **unité SI** + chiffres significatifs cohérents + **encadrer**.
7. **Conclusion** : une phrase qui répond à la question (« La portée vaut... », « Le régime est pseudo-périodique car... »).

> بالدارجة: المنهجية وحدة فكلشي — النظام + المرجع ← القوى/الرسم ← القانون ← الإسقاط والمعادلة ← الحل بالشروط البدئية ← التطبيق العددي بالوحدات ← الاستنتاج. حفظ هاد السلسلة وطبقها فأي تمرين، والمصحح غادي يعطيك نقاط المراحل وخا تغلط فالحساب!

## 2. Les 3 tueurs de points : unités, chiffres significatifs, homogénéité

- **Unités SI obligatoires dans les calculs** : $m$ (pas km !), $kg$, $s$, $A$, $V$, $F$, $H$, $mol\cdot L^{-1}$ ou $mol\cdot m^{-3}$ (attention aux conversions $1\,L = 10^{-3}\,m^3$ !). Convertir **avant** de calculer.
- **Conversions pièges** : $km/h \to m/s$ ($\div 3,6$), $cm \to m$, $mS/cm$, $g \to kg$, $min \to s$, $keV/MeV \to J$ ($\times 1,6\times10^{-19}$ / $\times 1,6\times10^{-13}$), $u \to kg$ ($1\,u = 1,66\times10^{-27}\,kg$).
- **Chiffres significatifs** : le résultat a autant de CS que la donnée la moins précise (souvent 2-3). $g = 9,8$ (2 CS) → pas de résultat à 5 CS !
- **Homogénéité** : vérifier que chaque terme d'une équation a la même unité (ex. $RC$ en secondes : $[R][C] = \Omega\cdot F = s$ ✔). Une EDP inhomogène = erreur certaine.

## 3. Réflexes par domaine (check-list examen)

**Mécanique (Newton)** : schéma des forces **avant** le PFD ; axes orientés ; conditions initiales lues dans l'énoncé ($v_0$, $\alpha$, $h$) ; projectile : $a_x = 0$, $a_y = -g$ → primitiver 2 fois ; satellites : $a_n = v^2/r$, mouvement uniforme + Kepler $T^2/r^3 = cte$.

**Électricité (RC/RL/RLC)** : orienter mailles et flèches ; écrire la loi des mailles avec **signes cohérents** ; EDP sous forme canonique ($\frac{du}{dt} + \frac{u}{\tau} = ...$) ; **continuités** : $u_C$ continue, $i_L$ continue (conditions initiales !) ; $\tau$ = temps caractéristique (lecture graphique : 63 % / 37 %) ; énergie : condensateur $\frac{1}{2}Cu^2$, bobine $\frac{1}{2}Li^2$.

**Ondes** : retard $\tau = \frac{d}{v}$ ; périodicité $\lambda = vT = v/f$ ; 2 points en phase si $d = k\lambda$ ; savoir lire $T$ (balayage horizontal) et amplitude sur un oscillogramme.

**Nucléaire** : conservation de $A$ et $Z$ (désintégrations $\alpha$, $\beta^-$, $\beta^+$) ; loi $N = N_0e^{-\lambda t}$, $A = \lambda N$, $t_{1/2} = \ln 2/\lambda$ ; énergie : $E = |\Delta m|c^2$ avec **masses en kg** (ou $1\,u = 931,5\,MeV/c^2$ en raccourci).

**Chimie** : tableau d'avancement **systématique** ; $Q_r$ vs $K$ ($<$ : sens direct, $>$ : sens inverse, $=$ : équilibre) ; pH : $pH = -\log[H_3O^+]$ ; dosage : repérer l'équivalence (saut de pH / indicateur), $C_AV_A = C_BV_B$ (stœchiométrie 1-1) ; piles : anode = oxydation ($-$), cathode = réduction ($+$), électrons $-\to+$ à l'extérieur ; électrolyse : c'est le générateur qui impose (anode reliée au $+$).

## 4. Erreurs top 10 vues dans les copies

1. Oublier le système/référentiel ou le bilan avant le PFD. 2. Signes faux dans la loi des mailles (flèches non respectées). 3. Projeter sans définir/orienter les axes. 4. Conditions initiales oubliées ($u_C(0^+)=u_C(0^-)$, $v(0)$...). 5. AN sans conversion ($km$, $cm$, $g$, $MeV$ utilisés tels quels !). 6. Unités manquantes ou fausses dans le résultat. 7. Confondre $T$ (période), $f$, $\lambda$, $\tau$ (retard/constante de temps) — 4 symboles, 4 sens ! 8. $Q_r$ calculé avec des concentrations à l'état final au lieu de l'état initial (critère d'évolution). 9. Anode/cathode inversées entre pile et électrolyseur. 10. Copier les constantes de mémoire au lieu de celles du sujet (valeurs parfois arrondies différemment !).

## 5. Schémas et courbes (points « gratuits »)

- Tout schéma : titre, éléments légendés, flèches/sens, échelles si graphe. Un oscillogramme/exploitation de courbe **décrit en mots** : « la tension monte rapidement puis sature vers $E$ : charge du condensateur, régime transitoire de durée $\sim 5\tau$ ».
- En mécanique : forces dessinées **au centre d'inertie** (sauf couples), longueurs proportionnelles aux intensités quand c'est demandé.

## 6. Gestion des 3 heures (plan de bataille)

| Bloc | Temps | Conseil |
|---|---|---|
| Lecture totale + ordre perso | 10 min | Repérer l'exercice « cadeau » (souvent nucléaire/ondes/QCM de cours) |
| Exercice cadeau + chimie facile | 35-40 min | Verrouiller ~6-8 pts vite |
| Mécanique (le gros) | 50-60 min | PFD complet, ne pas se noyer : admettre un résultat et continuer si bloqué |
| Électricité / 2e physique | 35-40 min | EDP + courbes + AN soignées |
| Fin chimie + relecture unités | 25-30 min | Traquer : conversions, CS, signes, encadrés |

> بالدارجة: بدا بالساهل باش تجمع النقاط وتدخل فالتركيز، والميكانيك عطيها حقها من الوقت حيت هي الأطول. والقاعدة المقدسة: **أي عدد بلا وحدة = ناقص!** والوحدات خاصهم يكونو بالنظام العالمي قبل الحساب — الكيلومتر والسنتيمتر والغرام كيتحولو فالأول، ماشي فاللخر!

*Fiches réflexes détaillées par chapitre : voir `EXERCICES_TYPES.md` de chaque chapitre (Phase 2-4).*
