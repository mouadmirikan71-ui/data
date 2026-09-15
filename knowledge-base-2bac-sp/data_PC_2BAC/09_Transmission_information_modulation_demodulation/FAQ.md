---
chapitre: "09 - Transmission information modulation demodulation"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
date_collecte: "2026-09-15"
type: "faq"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - modulation + demodulation"
---

# FAQ — Chapitre 09 (Transmission & modulation) ❓

**Q1. C'est quoi physiquement « l'enveloppe » d'un signal AM ?**
Les deux courbes lentes ($U_M(t)$ en haut, $U_m(t)$ en bas) qui ENCADRENT les oscillations rapides de la porteuse — c'est l'enveloppe qui porte l'info (elle a la forme de $s(t)$ !). Sur oscillogramme : les « vagues » lentes autour du « gribouillis » rapide !
الغلاف = الجوج منحنيات البطيئة اللي كيحيطو بالاهتزازات السريعة — **هو اللي هاز المعلومة** (عندو شكل $s(t)$ !). فالراسم : « الموجات » البطيئة حول « الخربشة » السريعة !

**Q2. Pourquoi faut-il $F_p \geq 10f_s$ (et pas juste $F_p > f_s$) ?**
Parce que l'enveloppe n'est bien définie que si BEAUCOUP d'oscillations porteuse tiennent dans une période d'enveloppe ($\geq 10$ !) — sinon on ne distingue plus l'enveloppe de la porteuse (le détecteur ne peut pas séparer les deux échelles). Le facteur 10 = la marge officielle !
حيت الغلاف ما كيتحدد مزيان غير إلا كان **بزاف** ديال اهتزازات الحاملة فدور واحد ($\geq 10$ !) — إلا لا، الغلاف والحاملة كيتخلطو (الكاشف ما يقدر يفرق) !

**Q3. La diode est-elle indispensable dans le détecteur ?**
OUI : sans diode, le condensateur se chargerait alternativement en $+$ et $-$ (moyenne nulle !) et ne suivrait AUCUNE enveloppe. La diode ne garde que le haut (alternances $+$) : c'est LÀ que vit l'enveloppe. Diode à l'envers = détecte l'enveloppe du bas (ça marche aussi, signal inversé !).
إيه : بلا ديود المكثف كيتشحن $+$ و$-$ بالتناوب (المعدل صفر !) وما كيتبع **والو** ! الديود كيخلي غير الفوق (فين عايش الغلاف) !

**Q4. Écrêtage : pourquoi les descentes sont-elles plates (et pas les montées) ?**
Parce que la CHARGE est rapide (via diode, $R \approx 0$ : suit les montées !) mais la DÉCHARGE est lente (via $R$ : $RC$ grand !). Quand l'enveloppe descend vite, le condensateur « ne descend pas assez vite » : la tension reste haute = plateau/écrêtage. Asymétrie charge/décharge = le cœur du défaut !
حيت **الشحن سريع** (عبر الديود : كيتبع الطلعات !) و**التفريغ بطيء** (عبر $R$ : $RC$ كبير !). ملي الغلاف كينزل بسرعة المكثف « ما كينزلش بالزربة » : التوتر كيبقى عالي = تسطيح/قص !

**Q5. Spectre AM : d'où sortent les 3 raies ($F_p$, $F_p \pm f_s$) ?**
Du produit $[U_0 + S_m\cos(2\pi f_s t)]\cos(2\pi F_p t)$ : $\cos A \cos B = \frac{1}{2}[\cos(A+B) + \cos(A-B)]$ (maths M02 !) → $F_p + f_s$ et $F_p - f_s$ ! Les 2 bandes latérales = l'info (sans elles, que la porteuse pure = silence !). Largeur totale occupée : $2f_s$.
من الجداء : $\cos A \cos B = \frac{1}{2}[\cos(A+B) + \cos(A-B)]$ ← $F_p + f_s$ و$F_p - f_s$ ! الجوج نطاقين الجانبيين = **المعلومة** (بلا بيهم : الحاملة بوحدها = الصمت !).

**Q6. Chaîne radio complète : dans quel ordre ?**
Émission : micro ($s(t)$) → MODULATEUR ($\times$ porteuse $F_p$) → antenne. Réception : antenne → TUNER (RLC en résonance sur $F_p$ : P08 !) → DÉTECTEUR d'enveloppe (diode + RC : ce chapitre !) → ampli → haut-parleur. Le tuner CHOISIT la station, le détecteur RÉCUPÈRE le son !
البث : ميكرو ← **مضمن** ← هوائي. الاستقبال : هوائي ← **موالف** (RLC فرنين على $F_p$ !) ← **كاشف الغلاف** ← مكبر ← مكبر الصوت. الموالف **كيختار** المحطة والكاشف **كيرجع** الصوت !
