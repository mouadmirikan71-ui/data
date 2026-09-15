---
chapitre: "04 - Décroissance radioactive"
unite: "Physique S1 - Noyau"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Synthèse prof (canon national : Soddy, N=N0e^-λt, activité, t1/2, datation) + scission P04/P05 v2"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v2 - élevé (§9+§10+§11)"
---

# Chapitre 04 — Décroissance radioactive

> 📋 **Exigible au bac (SI + nucléaire !)** : $^A_ZX$ ($A = Z+N$, isotopes = même $Z$) ; Soddy : $\alpha$ ($A-4$, $Z-2$), $\beta^-$ ($A$ fixe, $Z+1$), $\beta^+$ ($A$ fixe, $Z-1$), $\gamma$ ($A$/$Z$ inchangés !) ; $\boxed{N(t) = N_0e^{-\lambda t}}$ ; activité $\boxed{A(t) = \lambda N(t)}$ (Bq = dés/s) ; $\boxed{t_{1/2} = \ln2/\lambda}$ ; après $n$ demi-vies : $N_0/2^n$ ; datation : $t = -\ln(N/N_0)/\lambda$.

## 1. Accroche — l'horloge qui ne s'arrête jamais ⏳☢️

Ötzi (la momie des glaces, 5300 ans) : comment connaît-on son âge ? Son carbone-14, mort avec lui, décroît avec une demi-vie de 5730 ans — **le noyau est une horloge qu'on ne peut ni arrêter ni dérégler** (ni chaleur, ni pression, ni chimie !). Tout le chapitre : *écrire les désintégrations (Soddy), compter les survivants ($N = N_0e^{-\lambda t}$), lire l'heure ($t_{1/2}$, datation).* Le RÉCIT (dangers, déchets, C-14/K-Ar) : SVT S09 ; ici : les ÉQUATIONS.

> بالدارجة : أوتزي (المومياء، 5300 عام) : كيفاش عرفنا عمرو ؟ الكربون-14 ديالو، اللي مات معاه، كيتناقص بنصف عمر 5730 عام — **النواة ساعة ما كتوقف ما كتخربق** (لا حرارة، لا ضغط، لا كيمياء !). كاع الفصل : *كتب التفككات (سودي)، حسب الناجين ($N = N_0e^{-\lambda t}$)، قرا الساعة ($t_{1/2}$، التأريخ).* القصة (الأخطار، النفايات) : SVT S09 ؛ هنا : **المعادلات**.

## 2. Résumé du cours (exigible au bac)

**Noyau et stabilité.** $^A_ZX$ : $Z$ protons, $N = A-Z$ neutrons, $A$ nucléons. Isotopes : même $Z$, $A$ différent. Diagramme $(N,Z)$ : vallée de stabilité ($N \approx Z$ légers, $N > Z$ lourds) ; en dehors → radioactif ($\alpha$ si trop lourd, $\beta^-$ si trop de neutrons, $\beta^+$ si trop de protons).

**Équations (Soddy).** Conservation de $A$ ET $Z$ des deux côtés : $\alpha$ : $^A_ZX \to ^{A-4}_{Z-2}Y + ^4_2He$ ; $\beta^-$ : $^A_ZX \to ^A_{Z+1}Y + ^0_{-1}e$ ($n \to p$ : $A$ INCHANGÉ !) ; $\beta^+$ : $^A_ZX \to ^A_{Z-1}Y + ^0_{+1}e$ ($p \to n$) ; $\gamma$ : $^A_ZX^* \to ^A_ZX + \gamma$ (désexcitation, $A$/$Z$ inchangés — le $\gamma$ est un photon !).

