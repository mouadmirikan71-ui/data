---
chapitre: "08 - Circuit RLC sinusoidal force"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
date_collecte: "2026-09-15"
type: "faq"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - force"
---

# FAQ — Chapitre 08 (RLC force) ❓

**Q1. Quelle est la difference entre regime LIBRE et regime FORCE ?**
Libre : pas de generateur (ou transitoire) — le circuit oscille a SON $\omega_0$ et s'amortit. Force : GBF impose $u = U_m\cos(\omega t)$ en permanence — le circuit repond a $\omega$ IMPOSEE ($i = I_m\cos(\omega t - \varphi)$). Au bac P08 : TOUJOURS force (le libre = §0 socle) !
الحر : بلا مولد — كتهتز بترددها وكتموت. القسري : المولد كيفرض $\omega$ — الدائرة كتجاوب بنفس $\omega$ !

**Q2. $Z$ depend de $\omega$ — mais $R$ aussi ?**
NON : $R+r$ = constante (vraie resistance, Joule). Ce qui depend de $\omega$ : $L\omega$ (grandit) et $1/C\omega$ (diminue) — leur DIFFERENCE fait bouger $Z$ et $\varphi$. A $\omega_0$ la difference s'annule → $Z = R+r$ (minimale !).
$R$ ثابتة ! اللي كيتبدل : $L\omega$ (كيكبر) و$1/C\omega$ (كيصغار) — الفرق بيناتهم كيحرك $Z$ و$\varphi$ !

**Q3. Comment lire $\varphi$ sur un oscillogramme ?**
Mesurer le decalage $\Delta t$ entre les deux max + la periode $T$ : $|\varphi| = 2\pi\Delta t/T$. SIGNE : celle qui atteint son max EN PREMIER est en avance — si c'est $u$ → $\varphi > 0$, si c'est $i$ → $\varphi < 0$. Verifier avec $\tan\varphi$ (calcul) !
قيس الفرق $\Delta t$ بين العظميين والدور $T$ : $|\varphi| = 2\pi\Delta t/T$. الإشارة : اللي كتوصل **اللولة** هي السابقة !

**Q4. La bande passante : pourquoi $I_{max}/\sqrt{2}$ et pas $I_{max}/2$ ?**
Parce que $-3$ dB = moitie de la PUISSANCE ($P \propto I^2$) : $P/2$ → $I/\sqrt{2}$ ! $I_{max}/2$ donnerait $P/4$ ($-6$ dB) — FAUX. Reflexe : dB = puissance ($I^2$) → racine !
حيت $-3$ dB = نص **الاستطاعة** ($P \propto I^2$) : $P/2$ ← $I/\sqrt{2}$ ! $I/2$ كتعطي $P/4$ — غلط !

**Q5. $Q = 50$ : c'est bien ou dangereux ?**
Les deux ! Bien : ultra-selectif (radio pro). Dangereux : surtension $\times 50$ — un condensateur 12 V sur un GBF 10 V a la resonnance CLAUQE ($U_C = 500$ V !). En TP : verifier le calibre AVANT de chercher la resonnance !
بجوج ! مزيان : انتقائية عالية. خطير : فرط التوتر $\times 50$ — المكثف **كينفجر** ! فالأعمال التطبيقية : تأكد من العيار قبل ما تقلب على الرنين !

**Q6. Faut-il apprendre Fresnel par cœur ?**
NON — il faut savoir le RECONSTRUIRE : $U_R$ avec $I$ (horizontal), $U_L$ a $+\pi/2$ ($L\omega I_m$), $U_C$ a $-\pi/2$ ($I_m/C\omega$), Pythagore → $Z$, $\tan\varphi$ = oppose/adjacent. C'est le PLAN B officiel quand les formules bloquent (COURS §11) !
لا — خاصك تعرف **تعاود تبنيه** : $U_R$ أفقي، $U_L$ الفوق، $U_C$ التحت، فيثاغورس ← $Z$ ! هادا هو Plan B ملي الصيغ كيبلوكيو !
