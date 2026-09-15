---
chapitre: "06 - Dipole RC"
unite: "Physique S1 - Électricité"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "AlloSchool PC 2BAC SP (Dipôle RC) + Manuel Massar PC 2BAC SP + synthèse prof"
date_collecte: "2026-09-14"
type: "summary"
langues: "FR + Darija + LaTeX"
---

# Chapitre 06 — Dipôle RC

> 📋 **Exigible au bac (cadre de référence)** : Charge/décharge, EDP, $\tau = RC$, énergie $\frac{1}{2}Cu^2$, continuité de $u_C$
> *Source : `00_Programme_officiel/programme_officiel.md` (v1 — à recouper avec le PDF officiel en Phase 3).*
*(CHAPITRE MODÈLE : expérience → loi → LaTeX → Darija → pièges, même gabarit pour les 19 autres)*

## 1. Accroche — l'expérience avant la loi 🔋

**FR :** Prends un condensateur (deux plaques métalliques face à face), un résistor, un générateur et un interrupteur. À $t = 0$, tu fermes le circuit : sur l'oscilloscope, la tension $u_C$ **monte vite puis de moins en moins vite**, et sature vers $E$ (tension du générateur). Le courant, lui, **part fort puis s'éteint**. Question : pourquoi la charge ralentit-elle ? Parce que plus le condensateur se remplit, plus il « repousse » les nouvelles charges — comme un réservoir dont la pression freine le remplissage. Tout le chapitre = mettre cette observation en équations.

**بالدارجة:** تخيل خزان ديال الماء (المكثف) كتعمرو بتيو رقيق (المقاومة). فالأول الماء كيدخل بجهد، ولكن ملي الخزان كيعمر، الضغط كيطلع والتيو كيبقى يدوز غير شوية حتى كيحبس — الخزان عمر! هادشي بالضبط اللي كيوقع فالدائرة RC: التوتر $u_C$ كيطلع بسرعة فالأول ومن بعد كيتباطأ حتى كيثبت فـ $E$، والتيار كيبدا قوي ومن بعد كيموت. هاد الفصل كامل = نحولو هاد الملاحظة لمعادلات!

## 2. Résumé du cours (français + LaTeX, exigible au bac)

### 2.1 Le condensateur — définitions
- Charge : $q = C\,u_C$ ($q$ en coulombs, $C$ en farads, $u_C$ en volts).
- Courant : $i = \frac{dq}{dt}$ (en convention récepteur : $i$ entre par la borne $+$).
- Énergie stockée : $E_e = \frac{1}{2}C\,u_C^2$ (en joules).
- **Continuité** : $u_C$ ne peut pas sauter instantanément : $u_C(0^+) = u_C(0^-)$ (condition initiale !).