**Loi de décroissance (maths !).** $\boxed{N(t) = N_0e^{-\lambda t}}$ (même EDL que M10 : $N' = -\lambda N$ !) ; activité $\boxed{A(t) = \lambda N(t)}$ (Bq = désintégrations/s) — $A$ suit la MÊME loi : $A = A_0e^{-\lambda t}$ ; $\boxed{t_{1/2} = \ln2/\lambda}$ (M05 !) ; après $n$ demi-vies : $N_0/2^n$, $A_0/2^n$. ⚠️ $A$ (activité, Bq) vs $A$ (nucléons, entier) : même lettre, 2 sens — lire l'UNITÉ !

**Datation.** $t = -\ln(N/N_0)/\lambda = -t_{1/2}\ln(N/N_0)/\ln2$ : mesurer la fraction restante ($^{14}$C, K-Ar — voir S09) → remonter au temps écoulé. Asymptote : jamais zéro (il RESTE toujours $1/2^n$) !

> ➡️ Masse-énergie ($E = \Delta mc^2$, $E_L/A$, fission/fusion) : chapitre **P05**.

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**النواة والاستقرار :** $^A_ZX$ : $Z$ بروتونات، $N = A-Z$ نيوترونات. النظائر : نفس $Z$. مخطط $(N,Z)$ : وادي الاستقرار ($N \approx Z$ للخفاف، $N > Z$ للثقال) ؛ برا ← مشع (ألفا إلا ثقيل بزاف، بيتا- إلا نيوترونات زايدة، بيتا+ إلا بروتونات زايدة).

**المعادلات (سودي) :** انحفاظ $A$ **و** $Z$ في الجهتين : ألفا ($A-4$، $Z-2$) ؛ بيتا- ($A$ ثابت !، $Z+1$) ؛ بيتا+ ($Z-1$) ؛ غاما : إزالة إثارة ($A$/$Z$ ثابتين — الغاما فوتون !).

**قانون التناقص (رياضيات !) :** $\boxed{N(t) = N_0e^{-\lambda t}}$ (نفس معادلة M10 !) ؛ النشاط $\boxed{A = \lambda N}$ (بكريل = تفكك/ث) — $A$ كيتبع نفس القانون : $A = A_0e^{-\lambda t}$ ؛ $\boxed{t_{1/2} = \ln2/\lambda}$ (M05 !) ؛ من بعد $n$ أنصاف : $N_0/2^n$. ⚠️ $A$ (النشاط) ماشي $A$ (النويات) — شوف الوحدة !

**التأريخ :** $t = -\ln(N/N_0)/\lambda$ : قيس الكسر الباقي ← رجّع الزمن. النهاية : ما كيوصلش للصفر أبداً (كيبقى ديما $1/2^n$) !

## 4. How to understand this chapter the easy way 🎯

*(النسخة الكاملة خطوة بخطوة بالدارجة : voir `COMPRENDRE_FACILEMENT.md` — 5 étapes : Soddy → exponentielle → $t_{1/2}$ → datation → restant vs désintégré.)*

**En 30 secondes :** ① Soddy : $A$ et $Z$ des 2 côtés ($\beta$ : $A$ fixe ! $\gamma$ : rien ne change). ② $N = N_0e^{-\lambda t}$, $A = \lambda N$ (même loi !). ③ $t_{1/2} = \ln2/\lambda$, fraction $1/2^n$. ④ Datation : $t = -\ln(N/N_0)/\lambda$. ⑤ Désintégré = $1 - 1/2^n$ (pas $1/2^n$ !).

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| $^A_ZX$ / isotopes | النويدة / النظائر | $A = Z+N$ ; même $Z$ |
| Vallée de stabilité | وادي الاستقرار | $(N,Z)$ stables (Soddy pour le reste !) |
| $\alpha$ / $\beta^-$ / $\beta^+$ / $\gamma$ | ألفا / بيتا- / بيتا+ / غاما | $(A-4,Z-2)$ / $(A,Z+1)$ / $(A,Z-1)$ / rien |
| $\lambda$ / $t_{1/2}$ / Bq | ثابت التناقص / النشاط | $t_{1/2} = \ln2/\lambda$ ; Bq = dés/s |
| Datation | التأريخ | $t = -\ln(N/N_0)/\lambda$ |

## 6. FAQ du chapitre

Voir `FAQ.md` (6 questions FR + Darija) : 1. $\beta^-$ : $A-1$ ? 2. $\gamma$ change $A$/$Z$ ? 3. $A$ (Bq) ou $A$ (nucléons) ? 4. Tout parti après 2 demi-vies ? 5. Désintégré = 75 % ou 25 % ? 6. Principe de la datation ?

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **$\beta^-$ : « $A-1$ »** : non ! $A$ INCHANGÉ ($n \to p$ : un nucléon reste un nucléon), seul $Z$ change (+1).
- 🪤 **$t_{1/2}$ : « tout parti après 2 demi-vies »** : $1/4$ RESTE ! (Asymptote : jamais zéro.)
- 🪤 **« Désintégré à $2t_{1/2}$ = 25 % »** : NON — RESTANT = 25 %, DÉSINTÉGRÉ = 75 % ($1 - 1/2^n$ !). Le bac adore (2023N !).
- 🪤 **$\lambda$ en an$^{-1}$ pour $N_0 = A_0/\lambda$** : avec $A_0$ en Bq (s$^{-1}$), convertir $\lambda$ en s$^{-1}$ ! (VRAIE 2021N.)
- Mots-clés : *Soddy ($A$ ET $Z$), $A$ fixe en $\beta$, $1/2^n$, $t_{1/2} = \ln2/\lambda$, restant vs désintégré, $\lambda$ en s$^{-1}$.*

## 8. Sources de ce chapitre

Voir `SOURCES.md` (canon national : Soddy, décroissance, datation — synthèse prof ; vraies 2021N Ex3, 2023N Ex2-P1 ; récit S09, maths M05/M10).

## 9. Le « pourquoi » profond — pourquoi l'exponentielle 🔬

**Pourquoi $N = N_0e^{-\lambda t}$ ?** Chaque noyau a une probabilité $\lambda\,dt$ de se désintégrer pendant $dt$ — CONSTANTE (le noyau « ignore son âge » : sans mémoire !). Donc $dN = -\lambda N\,dt$ → $N' = -\lambda N$ → exponentielle (M10 !). **La décroissance est exponentielle parce que chaque noyau joue à pile ou face à chaque instant, indépendamment de son passé.**

**Pourquoi $t_{1/2} = \ln2/\lambda$ ?** $N_0/2 = N_0e^{-\lambda t}$ → $1/2 = e^{-\lambda t}$ → $-\ln2 = -\lambda t$ → $t = \ln2/\lambda$ (M05 : le $\ln$ « défait » l'exponentielle). **$t_{1/2}$ ne dépend ni de $N_0$ ni du passé : propriété intrinsèque du noyau.**

**Pourquoi peut-on dater ?** $\lambda$ est INALTÉRABLE (ni $T$, ni $P$, ni chimie : le noyau vit à des énergies ×1 million de la chimie !) → l'horloge ne se dérègle jamais. Mesurer $N/N_0$ (ex. $^{14}$C/$^{12}$C) = lire l'heure depuis la mort de l'organisme. **Dater = lire une horloge que personne ne peut truquer.**

**Liens croisés :** M10 — EDL $y' = ay$ (les MÊMES maths !) ; M05 — $\ln$ ; S09 — datations $^{14}$C/K-Ar, déchets, sûreté (le RÉCIT) ; P05 — l'énergie libérée (où va la masse perdue ?) ; médecine — $^{131}$I, $^{99}$Tc (imagerie).

## 10. Les 3 confusions qui coûtent des points 😵

**1. « $\beta^-$ : $A-1$ (un neutron part). »** Non : le neutron se TRANSFORME en proton ($n \to p + e^-$) : il RESTE dans le noyau ! $A$ inchangé, $Z$ +1. **Le déclic :** *$\beta^-$ = changement d'uniforme (neutron → proton), pas expulsion — l'effectif $A$ ne bouge pas.*

**2. « Après 2 demi-vies, tout est parti. »** Non : $1/2^2 = 1/4$ RESTE. Et à $t = 2t_{1/2}$ : DÉSINTÉGRÉ = 75 %, RESTANT = 25 %. **Le déclic :** *$1/2^n$ = les SURVIVANTS ; les morts = $1 - 1/2^n$. Le bac demande les morts en espérant que tu donnes les survivants (2023N !).*

**3. « $\gamma$ change $A$ ou $Z$. »** Non : le $\gamma$ est un PHOTON (zéro nucléon !) : $A$/$Z$ inchangés, seule l'ÉNERGIE baisse (désexcitation). **Le déclic :** *$\gamma$ = la sueur du noyau (il se refroidit, il ne maigrit pas en nucléons).*

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** atomes ($A$, $Z$), S09 (récit : $\alpha$/$\beta$/$\gamma$, $t_{1/2}$), M10 ($e^{-\lambda t}$), M05 ($\ln$), puissances de 10. **Test 30 s :** $^{14}_6C$ ($\beta^-$) → ? ($^{14}_7N$) ; $1/2^4$ ? ($1/16$) ; $t_{1/2} = 8$ j, $A_0 = 800$ → $A$ après 24 j ? ($100$).

**Plan B — Soddy + décroissance sans faute :** ① écrire la réaction, VÉRIFIER $A$ et $Z$ des 2 côtés ② $t_{1/2} \leftrightarrow \lambda$ ($\ln2$ !) en unités cohérentes (s !) ③ $1/2^n$ si $t = n\,t_{1/2}$, sinon $e^{-\lambda t}$ ④ restant ($1/2^n$) vs désintégré ($1 - 1/2^n$) : relire la question ! ⑤ datation : $t = -\ln(N/N_0)/\lambda$.

**Fiche réflexes :** *Soddy : $A$ ET $Z$ · $\beta$ : $A$ fixe · $\gamma$ : rien · $1/2^n$ = survivants · $t_{1/2} = \ln2/\lambda$ · $\lambda$ en s$^{-1}$ !*
