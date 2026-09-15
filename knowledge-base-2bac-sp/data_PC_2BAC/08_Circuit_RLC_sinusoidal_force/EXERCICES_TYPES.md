---
chapitre: "08 - Circuit RLC sinusoidal force"
unite: "Physique S1 - Electricite"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Banque type-bac reconstituee (style national PC) + corriges prof - v2 FORCE"
date_collecte: "2026-09-15"
type: "exercise"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - 3 type-bac force + 2e methode + pieges + VRAIE 2021N"
---

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types + corriges — Chapitre 08 (RLC force)

> **R1-R3 = type-bac reconstituees** (impedance/Fresnel, resonnance, bande passante). Unites SI partout. Meme $\omega$ pour $u$ et $i$ — toujours !

## Methode — RLC force en 5 gestes 🧭

1. **Convertir** : $mH \to H$, $\mu F \to F$, $kHz \to Hz$ — AVANT tout calcul !
2. **Identifier** : force ($\omega$ imposee par GBF) vs libre ($\omega_0$ propre) — ici TOUJOURS force !
3. **$Z$, $\varphi$** : formules OU Fresnel (Pythagore !) — $\varphi = \varphi_u - \varphi_i$ !
4. **Resonnance ?** $L\omega = 1/C\omega$ → $Z = R+r$, $I_{max}$, $\varphi = 0$.
5. **max vs efficace** : oscillo/calcul $\to U_m$ ; voltmetre/puissance $\to U_{eff} = U_m/\sqrt{2}$ !

## R1 — TYPE-BAC (impedance + dephasage, 2 methodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P8 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Enonce :** RLC serie : $R = 20\,\Omega$, bobine $(r = 10\,\Omega, L = 0{,}10\,H)$, $C = 10\,\mu F$. GBF : $u(t) = 6{,}0\cos(1000t)$ (V). (a) $Z$, $I_m$, $\varphi$ (2 methodes !). (b) $i(t)$. (c) Comportement inductif ou capacitif ?

**Corrige :**
$\omega = 1000$ rad/s ; $R+r = 30\,\Omega$ ; $L\omega = 100\,\Omega$ ; $1/C\omega = 100\,\Omega$.
(a) **Methode 1 (formules)** : $Z = \sqrt{30^2 + (100-100)^2} = \boxed{30\,\Omega}$ ; $I_m = U_m/Z = 6{,}0/30 = \boxed{0{,}20\,A}$ ; $\tan\varphi = 0/30 = 0 \to \boxed{\varphi = 0}$ (resonance ! $\omega = 1/\sqrt{LC} = 1000$ ✔).
**Methode 2 (Fresnel)** : $U_{Rm} = 30 \times 0{,}20 = 6{,}0$ V ; $U_{Lm} = 100 \times 0{,}20 = 20$ V ; $U_{Cm} = 100 \times 0{,}20 = 20$ V → L et C s'annulent ($20 - 20 = 0$ !) → $U_m = 6{,}0$ V ✔, $\varphi = 0$ ✔ (vecteur resultant horizontal !).
(b) $\boxed{i(t) = 0{,}20\cos(1000t)}$ (en phase !).
(c) Ni l'un ni l'autre : $\boxed{\text{resistif (resonnance)}}$ — $u$ et $i$ en phase !
🪤 *Piege teste : $Z = R + r + L\omega + 1/C\omega = 230\,\Omega$ (addition bourrin !) — $Z$ = racine d'une SOMME DE CARRES, et $L\omega - 1/C\omega$ se retranchent !*
> بالدارجة: $L\omega = 100$ و$1/C\omega = 100$ — **تساواو** ← رنين ! $Z = 30$ ($\Omega$ صافي)، $\varphi = 0$ ! وبفرينل : $U_L = 20$ الفوق و$U_C = 20$ التحت **كيتلغاو** ← كيبقى $U_R = 6$ ! (ولاحظ : $U_C = 20 > U = 6$ — **فرط التوتر** : $Q = L\omega_0/30 = 3{,}3$ !)

## R2 — TYPE-BAC (resonnance : $f_0$ par 2 methodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P8 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Enonce :** RLC serie $(R+r = 50\,\Omega, L = 0{,}20\,H, C = 5{,}0\,\mu F)$, $U_m = 10$ V constant. La courbe $I(f)$ relevee est une cloche de sommet $I_{max} = 0{,}20$ A a $f = 159$ Hz. (a) $f_0$ par 2 methodes. (b) Verifier $I_{max}$.

