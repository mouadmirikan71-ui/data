---
chapitre: "11 - Produit scalaire dans l'espace"
unite: "S3 - Géométrie dans l'espace"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2025 Normale Ex.1 Q1+Q2+Q4 (réel, SP : sphère, section plane) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 11 — Produit scalaire dans l'espace

> 📋 **Exigible au bac** : $\vec{u}\cdot\vec{v} = xx' + yy' + zz'$ ; $\|\vec{u}\| = \sqrt{x^2+y^2+z^2}$ ; orthogonalité $\iff$ scalaire nul ; plan : $\vec{n}\cdot\overrightarrow{AM} = 0 \iff ax+by+cz+d = 0$ ; distance point-plan $\frac{|ax_0+by_0+cz_0+d|}{\sqrt{a^2+b^2+c^2}}$ ; sphère $(x-a)^2+(y-b)^2+(z-c)^2 = R^2$.

## 1. Accroche — l'ombre et le mur 🌞

Le soleil projette ton ombre sur un mur : l'ombre mesure « combien de toi va vers le mur ». Le produit scalaire, c'est ça : **combien un vecteur va dans la direction d'un autre**. Et un plan ? C'est un mur : tous les points $M$ tels que $\overrightarrow{AM}$ ne va PAS du tout vers le vecteur normal $\vec{n}$ (scalaire = 0). **Équation de plan = une orthogonalité déguisée.** Tout le chapitre découle de cette phrase.

> بالدارجة : الجداء السلمي = **«شحال متجه غادي في اتجاه متجه آخر»** (بحال الظل على الحيط). والمستوى ؟ هو حيط : كاع النقط $M$ اللي $\overrightarrow{AM}$ ما غاديش قاع نحو الناظم $\vec{n}$ (الجداء = 0). **معادلة المستوى = تعامد متنكر.** كاع الفصل خارج من هاد الجملة.

## 2. Résumé du cours (exigible au bac)

