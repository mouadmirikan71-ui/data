---
chapitre: "15 - Pendule pesant et pendule de torsion"
unite: "Physique S2 - Mécanique"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (canon national : T0=2π√(J/mgd), pendule simple, T0=2π√(J/C), résonance) + scission P14/P15 v2"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - élevé (§9+§10+§11)"
---

# Chapitre 15 — Pendule pesant et pendule de torsion

> 📋 **Exigible au bac (SI !)** : pesant (solide autour d'un axe, $d$ = G-axe) : $\boxed{J\ddot{\theta} + mgd\,\theta = 0}$, $\boxed{T_0 = 2\pi\sqrt{J/mgd}}$ (petits angles !) ; cas SIMPLE (masse ponctuelle, fil $l$) : $\boxed{T_0 = 2\pi\sqrt{l/g}}$ (isochronisme : ni $m$ ni amplitude !) ; TORSION (fil, cste $C$) : $\boxed{J\ddot{\theta} + C\theta = 0}$, $\boxed{T_0 = 2\pi\sqrt{J/C}}$ ; solution $\theta = \theta_m\cos(\omega_0t + \varphi)$ ; RÉSONANCE : exciter à $f \approx f_0$ → amplitude EXPLOSE.

## 1. Accroche — la balançoire et l'horloge 🕰️

Pousse une balançoire n'importe comment : elle finit toujours par se balancer à SON rythme, jamais au tien. Et l'horloge comtoise : son pendule bat la seconde depuis 300 ans avec la même régularité — parce que sa période ne dépend QUE de sa longueur. Tout le chapitre : *le pendule impose son tempo ($T_0$), la torsion aussi ($C$), et pousser au bon rythme fait exploser l'amplitude (résonance).* Le jumeau rectiligne (ressort) : P14.

> بالدارجة : دفع الأرجوحة كيفما بغيتي : في الخر كتولي تتمايل **بالإيقاع ديالها**، ماشي ديالك. وساعة الحايط : الرقاص ديالها كيدق الثانية من 300 عام بنفس الانتظام — حيت الدور ديالو معتمد غير على الطول. كاع الفصل : *الرقاص كيفرض الإيقاع ديالو ($T_0$)، والليّ حتى هو ($C$)، والدفع بالإيقاع الصحيح كيفجّر السعة (الرنين).* التوأم المستقيم (النابض) : P14.

## 2. Résumé du cours (exigible au bac)

**Pendule pesant.** Solide mobile autour d'un axe horizontal fixe (ne passant PAS par G) ; $d$ = distance G-axe ; $J$ = moment d'inertie (P13 !). Moment du poids : $M = -mgd\sin\theta \approx -mgd\,\theta$ (PETITS ANGLES : $\sin\theta \approx \theta$ !). Théorème du moment (P13 : $\sum M = J\ddot{\theta}$) → $\boxed{J\ddot{\theta} + mgd\,\theta = 0}$ → $\boxed{T_0 = 2\pi\sqrt{J/mgd}}$, $\omega_0 = \sqrt{mgd/J}$. En haut l'INERTIE ($J$), en bas le RAPPEL ($mgd$) — même logique que P14 !

**Cas particulier : pendule SIMPLE.** Masse ponctuelle $m$ au bout d'un fil $l$ : $J = ml^2$, $d = l$ → $\boxed{T_0 = 2\pi\sqrt{l/g}}$, $\omega_0 = \sqrt{g/l}$. **Isochronisme** : $T_0$ indépendante de $m$ ($m$ s'élimine — Galilée !) ET de l'amplitude (petits angles !). Pendule « seconde » : $l = 1{,}0$ m → $T_0 = 2{,}0$ s. Grands angles : $T$ augmente (isochronisme brisé !).