**Corrige :**
(a) **Methode 1 (calcul)** : $f_0 = 1/2\pi\sqrt{LC} = 1/(2\pi\sqrt{0{,}20 \times 5{,}0\times10^{-6}}) = 1/(2\pi\times10^{-3}) = \boxed{159\,Hz}$.
**Methode 2 (courbe)** : sommet de la cloche $I(f)$ → $\boxed{f_0 = 159\,Hz}$ (lu !). ✅ Concordance calcul/mesure !
(b) $I_{max} = U_m/(R+r) = 10/50 = \boxed{0{,}20\,A}$ ✔ (la valeur du sommet confirme $R+r$ !).
🪤 *Piege teste : $f_0 = 1/\sqrt{LC} = 1000$ « Hz » ($\omega_0$ lue comme $f_0$ !) — $1/\sqrt{LC}$ = $\omega_0$ en rad/s, DIVISER par $2\pi$ pour $f_0$ !*
> بالدارجة: **الحساب** ($1/2\pi\sqrt{LC}$) و**القمة ديال الجرس** — بجوج كيعطيو 159 Hz ! والقمة $I_{max} = U_m/(R+r)$ كتأكد $R+r$ ! (تحقق مزدوج : التردد كيعطي $LC$ والقمة كتعطي $R+r$ !)

## R3 — TYPE-BAC (bande passante + $Q$ + surtension + puissance)

🏷️ matière=PC · année=— · session=— · chapitre=P8 · type=ENTRAÎNEMENT · fidélité=n.a. · niveau=— · barème=—
**Enonce :** Meme circuit qu'en R2 ($f_0 = 159$ Hz, $I_{max} = 0{,}20$ A). Sur la courbe, $I = I_{max}/\sqrt{2} = 0{,}141$ A en $f_1 = 139$ Hz et $f_2 = 179$ Hz. (a) $\Delta f$, $Q$ (2 methodes !). (b) $U_{Ceff}$ a la resonnance ($U_{eff} = 7{,}07$ V). (c) $P_{max}$.

**Corrige :**
(a) $\Delta f = 179 - 139 = \boxed{40\,Hz}$. **Methode 1** : $Q = f_0/\Delta f = 159/40 = \boxed{4{,}0}$. **Methode 2** : $Q = L\omega_0/(R+r) = 0{,}20 \times 1000/50 = \boxed{4{,}0}$ ✅.
(b) $U_{Ceff} = Q \cdot U_{eff} = 4{,}0 \times 7{,}07 = \boxed{28\,V}$ — 4× la tension du generateur (surtension !).
(c) $I_{eff} = 0{,}20/\sqrt{2} = 0{,}141$ A ; $P_{max} = U_{eff}I_{eff}\cos 0 = 7{,}07 \times 0{,}141 = \boxed{1{,}0\,W}$ (= $(R+r)I_{eff}^2 = 50 \times 0{,}02 = 1{,}0$ ✔ — Joule !).
🪤 *Piege teste : $\Delta f$ lue a $I_{max}/2$ (au lieu de $I_{max}/\sqrt{2}$ !) — $-3$ dB = moitie de PUISSANCE ($I^2$), donc $I/\sqrt{2}$, pas $I/2$ !*
> بالدارجة: النطاق $= 40$ Hz و$Q = 4$ (بجوج الطرق !). **فرط التوتر** : $U_C = 28$ V (4 مرات المولد !). والاستطاعة $= 1$ W — تحقق بـ Joule ($(R+r)I_{eff}^2$) ! (النطاق كيتقرا فـ $I_{max}/\sqrt{2}$ — ماشي النص ! حيت $-3$ dB = نص **الاستطاعة** !)

## 🪤 Pieges testes par question

| Exo | Piege | Reflexe |
|---|---|---|
| R1 | $Z$ = somme simple | racine de carres + $L\omega - 1/C\omega$ ! |
| R1 | $\varphi$ signe inverse | $\varphi = \varphi_u - \varphi_i$ ! |
| R2 | $\omega_0$ lue en Hz | $f_0 = \omega_0/2\pi$ ! |
| R3 | $\Delta f$ a $I_{max}/2$ | $I_{max}/\sqrt{2}$ ($-3$ dB !) |
| R3 | $U_m$ dans $P$ | efficaces : $/\sqrt{2}$ ! |

---

## VRAIE — 2021N Ex4-II (LC socle : $T_0 = 2\pi\sqrt{LC}$ + $L = 0{,}92$ H)

🏷️ matière=PC · année=2021 · session=N · chapitre=P8 · type=VRAIE · fidélité=verbatim · niveau=— · barème=voir énoncé
LC ideal ($r = 0$) : regime periodique, $u_L + u_C = 0$ → $Lq'' + q/C = 0$. Verifier $q = Q_m\cos(2\pi t/T_0)$ (deriver 2× et injecter !) → $T_0 = 2\pi\sqrt{LC}$. Figure : $T_0 = 21$ ms → $L = T_0^2/(4\pi^2C) = (21\times10^{-3})^2/(4\times10\times12\times10^{-6}) = 0{,}92$ H ($C = 12$ μF de Ex4-I !).
🪤 *vraie : $\pi^2 \approx 10$ (AN !) ; $C$ recupere de la partie I (chainage !) ; $q''$ via cos (2 derivations !).*
> بالدارجة: اشتق جوج مرات وعوض — $T_0$ كتخرج بوحدها ! و$\pi^2 \approx 10$ كتسهل الحساب.
