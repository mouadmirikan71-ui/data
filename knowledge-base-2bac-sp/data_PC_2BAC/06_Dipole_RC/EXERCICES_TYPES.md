---
chapitre: "06 - Dipole RC"
unite: "Physique S1 - Électricité"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituée (style national PC) + corrigés prof"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - 4 type-bac + 2e méthode + pièges (backfill verbatim PC prévu)"
---

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types + corrigés — Chapitre 06 (Dipôle RC)

> **R1-R4 = type-bac reconstituées** dans le style du national PC (charge/décharge, $\tau$, énergie, linéarisation).
> Unités SI partout, AN avec chiffres significatifs. Banque verbatim prévue dès transcription.

## R1 — TYPE-BAC (établir l'EDP + vérifier la solution)

🏷️ matière=PC · année=— · session=— · chapitre=P6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Condensateur $C$ initialement vide en série avec $R$ et un générateur $E$ (interrupteur fermé à $t=0$).
(a) Établir l'équation différentielle vérifiée par $u_C$. (b) Vérifier que $u_C(t) = E(1-e^{-t/RC})$ est solution.

**Corrigé :**
(a) 1. Schéma orienté (flèches $u_R$, $u_C$, $i$ en convention récepteur). 2. Loi des mailles : $E = u_R + u_C = Ri + u_C$.
3. $i = \frac{dq}{dt} = C\frac{du_C}{dt}$ → $\boxed{RC\frac{du_C}{dt} + u_C = E}$ (forme canonique ✔).
(b) 1. Dériver : $\frac{du_C}{dt} = E\cdot\frac{1}{RC}e^{-t/RC}$. 2. Injecter : $RC\cdot\frac{E}{RC}e^{-t/RC} + E(1-e^{-t/RC}) = E$ ✔.
3. Condition initiale : $u_C(0) = E(1-1) = 0$ ✔ (continuité, condensateur vide).
> بالدارجة: الوصفة: **أسهم ← عقد ← عوّض $i=C\frac{du}{dt}$ ← الشكل القياسي**! والتحقق = اشتق وعوّض: إلا خرجات $E=E$ راه الحل صحيح. وجرب $t=0$ ديماً!

## R2 — TYPE-BAC ($\tau$ par 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Charge sous $E = 6,0\,V$ avec $R = 10\,k\Omega$, $C = 100\,\mu F$. La courbe $u_C(t)$ est relevée.
Déterminer $\tau$ par deux méthodes indépendantes.

