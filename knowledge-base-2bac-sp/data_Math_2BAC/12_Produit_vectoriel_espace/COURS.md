---
chapitre: "12 - Produit vectoriel dans l'espace"
unite: "S3 - Géométrie dans l'espace"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2025 Normale Ex.1 Q3 (réel, SP : produit vectoriel vers plan) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 12 — Produit vectoriel dans l'espace

> 📋 **Exigible au bac** : $\vec{u} \wedge \vec{v}$ = vecteur $\perp$ à $\vec{u}$ et $\vec{v}$, de norme $|\vec{u}||\vec{v}||\sin\theta|$ (aire !) ; calcul par déterminants $2\times2$ ; $\vec{v} \wedge \vec{u} = -\vec{u} \wedge \vec{v}$ ; $\vec{u} \wedge \vec{u} = \vec{0}$ ; applications : normal à un plan, aire ($|\vec{u} \wedge \vec{v}|/2$ pour un triangle), test de colinéarité.

## 1. Accroche — la porte et son gond 🚪

Une porte tourne autour de son gond : le gond est **perpendiculaire** au plan de la porte, et son « efficacité » dépend de l'angle (pousser face à la porte ne sert à rien). Le produit vectoriel $\vec{u} \wedge \vec{v}$, c'est le gond fabriqué à partir de deux vecteurs : **perpendiculaire aux deux**, avec une norme = **l'aire** qu'ils engendrent (nulle s'ils sont alignés — pas de porte sans angle !). Et le chapitre 11 réclamait des normaux : **le produit vectoriel en est l'usine.**

> بالدارجة : الجداء المتجهي $\vec{u} \wedge \vec{v}$ = **المفصلة** المصنوعة من متجهين : **عمودية عليهما بجوج**، والمنظم ديالها = **المساحة** اللي كيكْوّنوها (صفر إلا كانو على خط واحد — ما كايناش باب بلا زاوية !). والفصل 11 كان كيطلب النواظم : **الجداء المتجهي هو المصنع ديالهم.**

## 2. Résumé du cours (exigible au bac)

**Définition (3 ingrédients).** $\vec{w} = \vec{u} \wedge \vec{v}$ est LE vecteur tel que : ① **direction** : $\perp$ à $\vec{u}$ ET à $\vec{v}$ ; ② **norme** : $\boxed{\|\vec{u} \wedge \vec{v}\| = \|\vec{u}\|\|\vec{v}\||\sin\theta|}$ (= aire du parallélogramme construit sur $\vec{u}$, $\vec{v}$) ; ③ **sens** : $(\vec{u}, \vec{v}, \vec{w})$ direct (règle de la main droite : index $\vec{u}$, majeur $\vec{v}$, pouce $\vec{w}$). Si $\vec{u} \parallel \vec{v}$ : $\vec{u} \wedge \vec{v} = \vec{0}$ (pas d'aire, pas de perpendiculaire privilégiée).

**Calcul (coordonnées).** $\vec{u}(x,y,z)$, $\vec{v}(x',y',z')$ : $\boxed{\vec{u} \wedge \vec{v} = \begin{pmatrix} yz' - zy' \\ zx' - xz' \\ xy' - yx' \end{pmatrix}}$ — chaque composante = un déterminant $2\times2$ (barrer une ligne, multiplier en croix avec le bon signe : $+,-,+$). **Vérification obligatoire** : tester $\vec{w}\cdot\vec{u} = 0$ et $\vec{w}\cdot\vec{v} = 0$ (M11 !) — 20 secondes qui valident tout le calcul.

**Propriétés.** $\boxed{\vec{v} \wedge \vec{u} = -\vec{u} \wedge \vec{v}}$ (**antisymétrie** : l'ordre compte !) ; $\boxed{\vec{u} \wedge \vec{u} = \vec{0}}$ ; bilinéarité ($(\alpha\vec{u}) \wedge \vec{v} = \alpha(\vec{u} \wedge \vec{v})$, distributivité). Base directe : $\vec{i} \wedge \vec{j} = \vec{k}$, $\vec{j} \wedge \vec{k} = \vec{i}$, $\vec{k} \wedge \vec{i} = \vec{j}$ (cycle $i \to j \to k \to i$ ; sens inverse = signe $-$).

**Applications (cœur du bac).** ① **Normal à un plan** : plan dirigé par $\vec{u}$, $\vec{v}$ (non colinéaires) → $\vec{n} = \vec{u} \wedge \vec{v}$ est normal → équation via M11 ! ② **Aire** : parallélogramme $= \|\vec{u} \wedge \vec{v}\|$, **triangle** $ABC = \frac{1}{2}\|\overrightarrow{AB} \wedge \overrightarrow{AC}\|$. ③ **Colinéarité** : $\vec{u} \parallel \vec{v} \iff \vec{u} \wedge \vec{v} = \vec{0}$ (test propre, mieux que la proportionnalité en 3D).

**Repère important :** scalaire = NOMBRE ($\vec{u}\cdot\vec{v} \in \mathbb{R}$, M11) ; vectoriel = VECTEUR ($\vec{u} \wedge \vec{v}$ a 3 composantes). Ne jamais les mélanger : $\vec{u}\cdot\vec{v}$ n'a pas de direction, $\vec{u} \wedge \vec{v}$ n'est pas un nombre.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**التعريف (3 مكونات) :** $\vec{w} = \vec{u} \wedge \vec{v}$ هو المتجه اللي : ① **الاتجاه** : عمودي على $\vec{u}$ **و** $\vec{v}$ ؛ ② **المنظم** : $\|\vec{u} \wedge \vec{v}\| = \|\vec{u}\|\|\vec{v}\||\sin\theta|$ (= مساحة متوازي الأضلاع) ؛ ③ **المنحى** : $(\vec{u}, \vec{v}, \vec{w})$ مباشر (قاعدة اليد اليمنى). إلا كانو متوازيين : الجداء = $\vec{0}$ (لا مساحة، لا عمودي مميز).

**الحساب (بالإحداثيات) :** $\vec{u} \wedge \vec{v} = (yz' - zy', zx' - xz', xy' - yx')$ — كل مركبة = محدد $2\times2$ (حيّد سطر، ضرب عكسي بالإشارة : $+,-,+$). **التحقق إجباري** : جرّب $\vec{w}\cdot\vec{u} = 0$ و $\vec{w}\cdot\vec{v} = 0$ (M11 !) — 20 ثانية كتصحح كلشي.

**الخواص :** $\vec{v} \wedge \vec{u} = -\vec{u} \wedge \vec{v}$ (**قلب الإشارة : الترتيب مهم !**) ؛ $\vec{u} \wedge \vec{u} = \vec{0}$ ؛ التوزيعية. القاعدة المباشرة : $\vec{i} \wedge \vec{j} = \vec{k}$، $\vec{j} \wedge \vec{k} = \vec{i}$، $\vec{k} \wedge \vec{i} = \vec{j}$ (الدورة $i \to j \to k$ ؛ العكس = ناقص).

**التطبيقات (قلب الباك) :** ① **ناظم المستوى** : مستوى موجَّه بـ $\vec{u}$، $\vec{v}$ ← $\vec{n} = \vec{u} \wedge \vec{v}$ ناظم ← المعادلة عبر M11 ! ② **المساحة** : متوازي الأضلاع $= \|\vec{u} \wedge \vec{v}\|$، **المثلث** $= \frac{1}{2}\|\overrightarrow{AB} \wedge \overrightarrow{AC}\|$. ③ **الارتباط الخطي** : متوازيان $\iff$ الجداء $= \vec{0}$.

**الفرق الحاسم :** السلمي = **عدد** ؛ المتجهي = **متجه** (3 مركبات). ما تخلطهومش أبداً !

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — شنو كيعطيك ؟ متجه عمودي + مساحة.** $\vec{u} \wedge \vec{v}$ : سول راسك جوج أسئلة : «شكون العمودي عليهما بجوج ؟» (الاتجاه) و «شحال المساحة اللي بيناتهما ؟» (المنظم). إلا كانو على نفس الخط : الجواب $\vec{0}$ (لا عمودي مميز ولا مساحة).

**الخطوة 2 — الحساب : احفظ النمط $+,-,+$.** $\vec{u}(1,2,3)$، $\vec{v}(4,5,6)$ : المركبة 1 : $(2\times6 - 3\times5) = -3$ ؛ المركبة 2 : $(3\times4 - 1\times6) = 6$ ؛ المركبة 3 : $(1\times5 - 2\times4) = -3$. النتيجة $(-3,6,-3)$. **ومن بعد تحقق** : $(-3,6,-3)\cdot(1,2,3) = -3+12-9 = 0$ ✓ و $(-3,6,-3)\cdot(4,5,6) = -12+30-18 = 0$ ✓. التحقق هو نصف التمرين !

**الخطوة 3 — الاستعمال 1 : الناظم (الجسر مع M11).** مستوى معرّف بثلاث نقط $A, B, C$ ؟ حسب $\overrightarrow{AB} \wedge \overrightarrow{AC}$ ← ناظم ← معادلة $ax+by+cz+d = 0$ ← عوّض $A$. **هاد السلسلة (متجهي ← ناظم ← معادلة) هي أكثر سؤال تكراراً في الوطني.**

**الخطوة 4 — الاستعمال 2 : المساحة.** مساحة المثلث $ABC$ : $\frac{1}{2}\|\overrightarrow{AB} \wedge \overrightarrow{AC}\|$. نسى $\frac{1}{2}$ = الجواب مضروب في 2 = غالط. **القاعدة : متوازي الأضلاع كامل، المثلث النص.**

**الخطوة 5 — الفخ الوحيد : الترتيب.** $\vec{v} \wedge \vec{u} = -\vec{u} \wedge \vec{v}$ (عكس المنحى !). للمساحة ما كيهمّش (المنظم كيحيّد الإشارة)، ولكن للناظم الموجَّه (المسافة بإشارة، التوجيه) كيهمّ. **القاعدة : احترم الترتيب اللي عطاه التمرين.**

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Produit vectoriel | الجداء المتجهي | vecteur $\perp$ aux 2, norme = aire |
| Antisymétrie | قلب الإشارة | $\vec{v} \wedge \vec{u} = -\vec{u} \wedge \vec{v}$ |
| $\vec{u} \wedge \vec{u} = \vec{0}$ | الجداء مع النفس | nul (colinéaires !) |
| Main droite | اليد اليمنى | $(\vec{u}, \vec{v}, \vec{w})$ direct |
| Normal via $\wedge$ | الناظم بالجداء | 2 directeurs → 1 normal (→ M11) |
| Aire triangle | مساحة المثلث | $\frac{1}{2}\|\overrightarrow{AB} \wedge \overrightarrow{AC}\|$ |
| Test $\parallel$ | اختبار التوازي | $\vec{u} \wedge \vec{v} = \vec{0}$ |

## 6. FAQ du chapitre

**1. Pourquoi $+,-,+$ dans le calcul ?** Ce sont les signes du développement d'un déterminant $3\times3$ (alternés). Astuce : 1ʳᵉ et 3ᵉ composantes « directes », 2ᵉ inversée. / إشارات نشر المحدد : الأولى والثالثة مباشرتان، الثانية معكوسة.

**2. $\vec{u} \wedge \vec{v} = \vec{0}$ : que conclure ?** $\vec{u}$ et $\vec{v}$ colinéaires (ou l'un nul). C'est LE test de parallélisme en 3D. / متوازيان (ولا واحد منعدم) — هو اختبار التوازي في الفضاء.

**3. Ordre des vecteurs pour le normal ?** $\overrightarrow{AB} \wedge \overrightarrow{AC}$ ou l'inverse : les deux sont normaux (opposés) — l'équation du plan est la même (à un facteur $-1$ près). / بجوج نواظم (متعاكسان) — نفس المعادلة (حتى $-1$).

**4. Aire ou norme, quelle différence ?** $\|\vec{u} \wedge \vec{v}\|$ = aire du PARALLÉLOGRAMME ; le triangle = moitié. / المنظم = مساحة متوازي الأضلاع ؛ المثلث = النص.

**5. Pourquoi vérifier avec le scalaire ?** Par définition $\vec{w} \perp \vec{u}$ et $\vec{w} \perp \vec{v}$ : si les scalaires ne sont pas nuls, le calcul est faux. Test gratuit et total. / بالتعريف $\vec{w}$ عمودي عليهما : إلا ما خرجش الصفر، الحساب غالط.

**6. Lien physique ?** Moment $\vec{M} = \overrightarrow{OM} \wedge \vec{F}$ (rotation !), force de Lorentz $\vec{F} = q\vec{v} \wedge \vec{B}$. La porte et son gond, partout en PC. / العزم ولورنتز : الباب والمفصلة في كل الفيزياء.

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **Scalaire vs vectoriel** : $\vec{u}\cdot\vec{v}$ = nombre ; $\vec{u} \wedge \vec{v}$ = vecteur. « Calculer $\vec{u} \wedge \vec{v}$ » → 3 composantes, pas un nombre !
- 🪤 **2ᵉ composante : signe inversé** : $zx' - xz'$ (pas $xz' - zx'$ !). Le $-$ du $+,-,+$ frappe la 2ᵉ. Vérifier par les scalaires !
- 🪤 **$1/2$ oublié (aire triangle)** : $\|\vec{u} \wedge \vec{v}\|$ seul = parallélogramme. Triangle → diviser par 2.
- 🪤 **$\vec{u} \wedge \vec{v} = \vec{v} \wedge \vec{u}$** : FAUX ($= -$). L'ordre compte — seul le scalaire est symétrique.
- Mots-clés : *$\perp$ aux deux, norme = aire, $+,-,+$, vérifier par scalaire nul, normal → équation (M11).*

## 8. Sources de ce chapitre

- National Maths SX 2025 Normale Ex.1 Q3 (réel, SP) : produit vectoriel vers plan mx+2y+mz-2m = 0 — https://etude-generale.com/correction-dexamen-national-2025-math-science-physique/ ; + synthèse prof ; pont M11.

## 9. Le « pourquoi » profond — pourquoi un vecteur perpendiculaire 🔬

**Pourquoi la norme vaut-elle l'aire ?** $\|\vec{u}\|\|\vec{v}\||\sin\theta|$ = (base $\|\vec{u}\|$) × (hauteur $\|\vec{v}\||\sin\theta|$) : c'est exactement base × hauteur du parallélogramme. Le produit vectoriel n'est pas un calcul arbitraire : **c'est l'aire faite vecteur** (avec la direction qui manquait à l'aire : la perpendiculaire).

**Pourquoi l'antisymétrie ($\vec{v} \wedge \vec{u} = -\vec{u} \wedge \vec{v}$) ?** Parce que l'orientation compte : $(\vec{u}, \vec{v}, \vec{w})$ doit rester direct. Échanger $\vec{u}$ et $\vec{v}$ retourne l'orientation (miroir) → $\vec{w}$ doit se retourner pour compenser. C'est la même raison qui fait tourner une porte dans un sens ou l'autre selon le côté où on pousse.

**Pourquoi $\vec{u} \wedge \vec{u} = \vec{0}$ ?** Deux raisons qui coïncident : aire nulle ($\sin 0 = 0$) ET perpendiculaire indéterminée (tout vecteur $\perp$ à $\vec{u}$ conviendrait — le seul choix canonique est $\vec{0}$). Cette double nullité fait du produit vectoriel un **détecteur d'alignement** : non-nul = vraiment 2D (un plan !), nul = aplati sur une droite.

**Liens croisés :** M11 — $\wedge$ fabrique les normaux dont M11 a besoin (usine → consommateur) ; déterminants $2\times2$ (1BAC) : le calcul n'est que 3 déterminants ; PC — moment d'une force, Lorentz, Laplace : tous les effets « tournants » sont des produits vectoriels ; M06/M08 — $|a-b|$ et arguments : distances et angles, même combat en complexes.

## 10. Les 3 confusions qui coûtent des points 😵

**1. « $\vec{u} \wedge \vec{v} = 12$. »** Un nombre ! Impossible : le produit vectoriel est un VECTEUR (3 composantes). **Le déclic :** *$\cdot$ (point) = nombre ; $\wedge$ (chapeau) = vecteur qui « sort ».* Si ta réponse n'a pas 3 composantes, tu as calculé un scalaire.

**2. « 2ᵉ composante : $xz' - zx'$. »** Le signe ! C'est $zx' - xz'$. **Le déclic :** récite *« $+$, $-$, $+$ »* en écrivant les 3 composantes, puis **vérifie** par les 2 scalaires — l'erreur de signe échoue toujours au test.

**3. « Aire du triangle $= \|\vec{u} \wedge \vec{v}\|$. »** Oubli du $1/2$ : c'est l'aire du parallélogramme ENTIER. **Le déclic :** dessine le parallélogramme et sa diagonale : le triangle n'en est que la moitié — *qui dit triangle dit moitié.*

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** déterminants $2\times2$ (1BAC : $ad - bc$), produit scalaire M11 (la vérification !), vecteurs-coordonnées. **Test 30 s :** $\begin{vmatrix} 2 & 1 \\ 3 & 4 \end{vmatrix} = 8 - 3 = 5$ ; $(1,2,3)\cdot(4,5,6) = 4+10+18 = 32$.

**Plan B — le plus dur (le calcul sans erreur de signe) :** écris $\vec{u}$ et $\vec{v}$ en colonnes, barre mentalement la ligne 1 → $yz' - zy'$ ; ligne 2 → **inverse** ($zx' - xz'$) ; ligne 3 → $xy' - yx'$. Puis TEST : les 2 scalaires doivent être nuls. Non nuls ? Erreur de signe (90 % : la 2ᵉ composante) → recorriger avant de continuer.

**Fiche réflexes :** *vecteur $\perp$ + norme = aire · $+,-,+$ · vérifier par scalaire nul · 2 directeurs → normal → M11 · triangle = moitié.*
