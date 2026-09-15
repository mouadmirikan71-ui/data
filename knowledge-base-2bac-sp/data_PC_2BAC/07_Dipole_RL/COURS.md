---
chapitre: "07 - Dipole RL"
unite: "Physique S1 - Électricité"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof miroir RC (style national PC) - verbatim en backfill"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 07 — Dipôle RL

> 📋 **Exigible au bac** : établissement/rupture du courant, EDP, $\tau = L/R$, continuité de $i$, énergie
> $\frac{1}{2}Li^2$, surtension à la rupture, régime permanent (bobine réelle vs idéale).

## 1. Accroche — la bobine est têtue 🧲

**FR :** Deux expériences : (1) tu fermes un circuit avec une bobine + lampe : la lampe s'allume **EN RETARD**,
elle monte progressivement — la bobine freine l'ÉTABLISSEMENT du courant. (2) Tu OUVRES le circuit brutalement :
une **étincelle** jaillit à l'interrupteur ! La bobine refuse la RUPTURE et génère une surtension pour maintenir
le courant. Moral : la bobine DÉTESTE les variations de courant (loi de Lenz) — c'est l'INERTIE électrique,
exactement comme la masse déteste les variations de vitesse. Tout le chapitre = mettre cette têtu en équations.

**بالدارجة:** جوج تجارب: (1) ملي كتسد الدائرة اللي فيها وشيعة + مصباح: المصباح كيشعل **بالتأخر** — الوشيعة كتفرمل طلوع التيار! (2) ملي كتحل الدائرة بالزربة: **شرارة** كتطير! الوشيعة كترفض القطع وكتولد توتر زايد باش تحافظ على التيار. الخلاصة: الوشيعة **كتحقد على تغير التيار** (قانون لنز) — هي القصور الكهربائي، بحال الكتلة كتحقد على تغير السرعة!

## 2. Résumé du cours (exigible au bac)

### 2.1 La bobine — définitions
- Inductance $L$ (en **henrys**, $H$) ; résistance interne $r$ (en $\Omega$, souvent petite).
- Tension aux bornes : $\boxed{u_L = L\frac{di}{dt}}$ (bobine idéale, convention récepteur) ;
  bobine réelle : $u_b = ri + L\frac{di}{dt}$.
- **Continuité** : $i$ ne saute JAMAIS ($i(0^+) = i(0^-)$) — argument énergétique, comme $u_C$ en RC !
- Énergie emmagasinée : $\boxed{E_m = \frac{1}{2}Li^2}$ (en joules).

### 2.2 Établissement du courant (échelon $E$, $i(0) = 0$)
- Circuit : $E$ + résistor $R$ (+ $r$ de la bobine : $R_{tot} = R + r$) + bobine $L$ en série.
- Mailles : $E = Ri + L\frac{di}{dt}$ → **EDP** : $\boxed{L\frac{di}{dt} + Ri = E}$.
- Solution : $\boxed{i(t) = I_0\left(1-e^{-t/\tau}\right)}$, $I_0 = \frac{E}{R}$, $\boxed{\tau = \frac{L}{R}}$.
- Tension bobine : $u_L = L\frac{di}{dt} = Ee^{-t/\tau}$ — ⚠️ part de $E$ (max !), pas de 0 !