**Pendule de TORSION.** Disque/tige suspendu à un FIL DE TORSION (constante $C$, en N·m/rad) : moment de rappel $M = -C\theta$ → $\boxed{J\ddot{\theta} + C\theta = 0}$ → $\boxed{T_0 = 2\pi\sqrt{J/C}}$, $\omega_0 = \sqrt{C/J}$. Mêmes maths que le ressort ($J \leftrightarrow m$, $C \leftrightarrow k$ — et $g$ absent : la torsion marche même en apesanteur !).

**Solution : le cosinus (en $\theta$).** $\boxed{\theta(t) = \theta_m\cos(\omega_0 t + \varphi)}$ : $\theta_m$ (rad), $\varphi$ par conditions INITIALES (lâché sans vitesse à $\theta_m$ → $\varphi = 0$). $\dot{\theta}_{max} = \omega_0\theta_m$ (au passage par 0 !). (Détail méthode cosinus : voir P14 §4 — mêmes gestes.)

**Énergie.** Pesant : $E_p = mgl(1-\cos\theta) \approx \tfrac{1}{2}mgl\,\theta^2$ (petits angles) ; torsion : $E_p = \tfrac{1}{2}C\theta^2$ ; $E_m = E_c + E_p$ = cste (sans frottement). **Amortissement** : $T \approx T_0$, amplitude ↓.

**RÉSONANCE.** Excitateur périodique à $f \approx f_0$ → amplitude EXPLOSE : chaque apport d'énergie arrive EN PHASE ($W = F\cdot v$ maximal) et s'accumule. Balançoire poussée au bon moment ✓ ; pont de Tacoma (1940) ✗ — la résonance construit ET détruit !

**Unités SI.** $\theta$, $\varphi$ : rad. $J$ : kg·m². $d$, $l$ : m. $C$ : N·m/rad. $T_0$ : s. $\omega_0$ : rad/s.

**Énergétique torsion (tombé 2025R !).** $E_c = \tfrac12J\dot\theta^2$, $E_p = \tfrac12C\theta^2$, $E_m = E_c + E_p$ = cste (sans frottement) → $\dot\theta_{max} = \theta_m\sqrt{C/J}$ (au passage par 0). **Travail du couple** : $W_C = \Delta E_c = \tfrac{J}{2}[\dot\theta^2(t_2) - \dot\theta^2(t_1)]$ (moteur quand le pendule accélère vers 0). Chaîne nationale-type : RFD → $T_0$ graphique → $\theta_m = T_0\dot\theta_m/2\pi$ → $C = 4\pi^2J/T_0^2$ → $E_m$ → $W_C$.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**الرقاص الثقيل :** صلب كيدور حول محور أفقي ثابت (ما دايزش من G) ؛ $d$ = المسافة G-المحور ؛ $J$ = عزم القصور (P13 !). عزم الوزن : $M = -mgd\sin\theta \approx -mgd\,\theta$ (**زوايا صغار** !). مبرهنة العزم (P13) ← $\boxed{J\ddot{\theta} + mgd\,\theta = 0}$ ← $\boxed{T_0 = 2\pi\sqrt{J/mgd}}$. الفوق القصور ($J$)، التحت الإرجاع ($mgd$) — نفس منطق P14 !

**الحالة الخاصة : الرقاص البسيط.** كتلة نقطية في خيط $l$ : $J = ml^2$، $d = l$ ← $\boxed{T_0 = 2\pi\sqrt{l/g}}$. **تساوي الزمن** : $T_0$ مستقلة عن $m$ ($m$ كتحيد — غاليلي !) **وعن** السعة (زوايا صغار !). رقاص «الثانية» : $l = 1$ م ← $T_0 = 2$ ث. الزوايا الكبار : $T$ كتكبر (تكسر التساوي !).

**رقاص الليّ :** قرص معلق بسلك الليّ (الثابتة $C$) : عزم الإرجاع $M = -C\theta$ ← $\boxed{J\ddot{\theta} + C\theta = 0}$ ← $\boxed{T_0 = 2\pi\sqrt{J/C}}$. نفس رياضيات النابض ($J \leftrightarrow m$، $C \leftrightarrow k$ — و $g$ غايبة : الليّ خدام حتى بلا جاذبية !).

