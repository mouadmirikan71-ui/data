> **Pointer** : `01_Ondes_mecaniques_progressives` → P4 (R1-R3 type-bac + R4 vrai/faux-homogénéité) + 1 VRAIE (2024N Ex2 ondes eau) → corrigés-types + pièges testés.
> Périodicité ($\lambda$, phase) → `02_Ondes_mecaniques_progressives_periodiques`.
> 🏷️ Schéma de tags : `matière · année · session · chapitre · type (VRAIE/ENTRAÎNEMENT) · fidélité (verbatim/reconstitué-corrigé/n.a.) · type_question · niveau · compétence · barème`.

> 🏷️ Légende fiabilité : `type=VRAIE · fidélité=verbatim` = énoncé transcrit du sujet national intégral (Tier A) · `fidélité=reconstitué-corrigé` = vraie session, énoncé reconstitué depuis corrigé/description (Tier B) · `type=ENTRAÎNEMENT · fidélité=n.a.` = exercice généré style-bac (jamais un vrai national).

# Exercices types — Ondes mécaniques progressives (P01)

## Méthode — propagation en 4 gestes 🧭

1. **SI !** (m, s — convertir km, ms, cm).
2. Trajet simple : $\tau = x/v$ ; **écho : $/2$ !**
3. Séisme : $d = \Delta t/(1/v_S - 1/v_P)$ ($1/v$ !).
4. Contrôle : ordre de grandeur (séisme ~100 km, sonar ~10-100 m).

## R1 — ENTRAÎNEMENT (célérité + retard)

🏷️ matière=PC · année=— · session=— · chapitre=P01 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=célérité-retard · niveau=★ · compétence=formule-un · barème=—

**Énoncé.** Une perturbation parcourt une corde de $12$ m en $0{,}40$ s. a) Célérité ? b) Retard d'un point situé à $9{,}0$ m de la source ? c) Si on secoue la corde deux fois plus fort, que deviennent $v$ et l'amplitude ?

**Corrigé-type.** a) $v = d/\Delta t = 12/0{,}40 = \boxed{30\text{ m/s}}$. b) $\tau = x/v = 9{,}0/30 = \boxed{0{,}30\text{ s}}$. c) $v$ **inchangée** (propriété du milieu !), amplitude **doublée** (plus d'énergie injectée).
🪤 *Piège testé : « plus fort = plus vite » — NON : la force règle l'ÉNERGIE (amplitude), le MILIEU règle la vitesse.*
🗣️ الخلاصة : القوة كتزيد **الطاقة** (السعة) — والسرعة ديال الموجة ملك للوسط بوحدو.

## R2 — ENTRAÎNEMENT (séisme : 2 méthodes !)

🏷️ matière=PC · année=— · session=— · chapitre=P01 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=séisme-P-S · niveau=★★ · compétence=formule+système · barème=—

**Énoncé.** $v_P = 6{,}0$ km/s, $v_S = 3{,}5$ km/s. Une station mesure $\Delta t_{S-P} = 20$ s. Distance de l'épicentre ?

**Corrigé-type — Méthode 1 (formule directe).** $\Delta t = d(1/v_S - 1/v_P)$ → $d = 20/(1/3{,}5 - 1/6{,}0) = 20/(0{,}2857-0{,}1667) = 20/0{,}1190 = \boxed{168\text{ km}}$. Contrôle : $168/3{,}5 = 48$ s, $168/6 = 28$ s, $48-28 = 20$ ✓.

**Corrigé-type — Méthode 2 (système).** Poser $t_P = d/v_P$ et $t_S = d/v_S$ avec $t_S - t_P = 20$ : $d/3{,}5 - d/6{,}0 = 20$ → $d(0{,}1190) = 20$ → $\boxed{d = 168\text{ km}}$. Même verdict, démarche d'équations.
🪤 *Piège testé : $d = \Delta t(v_P - v_S) = 50$ km — FAUX : les temps se retranchent ($d/v$), pas les vitesses ! Retenir $1/v_S - 1/v_P$.*
🗣️ الخلاصة : الزمن هو اللي كيتطرح ماشي السرعة — $d$ كتخرج من **فرق المقلوبات** $1/v$.

## R3 — ENTRAÎNEMENT (sonar : le $/2$ !)

🏷️ matière=PC · année=— · session=— · chapitre=P01 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=sonar-écho · niveau=★ · compétence=aller-retour · barème=—

**Énoncé.** Sonar marin ($v = 1500$ m/s) : écho reçu $0{,}10$ s après émission. Profondeur ?

**Corrigé-type.** Aller-retour : $2d = v\Delta t$ → $d = 1500\times0{,}10/2 = \boxed{75\text{ m}}$.
🪤 *Piège testé : $d = 150$ m (oublier $/2$) — LE piège n°1 du chapitre : $\Delta t$ = aller + retour, $d$ = moitié !*
🗣️ الخلاصة : السونار كيمشي **ويجي** — الكرونو كيحسب الرحلة كاملة، والعمق هو النص : قسّم على 2.

## R4 — ENTRAÎNEMENT (vrai/faux + homogénéité, esprit 2024N/R)

🏷️ matière=PC · année=— · session=— · chapitre=P01 · type=ENTRAÎNEMENT · fidélité=n.a. · type_question=vrai-faux+homogénéité · niveau=★★ · compétence=raisonnement+dimensions · barème=—

**Énoncé.** a) Vrai ou faux (justifier) : ① « Une onde sonore est transversale dans l'air. » ② « Deux points distants de $3vT$ vibrent en phase. » ③ « Un milieu est dispersif si $v$ dépend de la fréquence. » b) On propose $v = \sqrt{g\cdot h}$ ($h$ : profondeur). Vérifier l'homogénéité.