**Produit scalaire (coordonnées).** Dans un repère orthonormé : $\boxed{\vec{u}\cdot\vec{v} = xx' + yy' + zz'}$. Propriétés : symétrie, bilinéarité ($\vec{u}\cdot(\alpha\vec{v}+\beta\vec{w}) = \alpha\,\vec{u}\cdot\vec{v} + \beta\,\vec{u}\cdot\vec{w}$), $\vec{u}\cdot\vec{u} = \|\vec{u}\|^2$. **Norme :** $\boxed{\|\vec{u}\| = \sqrt{x^2+y^2+z^2}}$ ; distance $AB = \|\overrightarrow{AB}\|$. **Orthogonalité :** $\boxed{\vec{u} \perp \vec{v} \iff \vec{u}\cdot\vec{v} = 0}$ (vecteurs non nuls).

**Équation cartésienne de plan.** Plan $P$ passant par $A(x_A,y_A,z_A)$, de vecteur normal $\vec{n}(a,b,c)$ : $M(x,y,z) \in P \iff \vec{n}\cdot\overrightarrow{AM} = 0 \iff \boxed{ax+by+cz+d = 0}$ où $d = -(ax_A+by_A+cz_A)$. **Lire à l'envers** : face à $2x - y + 3z - 5 = 0$, le normal est $\vec{n}(2,-1,3)$ (les coefficients !). **Recette** : normal $\vec{n}$ + point $A$ → écrire $ax+by+cz+d = 0$, injecter $A$ → $d$.

**Positions de plans.** $P \parallel P'$ $\iff$ normaux **colinéaires** ; $P \perp P'$ $\iff$ normaux **orthogonaux** (scalaire nul). Droite $\parallel$ plan $\iff$ vecteur directeur $\perp$ normal du plan. Droite $\perp$ plan $\iff$ directeur colinéaire au normal.

**Distance point-plan.** $\boxed{d(A, P) = \frac{|ax_A+by_A+cz_A+d|}{\sqrt{a^2+b^2+c^2}}}$ — le numérateur = « injecter $A$ dans l'équation », le dénominateur = norme du normal. Cas d'école : distance d'un centre à un plan tangent.

**Sphère.** Centre $\Omega(a,b,c)$, rayon $R$ : $\boxed{(x-a)^2+(y-b)^2+(z-c)^2 = R^2}$. **Forme développée** : $x^2+y^2+z^2+ux+vy+wz+k = 0$ → **compléter les carrés** pour retrouver centre et rayon (ex : $x^2 - 4x = (x-2)^2 - 4$). Attention : pas toujours une sphère (rayon² doit être $> 0$ !). Plan tangent en $T$ : plan de normal $\overrightarrow{\Omega T}$ passant par $T$. **Section plane** : $P$ coupe $S$ selon $d = d(centre,P)$ : $d > R$ donne vide ; $d = R$ donne un point (tangent) ; $d < R$ donne un **cercle** de rayon $r$ avec $r^2 = R^2-d^2$ (centre = projete du centre sur $P$).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الجداء السلمي (بالإحداثيات) :** $\vec{u}\cdot\vec{v} = xx' + yy' + zz'$. الخواص : التناظر، التوزيعية. **المنظم :** $\|\vec{u}\| = \sqrt{x^2+y^2+z^2}$ ؛ المسافة $AB = \|\overrightarrow{AB}\|$. **التعامد :** $\vec{u} \perp \vec{v} \iff \vec{u}\cdot\vec{v} = 0$.

**المعادلة الديكارتية للمستوى :** المستوى المارّ من $A$ بالناظم $\vec{n}(a,b,c)$ : $\vec{n}\cdot\overrightarrow{AM} = 0 \iff \boxed{ax+by+cz+d = 0}$ حيث $d = -(ax_A+by_A+cz_A)$. **القراءة المعاكسة** : قدام $2x - y + 3z - 5 = 0$ الناظم هو $(2,-1,3)$ (المعاملات نيشان !). **الوصفة** : الناظم + النقطة ← كتب المعادلة ← عوّض النقطة ← $d$.

**أوضاع المستويات :** متوازيين $\iff$ الناظمان **مرتبطان خطياً** ؛ متعامدين $\iff$ الناظمان **متعامدان** (الجداء صفر). مستقيم $\parallel$ مستوى $\iff$ الموجه $\perp$ الناظم. مستقيم $\perp$ مستوى $\iff$ الموجه مرتبط بالناظم.

**المسافة نقطة-مستوى :** $\boxed{d = \frac{|ax_A+by_A+cz_A+d|}{\sqrt{a^2+b^2+c^2}}}$ — البسط = «عوّض $A$ في المعادلة»، المقام = منظم الناظم.

**الكرة :** المركز $\Omega(a,b,c)$ والشعاع $R$ : $\boxed{(x-a)^2+(y-b)^2+(z-c)^2 = R^2}$. **الشكل المنشور** : كمّل المربعات باش تلقى المركز والشعاع ($x^2 - 4x = (x-2)^2 - 4$). ردّ البال : ماشي ديما كرة (مربع الشعاع خاصو يكون $> 0$ !). المستوى المماس في $T$ : الناظم $\overrightarrow{\Omega T}$ والمارّ من $T$.

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — الجداء السلمي : آلة التعامد.** نسى الصيغة المعقدة : في الفضاء، $\vec{u}\cdot\vec{v} = xx'+yy'+zz'$ (ضرب متناظر وجمّع). السؤال الوحيد اللي كيجاوب عليه : **«واش متعامدين ؟»** — إلا خرج 0، إيه. كاع التمارين : حسابات بسيطة + السؤال السحري «= 0 ؟».

**الخطوة 2 — المستوى : ناظم + نقطة = معادلة.** عطاوك الناظم $\vec{n}(1,2,-1)$ والنقطة $A(0,1,3)$ ؟ كتب : $x + 2y - z + d = 0$ (المعاملات = الناظم !). عوّض $A$ : $0 + 2 - 3 + d = 0$ ← $d = 1$. صافي : $x + 2y - z + 1 = 0$. **هادي هي الوصفة الكاملة — 90% من الأسئلة.**

**الخطوة 3 — منين نجيب الناظم ؟** من المعادلة (المعاملات نيشان)، ولا من المسألة («المستوى العمودي على $(AB)$» ← الناظم = $\overrightarrow{AB}$)، ولا من الجداء المتجهي (M12 : ناظم من متجهين). **أي سؤال مستوى كيبدا بـ : «شكون هو الناظم ؟»**

**الخطوة 4 — المسافة : عوّض وقسّم.** $d(A, P)$ : عوّض إحداثيات $A$ في $ax+by+cz+d$ (القيمة المطلقة !) وقسّم على $\sqrt{a^2+b^2+c^2}$. مثال : $d(O, 2x-y+3z-5=0) = \frac{|-5|}{\sqrt{4+1+9}} = \frac{5}{\sqrt{14}}$. الغلطة الوحيدة الممكنة : نسى الجذر ولا القيمة المطلقة.

**الخطوة 5 — الكرة : كمّل المربع.** شفتي $x^2+y^2+z^2-4x+2y-4 = 0$ ؟ جمّع : $(x^2-4x) + (y^2+2y) + z^2 = 4$ ← $(x-2)^2 - 4 + (y+1)^2 - 1 + z^2 = 4$ ← $(x-2)^2+(y+1)^2+z^2 = 9$ ← المركز $(2,-1,0)$ والشعاع $3$. **تكميل المربع = المهارة الوحيدة.**

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Produit scalaire | الجداء السلمي | $xx'+yy'+zz'$ (nombre !) |
| Norme | المنظم | $\|\vec{u}\| = \sqrt{x^2+y^2+z^2}$ |
| Orthogonalité | التعامد | scalaire $= 0$ |
| Vecteur normal | الناظم | $\perp$ au plan (coefficients de l'équation) |
| Équation $ax+by+cz+d = 0$ | معادلة المستوى | normal $(a,b,c)$ + point → $d$ |
| Distance point-plan | المسافة نقطة-مستوى | $|inj|/\|\vec{n}\|$ |
| Sphère | الكرة | centre + rayon (carrés complétés) |
| Plan tangent | المستوى المماس | normal $\overrightarrow{\Omega T}$ en $T$ |

## 6. FAQ du chapitre

**1. Pourquoi les coefficients $(a,b,c)$ sont-ils le normal ?** $ax+by+cz+d = 0$ se réécrit $\vec{n}\cdot\overrightarrow{OM} = -d$ avec $\vec{n}(a,b,c)$ : l'équation DIT que le scalaire avec $\vec{n}$ est constant → $\vec{n}$ est normal. / المعادلة كتقول أن الجداء مع $\vec{n}$ ثابت ← $\vec{n}$ ناظم.

**2. Plan par 3 points non alignés ?** Deux méthodes : système (injecter les 3 points, résoudre), ou normal via produit vectoriel $\overrightarrow{AB} \wedge \overrightarrow{AC}$ (M12) + un point. / جوج طرق : الجملة، ولا الناظم بالجداء المتجهي + نقطة.

**3. $P \parallel P'$ ou confondus ?** Normaux colinéaires → parallèles ; tester un point de l'un dans l'autre → confondus ou strictement parallèles. / الناظمان مرتبطان ← متوازيان ؛ جرّب نقطة ← منطبقان ولا متوازيان تماماً.

**4. Distance : pourquoi $|~|$ et $\sqrt{}$ ?** $|~|$ : une distance est positive. $\sqrt{a^2+b^2+c^2}$ : on divise par la norme du normal (projection !). / القيمة المطلقة : المسافة موجبة. الجذر : القسمة على منظم الناظم (الإسقاط !).

**5. Sphère ou pas ?** Après carrés complétés, $R^2 > 0$ → sphère ; $R^2 = 0$ → un point ; $R^2 < 0$ → ensemble vide ! / $R^2 > 0$ ← كرة ؛ $= 0$ ← نقطة ؛ $< 0$ ← فارغ !

**6. Lien avec la physique ?** Travail $W = \vec{F}\cdot\vec{d}$ (P-méca) : le scalaire mesure « combien de force va dans le déplacement ». Même objet, deux mondes. / الشغل $W = \vec{F}\cdot\vec{d}$ : نفس المفهوم في الفيزياء.

**7. Que donne sphère et plan ?** Comparer $d$ à $R$ : $d > R$ donne vide ; $d = R$ donne point de tangence ; $d < R$ donne cercle ($r^2 = R^2-d^2$, centre = projeté du centre). Cas 2025N : $r^2 = 2+4/(m^2+2)$.

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **Normal vs directeur** : le normal sort du plan ($\perp$), le directeur est couché dedans. « Plan dirigé par $\vec{u}$ » → $\vec{u}$ N'EST PAS le normal !
- 🪤 **$d$ calculé faux** : $d = -(ax_A+by_A+cz_A)$ — injecter le point CORRECTEMENT (signes !). Vérifier : $A$ doit satisfaire l'équation.
- 🪤 **Distance sans $\sqrt{}$ ni $|~|$** : les deux sont obligatoires. $5/14$ au lieu de $5/\sqrt{14}$ = faux.
- 🪤 **Centre de sphère : signes inversés** : $(x-2)^2$ → $x_\Omega = +2$ (« moins donne plus »). $(x+1)^2$ → $-1$.
- Mots-clés : *scalaire nul = orthogonalité, coefficients = normal, injecter le point, $|inj|/\|n\|$, compléter les carrés.*

## 8. Sources de ce chapitre

- National Maths SX 2025 Normale Ex.1 (réel, SP) : sphère x2+y2+z2 = 4, section r2 = 2+4/(m2+2) — https://etude-generale.com/correction-dexamen-national-2025-math-science-physique/ ; + synthèse prof ; vecteurs 1BAC.

## 9. Le « pourquoi » profond — pourquoi le scalaire gouverne les plans 🔬

**Pourquoi le scalaire mesure-t-il « combien va vers » ?** $\vec{u}\cdot\vec{v} = \|\vec{u}\|\|\vec{v}\|\cos\theta$ : c'est $\|\vec{u}\|$ fois la projection (signée) de $\vec{v}$ sur $\vec{u}$. $\cos\theta = 0$ ($\theta = 90°$) annule tout : l'orthogonalité = « rien ne va vers ». C'est pour ça que le physicien calcule un travail avec : seule la force DANS le déplacement travaille.

**Pourquoi l'équation du plan est-elle linéaire ($ax+by+cz+d = 0$) ?** Parce que le scalaire est linéaire (bilinéarité) : $\vec{n}\cdot\overrightarrow{AM} = 0$ se déplie en $a(x-x_A) + b(y-y_A) + c(z-z_A) = 0$ — du premier degré, toujours. Un plan = une contrainte linéaire (« une direction interdite ») ; une droite = deux contraintes (intersection de 2 plans) ; l'espace = zéro contrainte. La géométrie cartésienne, c'est du comptage de contraintes.

**Pourquoi diviser par $\|\vec{n}\|$ dans la distance ?** Injecter $A$ dans $ax+by+cz+d$ donne $\vec{n}\cdot\overrightarrow{HA}$ (où $H$ = projeté) $= \|\vec{n}\| \times AH$ (colinéaires !). Pour isoler $AH$ (la vraie distance), on divise par $\|\vec{n}\|$. La formule n'est pas magique : c'est une projection déguisée.

**Liens croisés :** M12 — le produit vectoriel FABRIQUE des normaux (2 directeurs → 1 normal) ; M06/M08 — $|a-b|$ et modules : même idée de distance ; PC — travail, flux, projections (tout scalaire est une projection) ; 1BAC — équations de droites $ax+by+c = 0$ : les plans sont la version 3D (même recette !).

## 10. Les 3 confusions qui coûtent des points 😵

**1. « Le plan est dirigé par $\vec{n}$. »** NON : $\vec{n}$ est normal ($\perp$), pas directeur (couché). **Le déclic :** *normal = clou planté dans le mur ; directeur = trait dessiné sur le mur.* « Dirigé par » → couché → pas le normal.

**2. « $P \parallel P'$ car même $d$. »** Le parallélisme se lit sur les NORMAUX (colinéaires), pas sur $d$. Deux plans $x+y+z = 1$ et $x+y+z = 5$ sont parallèles (même normal !), pas à cause du $d$. **Le déclic :** *même direction = même normal (à un facteur près) ; $d$ = la distance à l'origine, pas la direction.*

**3. « $(x-2)^2$ → centre $-2$. »** Le signe flippe : $(x - a)^2$ donne $a = +2$. **Le déclic :** demande « quelle valeur de $x$ ANNULE la parenthèse ? » ($x = 2$) — c'est elle, la coordonnée du centre.

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** vecteurs + coordonnées (1BAC : $\overrightarrow{AB} = B - A$), équations de droites $ax+by+c = 0$ (même logique), identités remarquables (carrés complétés). **Test 30 s :** $\overrightarrow{AB}$ pour $A(1,0,2)$, $B(3,1,0)$ → $(2,1,-2)$ ; $(x-3)^2$ développé → $x^2-6x+9$.

**Plan B — le plus dur (l'équation de plan en examen) :** boucle imbattable : ① « Qui est le normal ? » (énoncé / coefficients / $\overrightarrow{AB}$ / M12) ② écrire $ax+by+cz+d = 0$ ③ injecter le point → $d$ ④ **vérifier** : le point satisfait ? le normal est-il $\perp$ aux directions ? Si oui → terminé, points assurés.

**Fiche réflexes :** *scalaire $= 0$ ⟺ $\perp$ · coefficients = normal · normal + point → $d$ · distance = $|inj|/\|n\|$ · sphère : compléter les carrés.*