### 2.2 Charge du condensateur (échelon $E$, condensateur initialement vide)
- Schéma : générateur $E$ + résistor $R$ + condensateur $C$ en série, $u_C(0) = 0$.
- Loi des mailles (orientée) : $E = u_R + u_C = Ri + u_C$, avec $i = \frac{dq}{dt} = C\frac{du_C}{dt}$.
- **Équation différentielle** : $$RC\,\frac{du_C}{dt} + u_C = E$$
- Solution : $$\boxed{u_C(t) = E\left(1 - e^{-t/\tau}\right)} \quad \text{avec} \quad \boxed{\tau = RC}$$
- Courant : $i(t) = \frac{E}{R}e^{-t/\tau}$ (part de $E/R$, s'éteint).
- **Constante de temps** $\tau = RC$ (en secondes — vérifier : $\Omega\cdot F = s$ ✔) : à $t = \tau$, $u_C = 0,63\,E$ (63 %) ; régime transitoire $\approx 5\tau$, puis régime permanent ($u_C = E$, $i = 0$ : condensateur = interrupteur ouvert).

### 2.3 Décharge (condensateur chargé à $E$, branché sur $R$ seul)
- EDP : $RC\,\frac{du_C}{dt} + u_C = 0$ ; solution : $\boxed{u_C(t) = E\,e^{-t/\tau}}$.
- À $t = \tau$ : $u_C = 0,37\,E$ (37 %) ; énergie dissipée en chaleur dans $R$ (effet Joule).

### 2.4 Lecture graphique (ce que le national adore demander)
- $\tau$ = abscisse où la **tangente à l'origine** coupe l'asymptote ($E$ en charge, 0 en décharge).
- Ou : $\tau$ = temps pour atteindre 63 % de $E$ (charge) / tomber à 37 % (décharge).
- Courbe $\ln$ : en décharge, $\ln(u_C) = \ln E - t/\tau$ → droite de pente $-1/\tau$ (linéarisation !).

### 2.5 Pourquoi ça marche comme ça (le « pourquoi dans la nature »)
L'exponentielle vient du **freinage proportionnel** : la vitesse de charge $\frac{du_C}{dt}$ est proportionnelle à ce qui reste à charger ($E - u_C$). Tant qu'il reste beaucoup → vite ; quand il reste peu → lentement. C'est la même mathématique que le refroidissement, la radioactivité, la chute avec frottement : **partout où le freinage est proportionnel à l'écart restant, on trouve $e^{-t/\tau}$**.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** المكثف = **خزان الشحنات**، والمقاومة = **التيو الرقيق** اللي كيتحكم فالسرعة ديال التعمار.

1. **الشحن (La charge):** ملي كتسد الدائرة، الشحنات كيبداو يعمرو الخزان. فالأول الخزان خاوي → الماء كيدخل بجهد (تيار قوي). ملي كيعمر → الضغط كيقاوم → التيار كينقص. فاللخر الخزان عمر ($u_C = E$) والتيار حبس ($i = 0$). المعادلة $u_C = E(1-e^{-t/\tau})$ كتوصف هاد القصة بالضبط: كتبدا من 0 وكتقرب من $E$ بلا ما توصلو نظرياً!
2. **ثابت الزمن ($\tau = RC$):** هو **«مقياس الصبر»** ديال الدائرة. مقاومة كبيرة ولا مكثف كبير = تعمار بطيء = $\tau$ كبير. القاعدة العملية: بعد $5\tau$ كنعتبرو الشحن سالى (99 %).
3. **التفريغ (La décharge):** الخزان عامر وكتحل عليه التيو — الماء كيخرج بجهد فالأول ومن بعد كينقص حتى كيخوى. $u_C = Ee^{-t/\tau}$: كتبدا من $E$ وكتهبط للصفر.
4. **الطاقة:** المكثف المشحون فيه طاقة مخزونة $\frac{1}{2}Cu^2$ — بحال الخزان العالي اللي فيه طاقة الوضع. ملي كيتفرغ فالمقاومة، هاد الطاقة كتتحول لحرارة (تأثير جول).

**علاش $u_C$ ما كتقفزش؟ (الاستمرارية):** حيت القفزة فالتوتر كتعني تيار لا نهائي ($i = C\frac{du}{dt}$)، والتيار اللانهائي مستحيل فيزيائياً! إذن $u_C$ ديماً متصلة — وهادي هي اللي كتعطيك الشرط البدئي فكل تمرين.

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة + الأخطاء)*

**الخطوة 1 — شوف المنحنى قبل المعادلة.**
أي تمرين RC بدا بهاد السؤال: **المنحنى طالع (شحن) ولا هابط (تفريغ)؟** طالع من 0 لـ $E$ = شحن ($1-e^{-t/\tau}$). هابط من $E$ لـ 0 = تفريغ ($e^{-t/\tau}$). هاد التمييز بوحدو كيحل نص التمرين!

**الخطوة 2 — السلسلة الذهبية: رسم ← قانون ← معادلة ← حل ← تطبيق.**
الرسم بالأسهم ($u$, $i$) هو **الأساس** — إلا غلطتي فالاتجاه، الإشارات كيتخربو والمعادلة كتخرج غالطة. من بعد قانون العقد (mailles)، من بعد المعادلة التفاضلية بالشكل القياسي، من بعد الحل بالشرط البدئي، وفاللخر التطبيق العددي **بالوحدات العالمية** ($F$ ماشي $\mu F$ مباشرة!).

**الخطوة 3 — $\tau$ هو المفتاح.**
أي سؤال على «المدة» ولا «السرعة» الجواب فيه $\tau = RC$. ثلاثة طرق باش تجبدو: الحساب ($R\times C$)، المماس عند الأصل، ولا 63 %/37 %. تحقق ديماً: الوحدة خاصها تخرج بالثانية!