### 2.3 Rupture du courant (avec diode de roue libre)
- EDP : $L\frac{di}{dt} + Ri = 0$ → $\boxed{i(t) = I_0e^{-t/\tau}}$ (part de $I_0$, s'éteint).
- **Surtension** : à l'ouverture, $u_L = L\frac{di}{dt}$ fait un pic négatif ($\approx -RI_0$ sur la charge) :
  c'est l'étincelle ! La diode de roue libre offre au courant un chemin de passage (protection).
- Énergie $\frac{1}{2}LI_0^2$ dissipée en chaleur (Joule).

### 2.4 Régime permanent ($t \to \infty$)
- $\frac{di}{dt} = 0$ → bobine idéale : $u_L = 0$ = **court-circuit** (l'INVERSE du condensateur !).
- Bobine réelle : $u_b = rI_0$ (simple résistor). $I_0 = E/R_{tot}$.

### 2.5 Lecture graphique (miroir de RC)
- $\tau$ = temps pour atteindre $63\,\%$ de $I_0$ (établissement) / tomber à $37\,\%$ (rupture).
- Ou : tangente à l'origine → intersection avec l'asymptote ($I_0$ ou 0). Transitoire $\approx 5\tau$.

### 2.6 Le tableau miroir RC ↔ RL (à connaître !)

| RC ($u_C$) | RL ($i$) |
|---|---|
| $RC\frac{du_C}{dt}+u_C = E$ | $L\frac{di}{dt}+Ri = E$ |
| $\tau = RC$ | $\tau = L/R$ |
| $u_C$ continue | $i$ continu |
| $\frac{1}{2}Cu^2$ | $\frac{1}{2}Li^2$ |
| Permanent : interrupteur ouvert | Permanent : court-circuit |

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** الوشيعة = **العنيدة**! كتقاوم أي تغير فالتيار: ملي بغيتي تطلعو كتفرملك، وملي بغيتي تقطعو كتولد شرارة باش تبقيه. هاد العناد هو قانون لنز.

1. **التأسيس (Établissement):** ملي كتسد الدائرة، التيار كيبدا من 0 وكيطلع تدريجياً لـ $I_0 = E/R$: $i = I_0(1-e^{-t/\tau})$. توتر الوشيعة كيبدا من $E$ (كبيرة!) وكيهبط للصفر — **عكس التيار**!
2. **ثابت الزمن ($\tau = L/R$):** وشيعة كبيرة (عناد كبير) = بطء؛ مقاومة كبيرة (تيار صغير) = سرعة. إذن $\tau = L/R$ — المنطق!
3. **القطع (Rupture):** التيار كيهبط من $I_0$ للصفر: $i = I_0e^{-t/\tau}$. ولكن الوشيعة كتولد **توتر زايد** (surtension) فلحظة القطع — هادي هي الشرارة! الديود كيحمي الدائرة.
4. **النظام الدائم:** الوشيعة المثالية = **سلك** ($u_L = 0$) — عكس المكثف اللي كيولي قاطع مفتوح! هاد القلب هو السؤال المفضل ديال الوطني.
5. **الطاقة:** $\frac{1}{2}Li^2$ مخزونة فالمجال المغناطيسي — بحال الطاقة الحركية $\frac{1}{2}mv^2$! (التيار = السرعة، $L$ = الكتلة.)

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — إلا فهمتي RC، راه RL عندك 80 %!** نفس الرياضيات ($1-e^{-t/\tau}$ و$e^{-t/\tau}$)، غير المتغير تبدل ($u_C \to i$) والثابت تبدل ($RC \to L/R$).
أي تمرين RL: سول راسك «شنو المقابل ديالو فـ RC؟» والجواب كيجي بوحدو!

**الخطوة 2 — السلسلة الذهبية كيف RC:** رسم بالأسهم ← قانون العقد ← عوّض ← الشكل القياسي ← الحل بالشرط البدئي ($i(0) = 0$ فالتأسيس!) ← التطبيق العددي بالوحدات العالمية ($mH = 10^{-3} H$!).

**الخطوة 3 — زوج نقاط كيفرقو RL على RC:** (1) توتر الوشيعة **كيبدا من $E$** (ماشي من 0!) — اللي رسم $u_L$ طالعة من 0 غلط! (2) فالنظام الدائم الوشيعة = **سلك** (ماشي قاطع!) — عكس المكثف!

**الخطوة 4 — تشبيه واحد يعاونك:** **التيار = سيارة، الوشيعة = كتلتها (inertie)، المقاومة = الفرامل، المولد = المحرك.** كتلة كبيرة = إقلاع بطيء ($\tau = L/R$)! والشرارة ملي كتقطع = السيارة اللي ما بغاتش تحبس!

**الخطوة 5 — الأخطاء القاتلة:** نسيان $r$ فـ $R_{tot}$؛ $\tau = L\times R$ (غلط! القسمة!)؛ $u_L(0) = 0$ (غلط! $= E$!)؛ «الوشيعة = قاطع مفتوح» فالدائم (غلط! = سلك!)؛ الوحدات ($mH$ بلا تحويل!).

## 5. Définitions & formules clés (FR + Darija)

| Notion FR (LaTeX) | Énoncé FR | بالدارجة |
|---|---|---|
| $u_L = L\frac{di}{dt}$ | Tension proportionnelle à la VARIATION du courant | التوتر تابع للتغير ماشي للتيار! |
| $\tau = L/R$ | Constante de temps (s) | مقياس العناد — شحال كيطول التأسيس |
| Établissement $i = I_0(1-e^{-t/\tau})$ | Monte de 0 vers $I_0$ | طلوع التيار تدريجياً |
| Rupture $i = I_0e^{-t/\tau}$ | Descend de $I_0$ vers 0 + surtension | الهبوط + الشرارة! |
| Continuité de $i$ | Pas de saut (énergie finie) | التيار ما كيقفزش |
| $E_m = \frac{1}{2}Li^2$ | Énergie magnétique (J) | المخزون المغناطيسي |
| Permanent | Bobine idéale = fil ($u_L = 0$) | الوشيعة كتولي سلكة |

## 6. FAQ du chapitre

**Q1. Pourquoi $u_L$ part de $E$ alors que $i$ part de 0 ?**
Parce qu'à $t = 0$, $i = 0$ donc $Ri = 0$ et les mailles donnent $u_L = E - 0 = E$ ! La bobine « prend » toute la
tension au début (variation max), puis la rend au résistor. C'est le contraire de l'intuition — d'où les pièges.
بالدارجة: حيت فـ $t=0$ التيار صفر ← المقاومة ما كتاخذ والو ← الوشيعة كتاخذ $E$ كاملة! عكس الحدس — وهنا كيتصيدو التلاميذ!

**Q2. Pourquoi une étincelle à l'ouverture ?**
$i$ ne peut pas sauter (énergie $\frac{1}{2}Li^2$). Ouvrir brutalement force $\frac{di}{dt}$ énorme →
$u_L = L\frac{di}{dt}$ énorme → claquage de l'air = étincelle. La diode donne au courant un chemin doux.
بالدارجة: التيار ما كيقفزش — القطع المفاجئ كيولد توتر هائل كيشعل الهواء = شرارة! الديود كيعطيه طريق ناعمة.

**Q3. $\tau = L/R$ : pourquoi DIVISÉ ?**
$L$ grande = grosse inertie = lent (numérateur ✔) ; $R$ grande = courant faible = vite établi (dénominateur ✔).
Et dimension : $H/\Omega = (V\cdot s/A)/(V/A) = s$ ✔.
بالدارجة: وشيعة كبيرة = بطء (الفوق)، مقاومة كبيرة = سرعة (التحت). والبعد كيخرج بالثانية — تحقق!

**Q4. Bobine réelle vs idéale : ça change quoi ?**
Idéale ($r = 0$) : permanent = court-circuit pur. Réelle : $R_{tot} = R+r$ partout ($I_0$, $\tau$) + $u_b = rI_0$
en permanent. Oublier $r$ = TOUT faux (AN).
بالدارجة: الحقيقية: زيد $r$ على $R$ فكلشي! اللي نساها خسر التطبيق العددي كامل!

**Q5. RC ou RL : comment les distinguer en 5 s ?**
Le composant bizarre : deux plaques ($C$, en $F$) → RC ; spires ($L$, en $H$) → RL. L'unité tranche toujours !
بالدارجة: شوف الوحدة: فاراد = RC، هنري = RL. الوحدة كتحكم ديماً!

**Q6. Le courant peut-il dépasser $I_0$ ?**
NON en établissement simple (monotone vers $I_0$). Il ne dépasse que dans les oscillations (RLC, ch.08 !).
بالدارجة: لا! فالتأسيس العادي التيار كيطلع بلا ما يفوت $I_0$. التجاوز غير فالاهتزازات (الفصل الجاي!).

## 7. Pièges classiques + mots-clés ⚠️

**À écrire absolument** : schéma orienté ; « d'après la loi des mailles » ; EDP canonique ; « $i$ continu donc
$i(0^+) = \ldots$ » ; $R_{tot} = R+r$ explicite ; $\tau = L/R$ en **s** ; AN + unités ; $\boxed{\text{résultat}}$.
**Erreurs fréquentes** : $r$ oubliée ❌ ; $\tau = LR$ ❌ ; $u_L(0) = 0$ ❌ ; bobine = interrupteur ouvert ❌ ;
$mH$ non convertis ❌ ; formule d'établissement pour une rupture ❌.

## 8. Sources de ce chapitre
- Synthèse prof miroir RC (cours + exercices type-bac) : rédaction originale pour cette base, 2026-09-15.
- Backfill prévu : questions RL verbatim du national PC (sessions 2023-2025 prioritaires).

## 9. Le « pourquoi » profond — Lenz gouverne tout 🔬

**Pourquoi l'EDP a cette forme ? (Lenz → mailles → exponentielle)**
La bobine génère une force contre-électromotrice $e = -L\frac{di}{dt}$ qui S'OPPOSE à la variation (Lenz : « la
nature déteste le changement »). Dans les mailles : $E$ pousse, $Ri$ freine (Joule), $L\frac{di}{dt}$ freine
PROPORTIONNELLEMENT À LA VITESSE DE VARIATION. Vitesse de variation freinée proportionnellement à l'écart
restant → exponentielle (même théorème qu'en RC, §9 du ch.06 !). Lenz est le « pourquoi physique », l'exponentielle
le « comment mathématique ».

**Pourquoi $\tau = L/R$ ? (l'inertie contre le frein)**
$L$ = inertie (résiste au changement : ralentit → au NUMÉRATEUR) ; $R$ = dissipation (tue le courant : accélère
l'établissement du régime → au DÉNOMINATEUR). Compare la mécanique : $m$ (inertie) / $k$ (frottement) donne le
temps caractéristique de la chute freinée — MÊME structure ! Dimension : $[L] = \frac{V\cdot s}{A}$ (car
$u = L\frac{di}{dt}$), $[R] = \frac{V}{A}$ → $[L/R] = s$ ✔.

**Pourquoi la surtension est INÉVITABLE sans diode ?**
L'énergie $\frac{1}{2}LI_0^2$ DOIT aller quelque part (conservation !). Couper le chemin = forcer le courant à
s'arrêter dans un air isolant ($R \to \infty$) → $u = L\frac{di}{dt}$ explose → l'air devient conducteur (claquage)
→ étincelle = l'énergie qui s'échappe en lumière + chaleur. La diode ne « supprime » pas l'énergie : elle lui
offre un chemin civilisé (Joule dans $R$).

**Ponts :** RC ch.06 (miroir complet : $u \leftrightarrow i$, $C \leftrightarrow L$) ; RLC ch.08 (les deux inerties
ensemble → oscillations !) ; Newton ch.10 (tableau électromécanique : $i \leftrightarrow v$, $L \leftrightarrow m$,
$R \leftrightarrow k$, $E \leftrightarrow F$ — TOUT le chapitre se devine depuis la mécanique) ; Maths EDP (même
équation, même solution).

> بالدارجة: علاش المعادلة هاكا؟ حيت الوشيعة كتولد قوة **ضد التغير** (لنز: الطبيعة كتكره التبدل!) — والفرملة المتناسبة مع الباقي = أسية (نفس المبرهنة ديال RC!). و$\tau = L/R$: العناد (L) كيبطئ ← الفوق، والفرملة (R) كتسرع ← التحت. والشرارة حتمية بلا ديود: الطاقة $\frac{1}{2}Li^2$ **خاصها تمشي لشي بلاصة** (الحفاظ!) — إلا سديتي الطريق كتفجر الهواء!

## 10. Les 3 confusions qui coûtent des points 😵

**C1. $u_L(0) = E$, PAS 0 ! — le piège n°1 du chapitre.**
*Le clic :* à $t = 0$, $i = 0$ → le résistor ne « mange » rien ($Ri = 0$) → TOUTE la tension $E$ est aux bornes de
la bobine. La courbe de $u_L$ PART DU PLAFOND et descend — l'exact contraire de $u_C$ en RC qui part du plancher !
Dessine les deux courbes côte à côte une fois, tu ne confondras plus.
بالدارجة: فـ $t=0$ التيار صفر ← المقاومة ما كتاكل والو ← الوشيعة كتاخذ $E$ كاملة! منحنى $u_L$ **كيبدا من السقف وكيهبط** — عكس $u_C$! رسمهم حدا بعض مرة وحدة وعمرك تخلط!

**C2. Permanent : bobine = FIL, condensateur = INTERRUPTEUR — l'inversion fatale.**
*Le clic :* en continu établi, $\frac{di}{dt} = 0$ → $u_L = 0$ → la bobine idéale est un COURT-CIRCUIT (le courant
passe librement). Le condensateur, lui, bloque ($i = 0$). Retiens : « la bobine aime le courant établi, le
condensateur le déteste » — chacun bloque ce que l'autre laisse passer.
بالدارجة: فالدائم: الوشيعة = **سلك** (التيار دايز!)، المكثف = **قاطع** (التيار حابس!). حفظ: «الوشيعة كتبغي التيار المستقر، والمكثف كيكرهو»!

**C3. À la rupture, $i$ est continu mais $u_L$ SAUTE !**
*Le clic :* la continuité protège $i$ (énergie $\frac{1}{2}Li^2$), PAS $u_L = L\frac{di}{dt}$ qui dépend de la
PENTE de $i$. À l'ouverture, la pente change brutalement → $u_L$ fait un bond (le pic de surtension). Miroir de RC :
là-bas, $u_C$ continue mais $i$ saute à la commutation ! Règle : « l'énergieux est continu, son copain peut sauter ».
بالدارجة: اللي فيه الطاقة ($i$ هنا، $u_C$ فـ RC) ما كيقفزش — ولكن صاحبو ($u_L$) كيقدر! فلحظة القطع $u_L$ كتنقز (الشرارة) والتيار كيبقى متصل!

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Carte des prérequis :**
1. Dipôle RC (ch.06) : EDP, $\tau$, 63 %, $5\tau$ — TOUT se transpose par le tableau miroir.
2. Loi des mailles + orientation (TC) — les signes font l'EDP.
3. Dérivée de $e^{kt}$ (Maths) — pour vérifier les solutions.
4. Conversions $mH/H$, $mA/A$ + puissances de 10.

**Si l'EDP bloque — plan B :**
Même fallback qu'en RC : après 5 min, ADMETS l'EDP (« on admet $L\frac{di}{dt}+Ri = E$ ») et exploite
(solution, $\tau$, graphes, énergie) : 80 % des points ! Bonus RL : si tu connais RC par cœur, RECOPIE la
structure en échangeant $u_C \to i$, $C \to L$, $RC \to L/R$ — l'EDP « devinée » par miroir est juste.
بالدارجة: إلا وحلتي: **قبل المعادلة وكمل** (80 % ديال النقط فالاستغلال)! والحيلة: نسخ بنية RC وبدّل $u_C \to i$ و$RC \to L/R$ — المعادلة «المخمّنة بالمراية» صحيحة!
