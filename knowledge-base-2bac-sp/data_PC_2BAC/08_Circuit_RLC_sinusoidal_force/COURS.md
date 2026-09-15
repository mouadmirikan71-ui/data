---
chapitre: "08 - Circuit RLC sinusoidal force"
unite: "Physique S1 - Electricite"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthese prof (style national PC) - v2 force (refonte programme officiel)"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - RLC FORCE (impedance, resonnance, bande passante)"
---

# Chapitre 08 — Circuit RLC serie en regime sinusoidal force

> **Pointer** : `08_Circuit_RLC_sinusoidal_force` → P4 (impedance, dephasage, resonnance, bande passante, surtension) → COURS + EXERCICES_TYPES.

> 📋 **Exigible au bac (SI !)** : $u(t) = U_m\cos(\omega t)$ imposee, $i(t) = I_m\cos(\omega t - \varphi)$ (MEMe $\omega$ !) ; $\boxed{Z = U_m/I_m = \sqrt{(R+r)^2 + (L\omega - 1/C\omega)^2}}$ ; $\boxed{\tan\varphi = (L\omega - 1/C\omega)/(R+r)}$ ($\varphi = \varphi_u - \varphi_i$ !) ; RESONANCE : $\boxed{L\omega_0 = 1/C\omega_0}$ donc $\boxed{\omega_0 = 1/\sqrt{LC}}$ (la MEME qu'en libre !), $Z_{min} = R+r$, $I_{max} = U_m/(R+r)$, $\varphi = 0$ ; bande passante $-3$ dB : $I \geq I_{max}/\sqrt{2}$, $\boxed{\Delta f = (R+r)/2\pi L}$ ; $\boxed{Q = f_0/\Delta f = L\omega_0/(R+r)}$ ; surtension $\boxed{U_C/U = Q}$ (a la resonnance !) ; $\boxed{P = U_{eff}I_{eff}\cos\varphi}$ (max a la resonnance !).

## 0. Socle — les oscillations LIBRES (prerequis, bref !)

- **LC ideal** ($R = 0$) : $q'' + \omega_0^2q = 0$ → $q = Q_m\cos(\omega_0t + \varphi)$, $\boxed{\omega_0 = 1/\sqrt{LC}}$, $\boxed{T_0 = 2\pi\sqrt{LC}}$. Energie $E = q^2/2C + Li^2/2$ CONSERVEE (echange $E_e \leftrightarrow E_m$).
- **RLC libre** ($R \neq 0$) : $Lq'' + Rq' + q/C = 0$ — amortissement ($dE/dt = -Ri^2$), pseudo-periodique si $R$ faible ($T \approx T_0$).
- **Passage au force** : au lieu de charger le condensateur puis de laisser mourir, on branche un GBF qui impose $u(t) = U_m\cos(\omega t)$ EN PERMANENCE. Le circuit ne choisit plus sa frequence : il repond a $\omega$ IMPOSEE. La question du chapitre : **comment $I_m$ et $\varphi$ dependent-ils de $\omega$ ?** (Reponse : Tout explose... a $\omega_0$ !)

## 1. Accroche — le bouton de la radio 📻

**FR :** Tourne le bouton d'un vieux poste radio : parasites... parasites... puis SOUDAIN une station claire ! Tu viens de faire de la physique : le circuit RLC du poste ne « entend » bien qu'UNE frequence — quand la frequence de l'emetteur COINCIDE avec sa frequence propre $\omega_0$, le courant devient ENORME (resonnance !) et les autres stations (autres frequences) restent inaudibles. Tout le chapitre = pourquoi le circuit prefere UNE frequence, et comment le rendre plus selectif (bande passante fine !). Meme idee : pousser une balancoire — au bon rythme elle monte haut, au hasard elle ne bouge pas !

**بالدارجة:** دوّر الزر ديال الراديو القديم : تشويش... تشويش... وفجأة محطة واضحة ! درتي الفيزياء : الدائرة RLC ديال الراديو ما كتسمع مزيان غير **تردد واحد** — ملي تردد المحطة كيطابق التردد الخاص $\omega_0$، التيار كيكبار بزاف (**الرنين** !) والمحطات الاخرى ما كتسمعش ! هاد الفصل = علاش الدائرة كتفضل تردد واحد، وكيفاش نخليوها انتقائية (نطاق ضيق !). نفس الفكرة : دفع الارجوحة — بالايقاع الصحيح كطلع فوق، عشوائياً ما كتحركش !

## 2. Resume du cours (exigible au bac)

### 2.1 Regime force : le circuit obeit a $\omega$
- GBF impose $\boxed{u(t) = U_m\cos(\omega t)}$ aux bornes du RLC serie ($R$ + bobine $r, L$ + condensateur $C$).
- En regime PERMANENT (transitoire eteint), TOUT oscille a $\omega$ : $\boxed{i(t) = I_m\cos(\omega t - \varphi)}$ — meme pulsation, amplitude $I_m$ et DEPHASAGE $\varphi$ a determiner !
- Maille : $u = u_R + u_L + u_C = (R+r)i + L\,di/dt + q/C$ (EDL ordre 2 avec SECOND MEMBRE $U_m\cos\omega t$ — maths M10 !).

### 2.2 Impedance $Z$ et dephasage $\varphi$
- $\boxed{Z = U_m/I_m = U_{eff}/I_{eff} = \sqrt{(R+r)^2 + (L\omega - 1/C\omega)^2}}$ (en $\Omega$ !). $Z$ = la « resistance generalisee » — elle depend de $\omega$ !
- $\boxed{\tan\varphi = \frac{L\omega - 1/C\omega}{R+r}}$, avec $\boxed{\varphi = \varphi_u - \varphi_i}$ (de combien $u$ est EN AVANCE sur $i$).
- 3 comportements : $L\omega > 1/C\omega$ → **inductif** ($\varphi > 0$, $u$ en avance) ; $<$ → **capacitif** ($\varphi < 0$, $u$ en retard, $i$ en avance !) ; $=$ → **resistif** ($\varphi = 0$) = RESONANCE !
- Fresnel (construction) : vecteurs $\vec{U}_R$ (avec $\vec{I}$), $\vec{U}_L$ ($+\pi/2$), $\vec{U}_C$ ($-\pi/2$) ; $\vec{U} = \vec{U}_R + \vec{U}_L + \vec{U}_C$ → $U_m^2 = [(R+r)I_m]^2 + [(L\omega - 1/C\omega)I_m]^2$ (Pythagore = $Z$ !).

### 2.3 Resonnance d'intensite ($\omega = \omega_0$)
- $I_m = U_m/Z$ maximale quand $Z$ MINIMALE → $L\omega - 1/C\omega = 0$ → $\boxed{\omega_0 = 1/\sqrt{LC}}$, $\boxed{f_0 = 1/2\pi\sqrt{LC}}$ — **LA MEME qu'en oscillations libres !** Le circuit repond le mieux a sa frequence propre !
- A la resonnance : $\boxed{Z_{min} = R+r}$ (L et C s'annulent !), $\boxed{I_0 = I_{max} = U_m/(R+r)}$, $\boxed{\varphi = 0}$ ($u$ et $i$ EN PHASE !).
- Courbe $I(f)$ : CLOCHE centree sur $f_0$ (fine si $R+r$ petit, large sinon) — c'est elle qu'on releve au bac (R2 : 2 methodes !).

### 2.4 Bande passante et facteur de qualite
- **Bande passante a $-3$ dB** : l'intervalle $[f_1, f_2]$ autour de $f_0$ ou $\boxed{I \geq I_{max}/\sqrt{2}}$ (puissance moitie ! $-3$ dB = divise par 2 — lien P09 !).
- Largeur : $\boxed{\Delta f = f_2 - f_1 = (R+r)/2\pi L}$ (en Hz !). Petite $R$ → bande FINE → circuit SELECTIF (bonne radio !).
- **Facteur de qualite** : $\boxed{Q = f_0/\Delta f = L\omega_0/(R+r) = \frac{1}{R+r}\sqrt{L/C}}$ (sans unite !). $Q$ grand = pic fin = selectif.
- **Surtension** : a la resonnance, $\boxed{U_{Cm} = Q \cdot U_m}$ (et pareil pour la bobine !) — la tension aux bornes du condensateur peut DEPASSER la tension du generateur ($Q = 10$ → $10\times$ plus !). L et C echangent une grosse energie pendant que le GBF ne fournit que les pertes !

### 2.5 Puissance moyenne
- $\boxed{P = U_{eff}I_{eff}\cos\varphi}$ (en W !), $\cos\varphi$ = **facteur de puissance**. Seule $R+r$ consomme (Joule) ; L et C stockent/restituent (moyenne nulle !).
- A la resonnance : $\varphi = 0$ → $\cos\varphi = 1$ → $\boxed{P_{max} = U_{eff}I_{eff}}$ — TOUTE la puissance passe (ideal EDF : $\cos\varphi \approx 1$ !).
- $U_{eff} = U_m/\sqrt{2}$, $I_{eff} = I_m/\sqrt{2}$ (sinus !) — le voltmetre en AC affiche les EFFECTIVES !

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الفكرة الكبيرة:** الدائرة RLC = **راديو** ! كتسمع مزيان غير التردد اللي كيطابق التردد الخاص ديالها ($\omega_0 = 1/\sqrt{LC}$) — ملي كيطابق، التيار كيكبار بزاف (**الرنين**) ! والانتقائية = النطاق الضيق ($Q$ كبير) !

1. **النظام القسري:** المولد GBF كيفرض $u = U_m\cos(\omega t)$ — الدائرة ما كتختارش التردد، كتجاوب بنفس $\omega$ : $i = I_m\cos(\omega t - \varphi)$. السؤال : شحال $I_m$ وشحال $\varphi$ ؟
2. **المعاوقة $Z$:** $Z = U_m/I_m = \sqrt{(R+r)^2 + (L\omega - 1/C\omega)^2}$ — « مقاومة معممة » كتبدل مع التردد ! و$\tan\varphi = (L\omega - 1/C\omega)/(R+r)$ : موجب = تحريضي ($u$ سابقة)، سالب = سعوي ($i$ سابقة)، صفر = **رنين** !
3. **الرنين ($\omega = \omega_0$):** $L\omega_0 = 1/C\omega_0$ ← $Z$ صغرى ($= R+r$) ← $I$ عظمى ← $\varphi = 0$ ($u$ و$i$ في الطور !). المنحنى $I(f)$ = **جرس** متمركز على $f_0$ !
4. **النطاق والمعامل $Q$:** النطاق $-3$ dB : $I \geq I_{max}/\sqrt{2}$، العرض $\Delta f = (R+r)/2\pi L$، $Q = f_0/\Delta f$ : $Q$ كبير = قمة رقيقة = راديو انتقائي ! و**فرط التوتر** : $U_C = Q \cdot U$ — توتر المكثف يفوت توتر المولد !
5. **الاستطاعة:** $P = U_{eff}I_{eff}\cos\varphi$ — عظمى فالرنين ($\cos\varphi = 1$). غير $R$ كتستهلك (Joule)؛ $L$ و$C$ كيخزنو ويرجعو !

## 4. How to understand this chapter the easy way 🎯
*(بصوت الأستاذ — خطوة بخطوة)*

**الخطوة 1 — شكون كيفرض التردد؟ المولد!** فالنظام الحر الدائرة كتهتز بترددها ($\omega_0$)، وفالقسري المولد كيفرض $\omega$ والدائرة **كتجاوب** بنفس $\omega$ : $i = I_m\cos(\omega t - \varphi)$. إلا عطاوك $u$ و$i$ بترددين مختلفين — مستحيل فالنظام الدائم ! (نفس $\omega$ = اول تحقق !)

**الخطوة 2 — المعاوقة $Z$ هي المقاومة اللي كتبدل.** $Z = U_m/I_m$ : التردد كيبدل $L\omega$ (كيكبر) و$1/C\omega$ (كيصغار) — الفرق بيناتهم هو اللي كيحدد $Z$ و$\varphi$. **فخ الإشارة**: $\varphi = \varphi_u - \varphi_i$ ($u$ ناقص $i$ !) — موجب يعني $u$ سابقة !

**الخطوة 3 — الرنين : فين $L$ و$C$ كيتلغاو.** $L\omega_0 = 1/C\omega_0$ ← $Z = R+r$ (صغرى !) ← $I$ عظمى ← $\varphi = 0$. **نفس $\omega_0$ ديال النظام الحر** — الدائرة كتجاوب احسن على ترددها الطبيعي (الارجوحة : دفع بالايقاع الصحيح !). المنحنى $I(f)$ = الجرس !

**الخطوة 4 — $Q$ والنطاق : الانتقائية.** $R$ صغيرة ← قمة رقيقة ← $Q$ كبير ← راديو انتقائي (محطة وحدة واضحة). **وفرط التوتر** : $U_C = Q \cdot U$ — ملي $Q = 20$ توتر المكثف 20 مرة توتر المولد ! (ماشي سحر : طاقة مخزنة كبيرة كتمشي وتجي بين $L$ و$C$ !)

**الخطوة 5 — الاستطاعة : غير $R$ كتخلص.** $P = U_{eff}I_{eff}\cos\varphi$ : $L$ و$C$ ما كيستهلكوش (كيخزنو ويرجعو — المعدل صفر !). فالرنين $\cos\varphi = 1$ ← كلشي كيدوز ! **تحقق سريع**: $P$ خاصها تساوي $(R+r)I_{eff}^2$ (Joule !) — جوج طرق لنفس النتيجة !

## 5. Definitions & formules cles (FR + Darija)

| Notion FR (LaTeX) | Enonce FR | بالدارجة |
|---|---|---|
| $u = U_m\cos\omega t$, $i = I_m\cos(\omega t-\varphi)$ | Regime force : meme $\omega$ imposee | النظام القسري : نفس التردد المفروض |
| $Z = U_m/I_m = \sqrt{(R+r)^2+(L\omega-1/C\omega)^2}$ | Impedance ($\Omega$) | المعاوقة |
| $\tan\varphi = (L\omega-1/C\omega)/(R+r)$ | Dephasage $\varphi = \varphi_u - \varphi_i$ | فرق الطور |
| $\omega_0 = 1/\sqrt{LC}$ | Pulsation de resonnance (= libre !) | نبض الرنين |
| $Z_{min} = R+r$, $I_{max} = U_m/(R+r)$, $\varphi = 0$ | Resonnance d'intensite | رنين الشدة |
| $\Delta f = (R+r)/2\pi L$ | Bande passante $-3$ dB ($I \geq I_{max}/\sqrt{2}$) | عرض النطاق |
| $Q = f_0/\Delta f = L\omega_0/(R+r)$ | Facteur de qualite (selectivite) | معامل الجودة |
| $U_{Cm} = Q \cdot U_m$ | Surtension (a la resonnance) | فرط التوتر |
| $P = U_{eff}I_{eff}\cos\varphi$ | Puissance moyenne (W) | الاستطاعة المتوسطة |

## 6. FAQ du chapitre

**Q1. Pourquoi le courant passe-t-il par un MAXIMUM a $f_0$ ?**
Parce que $I_m = U_m/Z$ et $Z$ passe par un MINIMUM ($L\omega - 1/C\omega$ s'annule : les effets opposes de $L$ et $C$ se compensent exactement !). Il ne reste que $(R+r)$ — le denominateur est le plus petit possible → $I$ le plus grand possible.
بالدارجة: حيت $Z$ كدوز من قيمة **صغرى** ($L$ و$C$ كيتلغاو — تأثيرين متعاكسين !) ← المقام صغير ← التيار كبير !

**Q2. Pourquoi la resonnance tombe-t-elle sur $\omega_0 = 1/\sqrt{LC}$ (comme en libre) ?**
Parce qu'a $\omega_0$, l'echange naturel $E_e \leftrightarrow E_m$ est SYNCHRONE avec le generateur : chaque poussee arrive au bon moment et s'AJOUTE aux precedentes (comme la balancoire !). Hors $\omega_0$, le generateur pousse a contre-rythme : $L$ et $C$ « se battent » (dephasage) et $Z$ grandit.
بالدارجة: حيت فـ $\omega_0$ التبادل الطبيعي للطاقة **متزامن** مع المولد : كل دفعة كتجي فالوقت المناسب وكتزاد ! خارج $\omega_0$ المولد كيدفع ضد الايقاع ← $L$ و$C$ كيتعاركو ← $Z$ كبيرة !

**Q3. C'est quoi physiquement la bande passante ?**
La plage de frequences que le circuit « entend bien » ($I \geq 70\%$ du max). Etroite ($Q$ grand) = SELECTIF : la radio capte UNE station et ignore les voisines. Large ($Q$ petit) = tout se melange. Au bac : la mesurer sur la courbe $I(f)$ !
بالدارجة: مجال الترددات اللي الدائرة « كتسمع مزيان » ($I \geq 70\%$). ضيق = **انتقائي** (محطة وحدة !)، واسع = كلشي مخلط !

**Q4. La surtension $U_C = Q \cdot U$ : d'ou sort l'energie supplementaire ?**
D'AUCUNE creation : a la resonnance, une GROSSE energie oscille entre $L$ et $C$ ($E_e \leftrightarrow E_m$ cumulee poussee apres poussee) — le GBF ne fournit que les petites pertes Joule a chaque cycle. $U_C$ reflete l'energie STOCKEE (grande), $U$ reflete l'apport par cycle (petit). $Q$ = le nombre d'oscillations pour dissiper le stock !
بالدارجة: ماشي خلق للطاقة ! فالرنين طاقة **كبيرة** كتمشي وتجي بين $L$ و$C$ (تراكمت دفعة بدفعة) — المولد غير كيعوض الخسارة الصغيرة ! $Q$ = شحال من اهتزازة باش يتبدد المخزون !

**Q5. $\varphi > 0$ ou $\varphi < 0$ : qui est en avance ?**
$\varphi = \varphi_u - \varphi_i$ : $\varphi > 0$ → $u$ EN AVANCE sur $i$ (inductif : la bobine « retient » le courant) ; $\varphi < 0$ → $u$ EN RETARD, $i$ en avance (capacitif : le condensateur « appelle » le courant avant). Sur l'oscillo : la courbe qui ATTEINT SON MAX EN PREMIER est en avance !
بالدارجة: $\varphi = \varphi_u - \varphi_i$ : موجب ← $u$ **سابقة** (تحريضي)، سالب ← $i$ سابقة (سعوي). فالراسم : اللي كيوصل للعظمى **اللول** هو السابق !

**Q6. Pourquoi $\cos\varphi$ s'appelle « facteur de puissance » (EDF) ?**
Parce que $P = U_{eff}I_{eff}\cos\varphi$ : a $U, I$ donnes, la puissance UTILE (facturee !) est proportionnelle a $\cos\varphi$. Moteurs inductifs ($\varphi$ grand) → $\cos\varphi$ petit → EDF doit fournir plus de courant pour la meme puissance (pertes en ligne !). D'ou les condensateurs de compensation dans l'industrie (ramener $\varphi \to 0$ !).
بالدارجة: حيت $P = U_{eff}I_{eff}\cos\varphi$ : بنفس $U$ و$I$، الاستطاعة النافعة (اللي كتخلص !) متناسبة مع $\cos\varphi$ ! المحركات التحريضية كتصغرو ← المكثفات التعويضية كترجعو قريب لـ 1 !

## 7. Pieges classiques + mots-cles ⚠️

**A ecrire absolument** : $u(t)$ et $i(t)$ avec le MEME $\omega$ ; $Z$ en **$\Omega$** ; $\varphi = \varphi_u - \varphi_i$ (signe !) ; a la resonnance : $Z_{min} = R+r$, $I_{max}$, $\varphi = 0$ ; $\Delta f$ en **Hz** ; $Q$ SANS unite ; $P$ en **W** ; $\boxed{\text{resultat}}$.
**Erreurs frequentes** : « $Z$ maximale a la resonnance » ❌ ($I$ max → $Z$ MIN !) ; $\varphi = \varphi_i - \varphi_u$ (signe inverse !) ❌ ; $\omega$ confondu avec $f$ (facteur $2\pi$ !) ❌ ; $mH$/$\mu F$ non convertis ❌ ; max ($U_m$) melange avec efficace ($U_{eff} = U_m/\sqrt{2}$ !) ❌ ; $\Delta f$ lue aux MAUVAIS niveaux ($I_{max}$ au lieu de $I_{max}/\sqrt{2}$ !) ❌.

## 8. Sources de ce chapitre
- Synthese prof v2 (refonte RLC FORCE selon programme officiel 2BAC SP : impedance, resonnance, bande passante, surtension, puissance), 2026-09-15.
- Socle oscillations libres : conservation du v1 (LC : $T_0 = 2\pi\sqrt{LC}$, amortissement, Fresnel).
- VRAIE conservee : 2021N Ex4-II (LC socle : $T_0$ + $L = 0{,}92$ H). Backfill prevu : questions RLC force verbatim du national PC.

## 9. Le « pourquoi » profond — l'ecoute selective 🔬

**Pourquoi la resonnance tombe-t-elle EXACTEMENT sur $\omega_0$ ? (la poussee synchrone)**
En libre, le circuit echange $E_e \leftrightarrow E_m$ a son rythme naturel $\omega_0$. En force, le GBF pousse a $\omega$ : si $\omega = \omega_0$, chaque apport d'energie arrive pile quand le stock est pret a le recevoir (comme pousser la balancoire au bon instant) → l'amplitude GRIMPE jusqu'a ce que les pertes Joule ($Ri^2$, qui grandissent avec $I$ !) equilibrent l'apport. Si $\omega \neq \omega_0$, le GBF pousse parfois a contretemps : une partie de son travail est DETRUITE par le desaccord (dephasage $\varphi \neq 0$ !). **Le dephasage $\varphi$ mesure le desaccord ; $\varphi = 0$ = accord parfait = resonnance.** C'est pour ca que $I$ est max ET $\varphi = 0$ AU MEME $\omega_0$ — les deux sont le meme phenomene vu sous deux angles !

**Pourquoi $Z$ est-elle minimale ? ($L$ et $C$ : deux inerties qui s'annulent)**
La bobine RESISTE aux variations rapides ($u_L = L\,di/dt$ : plus $\omega$ grand, plus elle freine) ; le condensateur RESISTE aux variations lentes ($i = C\,du/dt$ : a basse frequence il a le temps de se charger et bloque). Les deux effets sont OPPOSES en phase ($+\pi/2$ vs $-\pi/2$ chez Fresnel !) : a $\omega_0$ ils se COMPENSENT EXACTEMENT ($L\omega_0 = 1/C\omega_0$) — comme deux personnes tirant une corde en sens opposes avec la meme force : la corde ne sent rien ! Il ne reste que la vraie resistance $(R+r)$. **$Z_{min} = R+r$ = les deux freins s'annulent, il ne reste que le frottement pur.**

**Pourquoi $Q$ grand = pic fin ? (la memoire du circuit)**
$Q = L\omega_0/(R+r)$ = (energie stockee)/(energie perdue par radian). $R$ petite → le circuit « oublie » lentement (il oscille longtemps en libre !) → il est TRES exigeant sur la frequence : seul $\omega_0$ exact l'entretient (pic fin, selectif). $R$ grande → il oublie vite → il accepte une large plage (pic large, peu selectif). **La selectivite frequentielle = la memoire temporelle** (lien profond libre/force : le $R$ qui tue les libres vite elargit la cloche !). Application : tuner radio ($Q$ grand), versus enceinte large-bande ($Q$ petit).

**Ponts :** P06/P07 (RC/RL : ordre 1 SANS resonnance — il faut l'ordre 2 !) ; P14/P15 (pendule : MEME resonnance mecanique — poussees synchrones !) ; P02 (signaux periodiques : $T$, $f$, $\omega = 2\pi f$ !) ; P09 (bande passante $-3$ dB = meme log !) ; Maths M10 (EDL ordre 2 avec 2nd membre $U_m\cos\omega t$ !) ; Maths M02 (trigo : $\cos/\sin$, Fresnel = vecteurs !).

> بالدارجة: علاش الرنين بالضبط فـ $\omega_0$؟ حيت فالتردد الطبيعي كل دفعة من المولد كتجي **فالوقت المناسب** (بحال الارجوحة !) ← السعة كطلع حتى Joule ($Ri^2$) كتوازن المدخول ! وفرق الطور $\varphi$ هو مقياس **عدم الاتفاق** : $\varphi = 0$ = اتفاق تام = رنين ! وعلاش $Z$ صغرى؟ حيت $L$ (كتعاكس السرعة) و$C$ (كيعاكس البطء) **كيتلغاو** — بحال جوج كيجرو الحبل بنفس القوة فاتجاهين متعاكسين : الحبل ما كيحس بوالو ! و$Q$ كبير = ذاكرة طويلة = انتقائية حادة (راديو مزيان !).

## 10. Les 3 confusions qui coutent des points 😵

**C1. « $Z$ est maximale a la resonnance » — FAUX, c'est l'inverse !**
*Le clic :* $I_m = U_m/Z$ : $I$ MAXIMALE exige $Z$ MINIMALE ! L'intuition « resonnance = grand » s'applique au COURANT (et aux tensions $U_C$, $U_L$ !), pas a l'impedance. Retiens : **resonnance = le circuit s'OUVRE ($Z$ min), le courant SE RUE ($I$ max)**. La cloche $I(f)$ monte pendant que $Z(f)$ descend en cuvette !
بالدارجة: $I = U/Z$ : التيار عظمى ← المعاوقة **صغرى** ! الرنين = الدائرة **كتفتح** ($Z$ صغيرة) والتيار **كيهجم** ($I$ كبير) ! الجرس ديال $I$ طالع والحفرة ديال $Z$ هابطة !

**C2. $\varphi = \varphi_u - \varphi_i$ : l'ordre du calcul !**
*Le clic :* TOUJOURS $u$ MOINS $i$. Sur l'oscillo : repere qui atteint son max EN PREMIER (c'est lui « en avance »), puis $\varphi = +2\pi\,\Delta t/T$ si c'est $u$, $-2\pi\,\Delta t/T$ si c'est $i$. Le piege : calculer $|\varphi|$ juste mais avec le mauvais signe → comportement inductif/capacitif INVERSE !
بالدارجة: ديماً $u$ **ناقص** $i$ ! فالراسم : شوف شكون كيوصل للعظمى **اللول** (هو السابق)، ومن بعد $\varphi = \pm 2\pi\Delta t/T$ (+ إلا كانت $u$، − إلا كانت $i$). الغلط فالإشارة = تحريضي ولا سعوي **معكوس** !

**C3. Resonnance d'INTENSITE vs maximum de $U_C$ — presque pareil, pas pareil !**
*Le clic :* Au programme : la RESONANCE D'INTENSITE ($I$ max a $f_0$ exact). Le maximum de $U_C$ (aux bornes du condensateur SEUL) se produit a une frequence LEGEREMENT DIFFERENTE ($< f_0$) — hors programme, ne pas chercher ! Au bac : surtension $U_C = Q \cdot U$ evaluee A $f_0$ (l'approximation officielle). Si un exo parle de « resonnance » sans preciser : c'est TOUJOURS l'intensite !
بالدارجة: فالبرنامج : رنين **الشدة** ($I$ عظمى فـ $f_0$ بالضبط). عظمى $U_C$ (المكثف بوحدو) كتكون فتردد **مختلف شوية** — خارج البرنامج، ما تقلبش عليها ! فالوطني : « الرنين » بلا توضيح = **الشدة** ديماً !

## 11. Signaux adaptatifs — prerequis + plan B 🧭

**Carte des prerequis :**
1. Oscillations libres (§0 : $\omega_0 = 1/\sqrt{LC}$ — la resonnance arrive DESSUS !).
2. P06/P07 (RC/RL : mailles, $u_C = q/C$, $u_L = L\,di/dt$, energies) — le socle direct.
3. Derivees de $\cos/\sin$ (Maths M02) — $d\cos(\omega t)/dt = -\omega\sin(\omega t)$ partout !
4. Courbes et mesures : lire $T$, $U_m$, $\Delta t$ sur oscillogrammes (P02 !).

**Si $Z$ et $\varphi$ bloquent — plan B (Fresnel !) :**
Le mur : les formules $Z$/$\tan\varphi$ par cœur. **Fallback officiel** : (1) dessine Fresnel : $\vec{U}_R$ horizontal (avec $\vec{I}$), $\vec{U}_L$ vers le haut ($U_{Lm} = L\omega I_m$), $\vec{U}_C$ vers le bas ($U_{Cm} = I_m/C\omega$) ; (2) Pythagore : $U_m^2 = U_{Rm}^2 + (U_{Lm} - U_{Cm})^2$ → divise par $I_m^2$ → $Z$ SANS formule apprise ! (3) $\tan\varphi = (U_{Lm} - U_{Cm})/U_{Rm}$ — le SIGNE se LIT sur le dessin (L en haut = $+$) !
بالدارجة: إلا وحلتي فالصيغ : **ارسم فرينل** ! $U_R$ أفقي، $U_L$ الفوق، $U_C$ التحت ← فيثاغورس كيعطيك $Z$ بلا حفظ ! والإشارة **كتقرا من الرسم** ($L$ الفوق = موجب) !