**الحل : الكوسينوس (بـ $\theta$).** $\boxed{\theta = \theta_m\cos(\omega_0t + \varphi)}$ : $\varphi$ من **الشروط الابتدائية** (مطلق بلا سرعة ← $\varphi = 0$).

**الرنين :** محرض دوري بـ $f \approx f_0$ ← السعة **كتنفاجر** : كل دفعة كتوصل في الطور وكتتراكم. الأرجوحة في الوقت المناسب ✓ ؛ جسر طاكوما (1940) ✗ — الرنين كيبني **وكيهدم** !

## 4. How to understand this chapter the easy way 🎯

*(النسخة الكاملة خطوة بخطوة بالدارجة : voir `COMPRENDRE_FACILEMENT.md` — 5 étapes : $J$/$mgd$ → simple → torsion → cosinus → résonance.)*

**En 30 secondes :** ① Pesant : $T_0 = 2\pi\sqrt{J/mgd}$ (P13 : $\sum M = J\ddot{\theta}$). ② Simple : $2\pi\sqrt{l/g}$ (ni $m$ ni amplitude !). ③ Torsion : $2\pi\sqrt{J/C}$ (pas de $g$ !). ④ Cosinus en $\theta$ ($\varphi$ = initiales). ⑤ Résonance : $f \approx f_0$ = explosion (phase !).

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| $J$ / $d$ (pesant) | عزم القصور / المسافة | kg·m² / m (G-axe !) |
| Isochronisme | تساوي الزمن | $T_0$ : ni $m$ ni amplitude (petits angles !) |
| $C$ (torsion) | ثابتة الليّ | N·m/rad : fil raide = $C$ grand |
| $\theta_m$ / $\varphi$ | السعة الزاوية / الطور | rad ; $\varphi$ = initiales ! |
| Résonance | الرنين | $f \approx f_0$ → amplitude explose |

## 6. FAQ du chapitre

Voir `FAQ.md` (6 questions FR + Darija) : 1. $m$ n'intervient pas ? 2. Petits angles : pourquoi ? 3. Pesant vs simple ? 4. Torsion : $C$ ? 5. Résonance : force ou rythme ? 6. Tacoma ?

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **$\sqrt{g/l}$ au lieu de $\sqrt{l/g}$** : $l$ grand (balancier d'horloge !) = LENT → $l$ au NUMÉRATEUR. Test : $l = 10$ m : lent, évidemment → $T_0$ GRAND.
- 🪤 **« $T_0 \times 6$ sur la Lune ($g \div 6$) »** : RACINE ! $T_0 \propto 1/\sqrt{g}$ → $\times\sqrt{6} = \times 2{,}45$ (voir R1).
- 🪤 **$g$ inversée (« mesurer $g$ »)** : $T_0 = 2\pi\sqrt{l/g}$ → $\boxed{g = 4\pi^2l/T_0^2}$ : $g$ au NUMÉRATEUR !
- 🪤 **« Pousser plus fort (n'importe quel rythme) »** : hors résonance, les apports se COMPENSENT au lieu de s'accumuler : le RYTHME bat la FORCE.
- Mots-clés : *petits angles ($\sin\theta \approx \theta$), $J$ (P13 !), $l$ en haut, racine ($\sqrt{}$ !), $g = 4\pi^2l/T^2$, résonance = phase.*

## 8. Sources de ce chapitre

Voir `SOURCES.md` (canon national : pesant, torsion, résonance — synthèse prof ; jumeau P14, rotation P13, EDL M10).

## 9. Le « pourquoi » profond — pourquoi le pendule bat la mesure 🔬

**Pourquoi $T_0$ indépendant de $m$ (pendule simple) ?** $m$ s'élimine : $ml^2\ddot{\theta} = -mgl\,\theta$ → les deux côtés $\propto m$. Double masse = double rappel MAIS double inertie : les deux effets se compensent EXACTEMENT. (4e apparition du principe d'équivalence — P11, P28, P14-vertical : c'est LE fil rouge de l'année !)

**Pourquoi petits angles ?** Le rappel VRAI est $-mgd\sin\theta$ (NON linéaire) ; $\sin\theta \approx \theta$ SEULEMENT si $\theta \ll 1$ rad. Au-delà, $T$ dépend de l'amplitude (l'isochronisme de Galilée a des limites — et « mesurer $g$ » à $30°$ SOUS-estime $g$ : voir R2 !).