**الخطوة 4 — تشبيه واحد يعاونك فالوطني.**
**الخزان والتيو:** المكثف = الخزان، المقاومة = التيو، التوتر = مستوى الماء، التيار = صبيب الماء. تيو رقيق (R كبيرة) = تعمار بطيء. خزان كبير (C كبيرة) = تعمار بطيء. إذن $\tau = R\times C$ — المنطق كيقول أن بجوجهم كيتباطأو التعمار!

**الخطوة 5 — الأخطاء اللي كتقتل النقاط.**
- نسيان التحويل: $4,7\,\mu F = 4,7\times10^{-6}\,F$ — **الغلطة رقم 1 فالمغرب!**
- الخلط بين الشحن والتفريغ (الصيغة المعكوسة).
- نسيان الشرط البدئي ($u_C(0) = 0$ فالشحن من خزان خاوي).
- كتابة النتيجة بلا وحدة ولا بأرقام معنوية خيالية.

## 5. Définitions & formules clés (FR + Darija)

| Notion FR (LaTeX) | Énoncé FR | بالدارجة |
|---|---|---|
| Condensateur $q = Cu_C$ | Stocke des charges proportionnellement à la tension | خزان الشحنات — السعة $C$ هي الحجم ديالو |
| $\tau = RC$ | Constante de temps (s) : échelle du transitoire | مقياس الصبر — شحال كيطول التعمار |
| Charge $u_C = E(1-e^{-t/\tau})$ | Monte de 0 vers $E$ | التعمار: من الخاوي للعامر |
| Décharge $u_C = Ee^{-t/\tau}$ | Descend de $E$ vers 0 | التخوية: من العامر للخاوي |
| Continuité de $u_C$ | Pas de saut instantané de tension | المستوى ديال الماء ما كيقفزش |
| Énergie $\frac{1}{2}Cu^2$ | Énergie stockée (J) | المخزون ديال الخزان العالي |
| Régime permanent | $u_C = E$, $i = 0$ (charge finie) | الخزان عمر والتيو حبس |

## 6. FAQ du chapitre (vraies questions d'élèves)

**Q1. Pourquoi le courant s'annule en fin de charge ?**
Parce que $u_C = E$ : le condensateur « repousse » autant que le générateur « pousse » → plus de circulation. Formule : $i = C\frac{du_C}{dt}$, et $u_C$ ne varie plus → $i = 0$.
حيت الخزان عمر — الضغط الداخلي ولى قد الضغط الخارجي، ما بقى حتى تدفق.

**Q2. D'où sort le 63 % ?**
De $1 - e^{-1} \approx 0,63$ : à $t = \tau$, la charge a fait 63 % du chemin. (Décharge : $e^{-1} \approx 0,37$.)
من الحساب: $1-e^{-1} \approx 0,63$ — فاللحظة $\tau$ كتكون قطعت 63 % ديال الطريق.

**Q3. Pourquoi $5\tau$ = fin du transitoire ?**
$e^{-5} \approx 0,007$ : il reste moins de 1 % → négligeable, on considère le régime permanent atteint.
حيت $e^{-5}$ صغيرة بزاف (أقل من 1 %) — كنعتبروها صافي سالات.

**Q4. Charge ou décharge : comment décider vite ?**
Regarder $u_C(0)$ et le sens : part de 0 et monte → charge ; part de $E$ et descend → décharge. Le schéma confirme (générateur présent ou non).
شوف البداية: من 0 وطالعة = شحن، من $E$ وهابطة = تفريغ.

**Q5. Faut-il vraiment orienter le schéma ?**
**OUI.** Les signes de la loi des mailles dépendent des flèches. Sans orientation, 1 chance sur 2 de se tromper de signe.
**إيه إجباري!** الإشارات تابعين للأسهم — بلا أسهم غادي تغلط فالإشارة.

**Q6. $\mu F$, $nF$, $mH$ : comment ne pas rater les conversions ?**
Écrire la puissance de 10 **explicitement** : $4,7\,\mu F = 4,7\times10^{-6}\,F$. Vérifier $\tau$ en secondes comme contrôle.
كتب الأس صراحة وخلّي $\tau$ بالثواني كمراقبة — إلا خرجات $\tau$ بالساعات ولا بالميكروثانية، عرف راسك غلطتي!