**Corrigé — Méthode 1 : calcul direct.** $\tau = RC = 10\times10^3 \times 100\times10^{-6} = \boxed{1,0\,s}$.
(Conversions explicites : $k\Omega\to10^3$, $\mu F\to10^{-6}$ !)
**Corrigé — Méthode 2 : lecture graphique (63 %).** $0,63E = 3,78\,V$ → abscisse correspondante sur la courbe :
$t \approx 1,0\,s$ ✔. (Variante : tangente à l'origine → intersection avec $u_C = E$ à $t = \tau$.)
Concordance calcul/graphique = vérification. ✅
> بالدارجة: جوج طرق مستقلين: **الحساب** ($R\times C$ مع التحويلات!) و**المنحنى** (63 % ولا المماس). إلا تطابقو راه خدمتك صحيحة — هادي هي المراقبة الذاتية ديال التلميذ الممتاز!

## R3 — TYPE-BAC (décharge + temps + énergie)

🏷️ matière=PC · année=— · session=— · chapitre=P6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** Condensateur $C = 470\,\mu F$ chargé sous $E = 12\,V$, déchargé dans $R = 2,2\,k\Omega$ à $t=0$.
(a) $u_C(t)$ ? (b) À quel instant $u_C = 3,0\,V$ ? (c) Énergie initialement stockée ?

**Corrigé :**
(a) Décharge : $\boxed{u_C(t) = 12\,e^{-t/\tau}}$, $\tau = RC = 2,2\times10^3\times470\times10^{-6} = \boxed{1,03\,s}$.
(b) $3,0 = 12e^{-t/\tau}$ → $e^{-t/\tau} = 1/4$ → $t = \tau\ln 4 = 1,03\times1,386 = \boxed{1,43\,s}$.
(c) $E_e = \frac{1}{2}Cu_C^2(0) = \frac{1}{2}\times470\times10^{-6}\times144 = \boxed{3,38\times10^{-2}\,J}$ ($\approx 34\,mJ$).
> بالدارجة: التفريغ = $E$ مضروبة فالأسية الهابطة. ملي كتسول «فوقاش؟» ($t$ مجهولة) ← **اللوغاريتم** هو الحل! والطاقة بالصيغة $\frac{1}{2}Cu^2$ مع $u$ اللحظية (هنا البدئية 12V).

## R4 — TYPE-BAC (linéarisation $\ln u_C$)

🏷️ matière=PC · année=— · session=— · chapitre=P6 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Énoncé :** En décharge ($R = 4,7\,k\Omega$, $C$ inconnue), on trace $\ln(u_C)$ en fonction de $t$ : droite de
pente $-2,13\,s^{-1}$. Déterminer $C$.

**Corrigé :**
1. $u_C = Ee^{-t/\tau}$ → $\ln(u_C) = \ln E - \frac{t}{\tau}$ : droite, pente $= -1/\tau$.
2. $-1/\tau = -2,13$ → $\tau = 1/2,13 = 0,469\,s$.
3. $C = \tau/R = 0,469/(4,7\times10^3) = \boxed{9,98\times10^{-5}\,F \approx 100\,\mu F}$.
> بالدارجة: ملي تشوف $\ln$ فالكهرباء ← **خطّية المنحنى**! الميل = $-1/\tau$ كيعطيك $\tau$ بلا ما تشوف المنحنى الأصلي. ومن $\tau$ كتجبد $C$. هاد التقنية كتعاود فبزاف ديال الفصول!

## 🪤 Pièges testés par question
- **R1** : mailles non orientées (signe faux) ❌ ; vérifier la solution sans tester $u_C(0)$ ❌ ; EDP non canonique (terme en $i$ restant) ❌.
- **R2** : $\tau = 10\times100 = 1000\,s$ (conversions oubliées !) ❌ ; 63 % de $E$ lu sur la mauvaise courbe ❌ ; tangente tracée ailleurs qu'à l'origine ❌.
- **R3** : formule de CHARGE utilisée pour une décharge ❌ ; $t$ sans $\ln$ (bloqué sur l'exponentielle) ❌ ; $E_e$ avec $u$ finale au lieu de $u(0)$ ❌.
- **R4** : pente lue $= -\tau$ au lieu de $-1/\tau$ ❌ ; $C$ en $\mu F$ non converti pour $\tau$ ❌ ; oublier que la méthode exige une DÉCHARGE ($Ee^{-t/\tau}$, pas $1-e^{\ldots}$) ❌.

---
*Banque d'entraînement étiquetée type-bac. Backfill : questions RC verbatim du national PC dès transcription (sessions 2023-2025 prioritaires).*

## VRAIE — 2021N Ex4-I (RC : C = 12 μF via pente)

🏷️ matière=PC · année=2021 · session=N · chapitre=P6 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
Charge sous $E = 12$ V, $R = 1$ kΩ : EDP $du_C/dt + u_C/RC = E/RC$. Courbe $du_C/dt = f(u_C)$ affine : pente $a = (1000-0)/(0-12) = -83,3$ s⁻¹ → $-1/RC = a$ → $C = -1/(Ra) = 1,2\times10^{-5}$ F $= 12$ μF.
🪤 *vraie : $C$ via PENTE de $du_C/dt$ (pas de $\tau$ !) ; $a = -1/RC$ (identifier !).*
> بالدارجة: الميل ديال المنحنى كيعطيك $RC$ — قارن المعادلتين وجبد $C$ !
