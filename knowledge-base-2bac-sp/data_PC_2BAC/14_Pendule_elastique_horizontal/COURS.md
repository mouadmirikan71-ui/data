---
chapitre: "14 - Pendule élastique horizontal"
unite: "Physique S2 - Mécanique"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (canon national : x¨+(k/m)x=0, T0=2π√(m/k), énergie, amortissement) + scission P14/P15 v2"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - élevé (§9+§10+§11)"
---

# Chapitre 14 — Pendule élastique horizontal

> 📋 **Exigible au bac (SI !)** : masse $m$ + ressort $k$ horizontal sans frottement : $\boxed{\ddot{x} + (k/m)x = 0}$ ; $\boxed{T_0 = 2\pi\sqrt{m/k}}$, $\boxed{\omega_0 = \sqrt{k/m}}$, $f_0 = 1/T_0$ ; solution $\boxed{x = X_m\cos(\omega_0 t + \varphi)}$ ($\varphi$ par conditions initiales !) ; $\boxed{v_{max} = \omega_0X_m}$ (au CENTRE) ; énergie $\boxed{E_m = \tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv_{max}^2}$ = cste ; vertical : MÊME $T_0$ ! ; amortissement : $T \approx T_0$, amplitude ↓.

## 1. Accroche — l'amortisseur de voiture 🚗🌀

Une voiture passe sur un dos-d'âne : elle rebondit… puis s'immobilise. Sans amortisseurs, elle rebondirait indéfiniment ! Sous la carrosserie : des RESSORTS (qui rappellent) + des amortisseurs (qui freinent). Tout le chapitre : *le ressort impose un tempo $T_0 = 2\pi\sqrt{m/k}$, l'énergie fait le ping-pong $E_c \leftrightarrow E_p$, et les frottements mangent l'amplitude.* Le jumeau angulaire (pendules) : P15.

> بالدارجة : الطوموبيل دازت على ضرضور : كتنقز... ومن بعد كتسكت. بلا ماصّات الصدمات، غادي تنقز بلا حبس ! تحت الكاروسري : **نوابض** (كترجع) + **ماصّات** (كتفرمل). كاع الفصل : *النابض كيفرض الإيقاع $T_0 = 2\pi\sqrt{m/k}$، والطاقة كتلعب البينغ-بونغ $E_c \leftrightarrow E_p$، والاحتكاكات كتاكل السعة.* التوأم الزاوي (الرقاصات) : P15.

## 2. Résumé du cours (exigible au bac)

**Dispositif.** Masse $m$ accrochée à un ressort de raideur $k$ (N/m), axe horizontal, SANS frottement. Équilibre en $x = 0$ (ressort ni étiré ni comprimé). On écarte à $X_m$ et on lâche : oscillations autour de 0.

**Équation différentielle (PFD — P10 !).** Seule force horizontale : rappel $\vec{F} = -kx\,\vec{i}$ → $m\ddot{x} = -kx$ → $\boxed{\ddot{x} + (k/m)x = 0}$ (même EDL que M10 : $y'' + \omega_0^2y = 0$ !).

**Période propre.** $\boxed{T_0 = 2\pi\sqrt{m/k}}$, $\boxed{\omega_0 = \sqrt{k/m}}$ (rad/s), $f_0 = 1/T_0$ (Hz). En haut l'INERTIE ($m$ : lourd = lent ✓), en bas le RAPPEL ($k$ : raide = rapide ✓). Ex. : $m = 0{,}20$ kg, $k = 20$ N/m → $T_0 = 2\pi\sqrt{0{,}01} = 0{,}63$ s.

**Ressort VERTICAL : même $T_0$ !** Le poids décale juste l'équilibre ($\Delta l = mg/k$) : autour du nouvel équilibre, $\ddot{x} + (k/m)x = 0$ IDENTIQUE. ($T_0$ ne dépend que de $m$ et $k$ — $g$ n'y figure même pas !)

**Solution : le cosinus.** $\boxed{x(t) = X_m\cos(\omega_0 t + \varphi)}$ : $X_m$ = amplitude, $\varphi$ = phase à l'origine (conditions INITIALES : lâché sans vitesse à $X_m$ → $\varphi = 0$ ; passage par 0 à $v_{max}$ → $\varphi = \pm\pi/2$). Vitesse : $v = -\omega_0X_m\sin(\omega_0t + \varphi)$ → $\boxed{v_{max} = \omega_0X_m}$, $a_{max} = \omega_0^2X_m$. Vitesse max au CENTRE, nulle aux EXTRÉMITÉS.