## 7. Pièges classiques + mots-clés obligatoires ⚠️

**À écrire absolument** : schéma orienté, « d'après la loi des mailles », EDP sous forme canonique, « $u_C$ est continue donc $u_C(0^+) = ...$ », $\tau = RC$ + valeur en **s**, AN avec unités, $\boxed{\text{résultat}}$.
**Erreurs fréquentes** :
- Conversions $\mu F$/$\mu H$ oubliées ❌. - Formule de charge utilisée pour une décharge ❌.
- Signe faux dans les mailles (flèches incohérentes) ❌. - $\tau$ en ms lu comme des secondes sur le graphe ❌.
- « Le condensateur est un interrupteur ouvert » dit **pendant** le transitoire (vrai seulement en régime permanent continu !) ❌.

## 8. Sources de ce chapitre
- AlloSchool — PC 2BAC SP, section « Dipôle RC » (cours + exercices). Accès : 2026-09-14. https://www.alloschool.com/course/physique-et-chimie-2eme-bac-sciences-physiques-biof
- Manuel Massar / Fadaa PC 2BAC SP — Ch. Dipôle RC (transcription originale).
- Synthèse prof (Darija + easy-way + FAQ) : rédaction originale pour cette base, 2026-09-14.

## 9. Le « pourquoi » profond — d'où vient vraiment l'exponentielle 🔬

**Pourquoi $e^{-t/\tau}$ et pas une droite ?** Parce que la physique impose un **freinage proportionnel à l'écart restant** :
en charge, $\frac{du_C}{dt} = \frac{E - u_C}{RC}$ — la vitesse de charge est proportionnelle à « ce qui manque encore »
($E - u_C$). Or la SEULE fonction dont la dérivée est proportionnelle à elle-même (au signe près), c'est
l'exponentielle. Donc la forme $e^{-t/\tau}$ n'est pas un choix : c'est la **conséquence mathématique forcée** du
freinage proportionnel. Retiens le réflexe : « freinage $\propto$ écart restant » → exponentielle, TOUJOURS.

**Pourquoi $\tau = RC$ a la dimension d'un temps ?** Vérifie : $[R] = \frac{V}{A}$, $[C] = \frac{C}{V} = \frac{A\cdot s}{V}$
(coulomb = ampère × seconde). Donc $[RC] = \frac{V}{A}\times\frac{A\cdot s}{V} = s$ ✔. Ce n'est pas un hasard :
le produit « frein × capacité » donne toujours un temps (compare RL : $L/R$ en secondes aussi !).