**Corrigé-type.** a) ① FAUX : le son = compressions/dilatations = LONGITUDINALE dans l'air. ② FAUX : en phase si distance $= n\lambda = nvT$ — $3vT = 3\lambda$… **VRAI** en fait ($n = 3$ entier) ! (Le piège était dans l'énoncé : vérifier $n$ entier.) ③ VRAI : c'est LA définition (l'eau profonde est dispersive : les vagues longues vont plus vite !). b) $[g\cdot h] = (\text{m/s}^2)\times\text{m} = \text{m}^2/\text{s}^2$ → $\sqrt{}$ = m/s = $[v]$ ✓ homogène.
🪤 *Piège testé : répondre « en phase » au feeling — TOUJOURS $d/\lambda$ entier ? ($3vT = 3\lambda$ → oui !).*
🗣️ الخلاصة : الصوت **طولي** فالهوا، والتوافق = المسافة **مضاعف صحيح** للموجة، والتجانس كيتأكد بالأبعاد.

## VRAIE — 2024N Ex2 (ondes à la surface de l'eau : $v$, homogénéité, dispersif)

🏷️ matière=PC · année=2024 · session=N · chapitre=P01 · type=VRAIE · fidélité=reconstitué-corrigé · type_question=ondes-eau+homogénéité+dispersif · niveau=★★ · compétence=célérité+dimensions+culture · barème=2,5/20

> Reconstituée d'après la correction détaillée (RAFIK, scribd) — questions et démarche fidèles ; valeurs exactes à recouper sur le PDF officiel.
**Dispositif.** Cuve à ondes : perturbation à la surface de l'eau, mesure de $v$ par $v = d/\Delta t$ (chronométrer le parcours entre deux points). **Homogénéité.** Relation proposée $v = \sqrt{g\cdot h}$ : $[g\cdot h] = \text{m}^2/\text{s}^2$ → racine = m/s ✓ — la relation est **homogène** (condition nécessaire, pas suffisante !). **Milieu dispersif ?** Eau profonde : $v$ dépend de $\lambda$ (donc de $f$) → milieu **dispersif** — contrairement à l'air pour le son ($v \approx 340$ m/s constante) ou au vide pour la lumière.
🪤 *vraie : homogène ≠ démontré (l'analyse dimensionnelle ne prouve pas la formule, elle élimine les fausses !) ; « dispersif » = $v(f)$, à ne pas confondre avec « amorti ».*
🗣️ الخلاصة : الوطني 2024 سول على **التجانس** و**التشتت** — التجانس كيحيد الغالط، والتشتت = السرعة كتبدل مع التردد.

## 🪤 Pièges testés par question

| Exo | Piège | Réflexe |
|---|---|---|
| R1 | plus fort = plus vite | $v$ = milieu ; force = amplitude |
| R2 | $\Delta t(v_P-v_S)$ | $\Delta t/(1/v_S-1/v_P)$ |
| R3 | $d = v\Delta t$ | écho $\to /2$ ! |
| R4 | phase au feeling | $d/\lambda$ entier ? |
| 2024N | homogène = prouvé | homogène = possible, pas prouvé |