**Pourquoi la résonance ?** Chaque poussée à $f_0$ ajoute de l'énergie EN PHASE ($W = F\cdot v$ maximal quand $F \parallel v$) : les apports s'ACCUMULENT au lieu de se compenser. Hors phase, ils s'annulent. **C'est de la synchronisation, pas de la force** — d'où Tacoma : un vent modéré mais SYNCHRONE a détruit un pont !

**Liens croisés :** P14 — jumeau rectiligne (mêmes maths !) ; P13 — rotation ($\sum M = J\ddot{\theta}$ : source des EDP) ; M10 — EDL ; P08 — résonance ÉLECTRIQUE à $f_0 = 1/(2\pi\sqrt{LC})$ (même phénomène, deux mondes !) ; SVT/géo — sismologie ($T_0$ des sols !) ; histoire — Galilée (1583, lustre de Pise !), Huygens (1656, comtoise), Tacoma (1940).

## 10. Les 3 confusions qui coûtent des points 😵

**1. « $\sqrt{l/g}$ vs $\sqrt{g/l}$. »** $l$ grand = LENT (balancier !) → $l$ au numérateur. **Le déclic :** *imagine $l = 10$ m — ça oscille lentement, évidemment : $T_0$ GRAND → $l$ en haut. Le bon sens place les lettres.*

**2. « Amplitude ↑ → $T_0$ ↑. »** Non (petits angles) : isochronisme ! Doubler l'amplitude = doubler la distance MAIS doubler la vitesse moyenne (plus d'énergie) : les deux se compensent. **Le déclic :** *la comtoise bat la seconde que le balancement soit large ou étroit — c'est POUR ÇA qu'elle donne l'heure !*

**3. « La résonance = pousser fort. »** Non : pousser fort HORS phase = compenser (une poussée sur deux freine !). **Le déclic :** *la balançoire monte quand on pousse AU BON MOMENT, même doucement — le rythme bat la force. Phase d'abord, force ensuite.*

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** P13 (moments : $M$, $J$, $\sum M = J\ddot{\theta}$), P10 (PFD — analogue), M10 (EDL), trigo ($\sin\theta \approx \theta$, rad !), racines. **Test 30 s :** $l \times 4$ → $T_0$ ? ($\times 2$ — racine ✓) ; $g \div 4$ → $T_0$ ? ($\times 2$ ✓).

**Plan B — si les moments ($J$) bloquent :** TOUT ramener au pendule SIMPLE ($T_0 = 2\pi\sqrt{l/g}$ par cœur : $l$ en haut !) + énergie ($E_m$ = cste : vitesses sans EDP) + résonance ($f = f_0$). Le pesant général et la torsion = « même film, $J$ en plus » — et $J$ est DONNÉ au bac (règle : $\tfrac{1}{3}mL^2$, disque : $\tfrac{1}{2}mR^2$).

**Fiche réflexes :** *petits angles ! · $T_0 = 2\pi\sqrt{J/mgd}$ · simple : $2\pi\sqrt{l/g}$ · torsion : $2\pi\sqrt{J/C}$ · $g = 4\pi^2l/T^2$ · résonance : $f = f_0$ · SI + rad !*