**Pourquoi $u_C$ est-elle continue ? (l'argument qui tue)** L'énergie du condensateur est $\frac{1}{2}Cu_C^2$.
Un saut instantané de $u_C$ demanderait une puissance infinie ($P = \frac{dE}{dt}\to\infty$) — physiquement
impossible. Donc $u_C$ ne saute JAMAIS : c'est un argument **énergétique**, pas une convention.
(C'est aussi pour ça que $i_L$ est continu en RL : même argument avec $\frac{1}{2}Li^2$.)

**Ponts vers les autres chapitres :**
- **RL (ch.07)** : miroir parfait — $i$ joue le rôle de $u_C$, $\tau = L/R$, continuité de $i_L$. Apprends RC à fond
  et RL est gratuit à 80 %.
- **Radioactivité (ch.04)** : $N = N_0e^{-\lambda t}$ — même exponentielle, $\tau = 1/\lambda$. La « demi-vie »
  $t_{1/2} = \tau\ln 2$ existe aussi en RC mais on ne l'utilise presque jamais : méfie-toi des transferts automatiques !
- **Newton + frottement (ch.10)** : chute avec $f = kv$ → vitesse en $(1-e^{-t/\tau})$ — LITTÉRALEMENT la courbe de
  charge du condensateur. Même équation, même solution, physique différente.
- **Math (suites/EDP)** : la solution se vérifie par dérivation — c'est le pont analyse-physique du bac.

> بالدارجة: علاش الأسية ($e$)؟ حيت **الفرملة متناسبة مع اللي باقي** — ملي كيبقى بزاف كتمشي بسرعة، ملي كيبقى شوية كتمشي بشوية. الرياضيات كتقول: الدالة الوحيدة اللي المشتقة ديالها متناسبة معاها هي $e$! إذن الشكل مفروض ماشي مختار. و$\tau = RC$ بالثانية ماشي صدفة: الفرملة × السعة = الزمن، ديماً. و$u_C$ ما كتقفزش حيت القفزة كتطلب طاقة لانهائية — مستحيل!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. Charge $(1-e^{-t/\tau})$ vs décharge $(e^{-t/\tau})$ — la confusion n°1.**
*Le clic :* regarde $t = 0$ ! Charge : $u_C(0) = 0$ → il faut le $(1-\ldots)$ qui « tue » le 1 initial.
Décharge : $u_C(0) = E$ → il faut le $E\times(\ldots)$ pur qui part de $E$. **Teste toujours ta formule à $t=0$**
avant de continuer : 5 secondes qui sauvent tout l'exercice.
بالدارجة: جرب الصيغة فـ $t=0$! إلا عطاتك البداية الصحيحة (0 للشحن، $E$ للتفريغ) راه صحيحة — إلا لا، راك قالبهم!

**C2. $\tau$ vs $5\tau$ vs $t_{1/2}$ — trois temps, trois sens.**
*Le clic :* $\tau$ = temps pour faire 63 % du chemin (UN seul $\tau$) ; $5\tau$ = fin pratique du transitoire
(99 %, le « c'est fini ») ; $t_{1/2} = \tau\ln 2$ = temps de moitié — utile en radioactivité, QUASIMENT JAMAIS
demandé en RC. Quand l'énoncé dit « durée du régime transitoire », il veut $5\tau$, pas $\tau$ !
بالدارجة: $\tau$ = لحظة 63 %، و$5\tau$ = النهاية العملية (99 %). ملي كيقول «مدة النظام الانتقالي» راه بغا $5\tau$ — ماشي $\tau$!

**C3. « Le condensateur = interrupteur ouvert » — vrai, mais QUAND ?**
*Le clic :* seulement en **régime permanent établi** ($t\to\infty$, $i = 0$). Pendant le transitoire, le courant
passe (décroissant) ! Dire « $i = 0$ donc... » au milieu d'une charge est FAUX et coûte la question.
L'image qui reste : le condensateur chargé = réservoir PLEIN qui ne prend plus d'eau (ouvert) ; en cours de
remplissage, l'eau passe (fermé partiellement).
بالدارجة: المكثف = قاطع مفتوح **غير ملي يسالي الشحن** ($i=0$)! فالوسط ديال الشحن التيار كيدوز — اللي قال $i=0$ فالوسط غلط!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis (ce qu'il faut déjà savoir) :**
1. Loi des mailles + orientation (Tronc Commun) — sans ça, l'EDP est inatteignable.
2. Dérivée de $e^{kt}$ (Math ch.01-02) — pour VÉRIFIER les solutions.
3. Conversions $\mu F/nF/pF$ + puissances de 10 — la faute n°1 du Maroc.
4. Lecture de graphe : tangente, asymptote, 63 % (méthode physique, pas calcul).

**Si l'EDP bloque (le concept le plus dur) — plan B :**
L'EDP par les mailles est le passage qui fait le plus échouer. **Fallback officiel** : si après 5 min tu n'as pas
l'EDP, ADMETS-LA (« on admet $RC\frac{du_C}{dt}+u_C = E$ ») et fonce sur l'exploitation (solution, $\tau$, AN,
graphe, énergie) : c'est là que sont 80 % des points ! Un élève qui admet l'EDP et exploite juste a PLUS que
celui qui s'acharne et rend une copie vide.
بالدارجة: إلا وحلتي فالمعادلة التفاضلية أكثر من 5 دقايق: **قبلها وكمل** («on admet...»)! التنقيط الكبير فالاستغلال (الحل، $\tau$، الحساب، المنحنى، الطاقة) ماشي فالبرهنة. اللي قبل وكمل كيجيب النقط — واللي تعنّد كيخرج بورقة خاوية!