**Énergie : le ping-pong.** $\boxed{E_m = \tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv_{max}^2}$ = cste (sans frottement) : $E_p = \tfrac{1}{2}kx^2$ (max aux bouts) ↔ $E_c$ (max au centre). **Amortissement** (frottements) : pseudo-période $T \approx T_0$, amplitude décroît (exponentielle) — $E_m$ mangée par frottements.

**Unités SI.** $m$ : kg. $k$ : N/m. $x$, $X_m$ : m. $T_0$ : s. $\omega_0$ : rad/s. $\varphi$ : rad. $f_0$ : Hz. $E$ : J.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الجهاز :** كتلة $m$ معلقة في نابض الصلابة ديالو $k$ (N/m)، أفقي، **بلا احتكاك**. التوازن في $x = 0$. كنبعدو بـ $X_m$ وكنطلقو : تذبذبات حول الصفر.

**المعادلة (PFD — P10 !) :** القوة الأفقية الوحيدة : الإرجاع $\vec{F} = -kx$ ← $m\ddot{x} = -kx$ ← $\boxed{\ddot{x} + (k/m)x = 0}$ (نفس معادلة M10 !).

**الدور الخاص :** $\boxed{T_0 = 2\pi\sqrt{m/k}}$ : الفوق **القصور** ($m$ : ثقيل = بطيء ✓)، التحت **الإرجاع** ($k$ : قاصح = سريع ✓).

**النابض العمودي : نفس $T_0$ !** الوزن غير كيزيح التوازن ($\Delta l = mg/k$) : حول التوازن الجديد، نفس المعادلة بالضبط ($g$ أصلاً ما كايناش في $T_0$ !).

**الحل : الكوسينوس.** $\boxed{x = X_m\cos(\omega_0t + \varphi)}$ : $\varphi$ من **الشروط الابتدائية** (مطلق بلا سرعة من $X_m$ ← $\varphi = 0$). $\boxed{v_{max} = \omega_0X_m}$ : السرعة قصوى في **الوسط**، صفر في **الأطراف**.

**الطاقة :** $\boxed{E_m = \tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv_{max}^2}$ = ثابتة : $E_p$ قصوى في الأطراف ↔ $E_c$ قصوى في الوسط. **التخميد** : $T \approx T_0$، السعة كتنقص (الاحتكاك كياكل الطاقة).

## 4. How to understand this chapter the easy way 🎯

*(النسخة الكاملة خطوة بخطوة بالدارجة : voir `COMPRENDRE_FACILEMENT.md` — 5 étapes : inertie/rappel → EDP → cosinus → énergie → vertical.)*

**En 30 secondes :** ① $T_0 = 2\pi\sqrt{m/k}$ (lourd = lent, raide = rapide). ② EDP par PFD : $-kx = m\ddot{x}$. ③ Cosinus : $\varphi$ = conditions initiales (lâché → 0). ④ Énergie : $\tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv_{max}^2$ (1 ligne pour $v_{max}$ !). ⑤ Vertical : même $T_0$ (équilibre décalé).

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| Raideur $k$ | الصلابة | N/m : raide = rappel fort |
| Pulsation $\omega_0$ | النبض الخاص | $\sqrt{k/m}$ (rad/s) |
| Période propre $T_0$ | الدور الخاص | $2\pi\sqrt{m/k}$ (s) |
| Amplitude $X_m$ / phase $\varphi$ | السعة / الطور | $X_m$ (m), $\varphi$ (rad, initiales !) |
| Amortissement | التخميد | $T \approx T_0$, amplitude ↓ |

## 6. FAQ du chapitre

Voir `FAQ.md` (6 questions FR + Darija) : 1. Vertical : $T_0$ change ? 2. $\sqrt{m/k}$ ou $\sqrt{k/m}$ ? 3. $\varphi$ : deviner ? 4. $v_{max}$ où ? 5. Amorti : $T$ change ? 6. $k$ : unités et sens ?

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **Vertical : « $T_0$ change (le poids s'ajoute) »** : NON — le poids translate l'équilibre, la dynamique autour est identique. $g$ ne figure même pas dans $T_0$ !
- 🪤 **$\sqrt{k/m}$ au lieu de $\sqrt{m/k}$** : lourd ($m$ ↑) = LENT ($T_0$ ↑) → $m$ au NUMÉRATEUR. Test : $m \to \infty$ : immobile ($T_0 \to \infty$ ✓).
- 🪤 **$X_m$ en cm dans les formules** : $5{,}0$ cm → $v = 50$ m/s (FAUX !). TOUT en SI : $0{,}050$ m AVANT de calculer.
- 🪤 **$\varphi$ devinée** : $\varphi$ vient des conditions INITIALES ($x(0)$, $v(0)$), jamais au hasard (lâché sans vitesse à $X_m$ → $\varphi = 0$).
- Mots-clés : *SI (m, kg, N/m), $m$ en haut / $k$ en bas, $\varphi$ = initiales, $v_{max}$ au centre, vertical = même $T_0$.*

## 8. Sources de ce chapitre

Voir `SOURCES.md` (canon national : pendule élastique — synthèse prof ; jumeau P15, PFD P10, EDL M10).

## 9. Le « pourquoi » profond — pourquoi le ressort impose son tempo 🔬

**Pourquoi $\ddot{x} + (k/m)x = 0$ ?** PFD (P10) : la seule force horizontale est le rappel $-kx$ (loi de Hooke : proportionnel à l'écart, opposé au déplacement) → $m\ddot{x} = -kx$. **Le signe MOINS = le secret : la force ramène TOUJOURS vers 0 (rappel), d'où l'oscillation.** Sans moins (répulsion), la masse fuirait — pas d'oscillateur !

**Pourquoi le vertical a-t-il le même $T_0$ ?** Le poids $mg$ est CONSTANT : il décale l'équilibre (ressort déjà étiré de $mg/k$) mais la VARIATION de force autour de l'équilibre reste $-kx$. Poser $X$ = écart au nouvel équilibre → $m\ddot{X} = -kX$ : équation IDENTIQUE. **Seules les forces VARIABLES comptent dans la dynamique ; les constantes règlent le décor (équilibre).**

**Pourquoi $v_{max}$ au centre ?** Énergie : $E_m = \tfrac{1}{2}kx^2 + \tfrac{1}{2}mv^2$ = cste. Aux extrémités ($x = \pm X_m$) : tout est potentiel → $v = 0$. Au centre ($x = 0$) : tout est cinétique → $v$ max. **Le centre = le point où le ressort a tout « rendu » en vitesse.**

**Liens croisés :** P15 — jumeau angulaire (mêmes maths en $\theta$ !) ; P10 — PFD (source de l'EDP) ; M10 — EDL $y'' + \omega_0^2y = 0$ ; P08 — RLC : $T_0 = 2\pi\sqrt{LC}$ ($L \leftrightarrow m$, $C \leftrightarrow 1/k$ : l'analogie électromécanique !) ; SVT/techno — sismographe (masse-ressort géant), amortisseurs auto.

## 10. Les 3 confusions qui coûtent des points 😵

**1. « Ressort vertical : $T_0$ change (poids en plus). »** Non : le poids translate l'ÉQUILIBRE, la dynamique autour est identique. **Le déclic :** *$T_0$ ne dépend que de $m$ et $k$ — $g$ n'y figure même pas ! Si $g$ comptait, il serait dans la formule.*

**2. « $T_0 = 2\pi\sqrt{k/m}$. »** Non : $m$ en HAUT ($m$ ↑ = lent = $T_0$ ↑). **Le déclic :** *imagine $m$ énorme (wagon) sur ressort mou : ça oscille lentement, évidemment → $T_0$ GRAND → $m$ au numérateur. Le bon sens place les lettres.*

**3. « $\varphi = 0$ toujours. »** Non : $\varphi = 0$ SEULEMENT si lâché sans vitesse à $+X_m$ (cosinus max à $t = 0$). Lancé depuis 0 ? $\varphi = \pm\pi/2$. **Le déclic :** *le cosinus est une FORME — $X_m$ et $\varphi$ disent où tu COMMENCES sur cette forme. Conditions initiales = point de départ.*

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** P10 (PFD : $\sum F = ma$), M10 (EDL $y'' + \omega^2y = 0$), trigo ($\cos$, $\sin$, dérivées), conversions (cm→m, g→kg). **Test 30 s :** $k \times 4$ → $T_0$ ? ($\div 2$ — racine !) ; $X_m = 5$ cm en SI ? ($0{,}05$ m).

**Plan B — si l'équa diff bloque :** $T_0 = 2\pi\sqrt{m/k}$ par cœur + énergie ($\tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv^2$) → périodes, vitesses, amplitudes SANS jamais résoudre d'équation. L'énergie est l'angle de secours universel des oscillateurs.

**Fiche réflexes :** *$-kx = m\ddot{x}$ · $T_0 = 2\pi\sqrt{m/k}$ · $\varphi$ = initiales · $v_{max} = \omega_0X_m$ au centre · $\tfrac{1}{2}kX_m^2 = \tfrac{1}{2}mv^2$ · vertical = même $T_0$ · SI !*
