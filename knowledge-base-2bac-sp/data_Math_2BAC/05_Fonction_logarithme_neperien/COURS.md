---
chapitre: "05 - Fonction logarithme népérien"
unite: "S2 - Analyse avancée"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "National 2020 Rattrapage Problème + 2020 Normale Ex.3 (réels, SP) + synthèse prof"
date_collecte: "2026-09-15"
type: "summary"
langues: "FR + Darija + LaTeX"
statut: "complet v1 - élevé (§9+§10+§11)"
---

# Chapitre 05 — Fonction logarithme népérien

> 📋 **Exigible au bac** : $\ln$ défini sur $]0, +\infty[$, réciproque de $\exp$ ($y = \ln x \iff x = e^y$) ; $\ln 1 = 0$, $\ln e = 1$ ; $\ln(ab) = \ln a + \ln b$, $\ln(a/b) = \ln a - \ln b$, $\ln(a^n) = n\ln a$ ; $(\ln u)' = u'/u$ ; limites ($0^+$, $+\infty$, CC) ; équations/inéquations (domaine d'abord !).

## 1. Accroche — le compteur de doublements 🧮

L'exponentielle dit : « pars de 1, multiplie par $e$, $x$ fois » ($e^x$). Le logarithme demande l'inverse : **« combien de fois faut-il multiplier par $e$ pour atteindre $x$ ? »** $\ln 10 \approx 2,3$ : il faut « $2,3$ multiplications par $e$ » pour fabriquer 10. $\ln$ est le **compteur de multiplications** — et c'est pour ça qu'il transforme les produits en sommes : compter des multiplications successives, c'est additionner.

> بالدارجة : الأسّية كتقول : «بدا من 1 وضرب في $e$، $x$ مرات». اللوغاريتم كيسوّل العكس : **«شحال من مرة خاصك تضرب في $e$ باش توصل لـ $x$ ؟»** $\ln$ هو **عدّاد الضربات** — وعلاش كيحوّل الجداء لمجموع ؟ حيت عدّ الضربات المتتابعة هو الجمع !

## 2. Résumé du cours (exigible au bac)

**Définition (2 visages).** $\ln$ est la fonction **réciproque de $\exp$** : $\boxed{y = \ln x \iff x = e^y}$ ($x > 0$). Équivalent (M04) : $\ln$ est LA primitive de $1/x$ sur $]0, +\infty[$ valant 0 en 1. Domaine : $\boxed{D = ]0, +\infty[}$ — tout le reste en découle. Valeurs : $\ln 1 = 0$, $\ln e = 1$ ; signe : $\ln x < 0$ sur $]0, 1[$, $> 0$ sur $]1, +\infty[$.

**Propriétés algébriques ($a, b > 0$).** $\boxed{\ln(ab) = \ln a + \ln b}$ ; $\boxed{\ln(a/b) = \ln a - \ln b}$ ; $\boxed{\ln(a^n) = n\ln a}$ ($n \in \mathbb{Z}$, $a > 0$) ; $\boxed{\ln\sqrt{a} = \frac{1}{2}\ln a}$ ; $\boxed{\ln(1/a) = -\ln a}$. **AUCUNE formule pour $\ln(a+b)$** — piège n°1 du bac.

**Dérivée.** $\boxed{(\ln x)' = 1/x}$ et $\boxed{(\ln u)' = u'/u}$ ($u > 0$). Conséquence : primitive de $u'/u$ = $\ln|u| + C$ (M04). Courbe : croissante, **concave** ($(\ln)'' = -1/x^2 < 0$), tangente en 1 : $y = x - 1$.

**Limites.** Références : $\boxed{\lim_{x\to 0^+} \ln x = -\infty}$, $\boxed{\lim_{x\to+\infty} \ln x = +\infty}$. Croissances comparées (contre les puissances, $\ln$ perd toujours) : $\boxed{\lim_{x\to+\infty} \frac{\ln x}{x^n} = 0}$, $\boxed{\lim_{x\to 0^+} x^n\ln x = 0}$ ($n > 0$). Taux : $\boxed{\lim_{h\to 0} \frac{\ln(1+h)}{h} = 1}$ (dérivée en 1).

**Équations / inéquations.** Méthode : ① **domaine** (chaque $\ln$ exige $> 0$ !) ; ② regrouper avec les propriétés ; ③ appliquer $\exp$ (les deux sens gardés, $\exp$ croissante) ou comparer (inéquation : $\ln$ croissante conserve l'ordre) ; ④ **vérifier l'appartenance au domaine**. Ex : $\ln(2x+1) = \ln(x+4)$ → domaine $x > -1/2$ → $2x+1 = x+4$ → $x = 3$ ✓.

**Ponts :** $\log_{10}$ en PC (pH $= -\log[H_3O^+]$) : $\log x = \ln x / \ln 10$ ; demi-vie (M10-R4) : $t_{1/2} = \ln 2/\lambda$.

**Logarithme décimal $\log$ (complément exigible).** $\boxed{\log x = \frac{\ln x}{\ln 10}}$ ($x > 0$) : réciproque de $10^t$ ($y = \log x \iff x = 10^y$). Mêmes propriétés que $\ln$ : $\log(ab) = \log a+\log b$, $\log(a^n) = n\log a$, $\log 1 = 0$, $\log 10 = 1$. Dérivée (rare) : $(\log x)' = \frac{1}{x\ln 10}$. Usage : pH $= -\log[H_3O^+]$, pKA, décibels — en PC on NE convertit jamais en $\ln$ (calculatrice : touche log !). Réflexe : $10^p$ « sort » du log en $p$ ($\log(2\times 10^{-3}) = \log 2 - 3$).

## 3. الشرح بالدارجة — الفهم قبل الحفظ 🇲🇦

**التعريف (جوج وجيه) :** $\ln$ هو **العكس ديال $\exp$** : $y = \ln x \iff x = e^y$. ولا (M04) : هو الأصلية ديال $1/x$ اللي كتسوى 0 في 1. المجال : $\boxed{D = ]0, +\infty[}$ — كلشي خارج من هنا. القيم : $\ln 1 = 0$، $\ln e = 1$ ؛ الإشارة : سالب قبل 1، موجب بعد 1.

**الخواص ($a, b > 0$) :** $\ln(ab) = \ln a + \ln b$ | $\ln(a/b) = \ln a - \ln b$ | $\ln(a^n) = n\ln a$ | $\ln\sqrt{a} = \frac{1}{2}\ln a$. **ما كايناش صيغة لـ $\ln(a+b)$** — الفخ رقم 1.

**المشتقة :** $(\ln x)' = 1/x$ و $(\ln u)' = u'/u$. المنحنى : متزايد، **مقعّر**، المماس في 1 : $y = x - 1$.

**النهايات :** في $0^+$ ← $-\infty$، في $+\infty$ ← $+\infty$. المقارنات : $\ln x / x^n \to 0$ ($+\infty$)، $x^n\ln x \to 0$ ($0^+$) — $\ln$ ديما كيخسر قدام القوى. المعدل : $\ln(1+h)/h \to 1$.

**المعادلات / المتراجحات :** ① **المجال اللول** (كل $\ln$ كيبغي $> 0$) ؛ ② جمّع بالخواص ؛ ③ طبّق $\exp$ ولا قارن ($\ln$ متزايد كيحفظ الترتيب) ؛ ④ **تحقق من المجال**.

## 4. How to understand this chapter the easy way 🎯

*(كأن الأستاذ كيشرح لك شفوياً — خطوة بخطوة)*

**الخطوة 1 — $\ln$ هو «عكس» $\exp$.** $e^2 \approx 7,4$ ←→ $\ln 7,4 = 2$. أي معادلة فيها $\exp$ كتحلّ بـ $\ln$، وأي معادلة فيها $\ln$ كتحلّ بـ $\exp$ : هما كيحيّدو بعضياتهم ($e^{\ln x} = x$، $\ln(e^y) = y$). **M05 و M07 مرايا : اللي تعلمتيه في الأسّية اقلبو.**

**الخطوة 2 — المجال مقدس.** قبل أي حساب : شنو داخل $\ln$ ؟ خاصو يكون $> 0$. $\ln(2x+1)$ ← $x > -1/2$. $\ln(x^2-1)$ ← $|x| > 1$. **80% من أخطاء التلاميذ : حلّو المعادلة ونساو المجال** (كيقبلو حلول مرفوضة). القاعدة : *المجال اللول، الحل من بعد، التحقق في اللخر.*

**الخطوة 3 — الخواص : الضرب كيولّي جمع.** $\ln(8) = \ln(2^3) = 3\ln 2$. $\ln a + \ln b = \ln(ab)$ (الاتجاهين !). تمرين نموذجي : جمّع كلشي في $\ln$ وحدة ← طبّق $\exp$ ← حلّ المعادلة العادية. وحفظ النفي : *$\ln(a+b)$ ما كيتفككش — اللي فككو سقط.*

**الخطوة 4 — النهايات : $\ln$ سلحفاة.** قدام أي قوة، $\ln$ كيربح ببطء وكيخسر : $\ln x / x \to 0$، $x\ln x \to 0$ في $0^+$. تخيّل : $\ln(1\,000\,000) \approx 14$ فقط ! **اللوغاريتم كيكبر ببطء شديد** — هاد الحدس كيحلّ كل النهايات.

**الخطوة 5 — دراسة دالة : نفس الفيلم ديما.** مجال ← نهايات ← مشتقة (غالباً $u'/u$ : الإشارة من $u'$) ← جدول ← (سؤال فرعي : معادلة $f(x) = 0$ بـ TVI ولا إشارة). إلا ضبطتي M07-Q1، M05 نفس الشي بالمرايا.

## 5. Définitions clés (FR + Darija)

| Terme FR | Darija | Sens |
|---|---|---|
| $\ln$ (réciproque de $\exp$) | اللوغاريتم النيبيري | $y = \ln x \iff x = e^y$, $D = ]0,+\infty[$ |
| $\ln 1 = 0$, $\ln e = 1$ | القيم المرجعية | repères (signe : $-$ avant 1, $+$ après) |
| $\ln(ab) = \ln a + \ln b$ | لوغاريتم الجداء | le produit → somme |
| $(\ln u)' = u'/u$ | مشتقة $\ln u$ | dérivée (signe via $u'$) |
| Concavité | التقعر | $(\ln)'' < 0$ (tangente $y = x-1$ en 1) |
| CC : $\ln x / x^n \to 0$ | المقارنة | $\ln$ perd contre les puissances |

## 6. FAQ du chapitre

**1. Pourquoi $\ln 1 = 0$ ?** $e^0 = 1$ donc $\ln 1 = 0$ (miroir). Et $\ln e = 1$ car $e^1 = e$. / المرايا : $e^0 = 1$ إذن $\ln 1 = 0$.

**2. $\ln x$ peut-il être négatif ? Oui !** Sur $]0, 1[$ : $\ln 0,5 \approx -0,69$. Ce qui est interdit, c'est $\ln$ D'UN négatif, pas un $\ln$ négatif. / إيه : $\ln 0,5 < 0$. الممنوع هو $\ln$ ديال عدد سالب، ماشي النتيجة السالبة.

**3. $(\ln x)^2$ ou $\ln(x^2)$ ?** RIEN À VOIR : $(\ln x)^2 = \ln x \times \ln x$ ; $\ln(x^2) = 2\ln|x|$. / ما كيتشابهوش : $(\ln x)^2$ مربع النتيجة، $\ln(x^2) = 2\ln|x|$.

**4. Pourquoi $(\ln x)' = 1/x$ ?** $\ln$ est défini comme la primitive de $1/x$ (valant 0 en 1) — c'est sa construction même (M04). / $\ln$ **تعرّف** كأصلية ديال $1/x$ — هادي هي البنية ديالو.

**5. $\ln$ et $\log$ (pH) ?** $\log_{10} x = \ln x / \ln 10$ (changement de base). En PC : $pH = -\log[H_3O^+]$. Même famille, base différente. / $\log x = \ln x / \ln 10$ — نفس العائلة، أساس مختلف.

**6. Comment résoudre $\ln x > 2$ ?** Domaine $x > 0$, $\ln$ croissante : $x > e^2$. Général : appliquer $\exp$ (croissante, conserve l'ordre) + vérifier le domaine. / طبّق $\exp$ : $x > e^2$ + تحقق من المجال.

## 7. Pièges classiques + mots-clés ⚠️

- 🪤 **Domaine oublié** : résoudre $\ln(x-2) + \ln(x+1) = \dots$ exige $x > 2$ D'ABORD. Solutions hors domaine = à rejeter (le bac en met toujours une !).
- 🪤 **$\ln(a+b) = \ln a + \ln b$** : FAUX, archi-faux. Aucune formule pour la somme. ($\ln(1+1) = \ln 2 \neq 0 = \ln 1 + \ln 1$ — contre-exemple en 5 s.)
- 🪤 **$\ln(a^n)$ avec $a < 0$** : $\ln(x^2) = 2\ln|x|$ — les $|~|$ sont obligatoires si $x$ peut être négatif.
- 🪤 **Signe de $(\ln u)'$** : $(2-\ln x)' = -1/x$ — le $-$ vient de la dérivée de l'intérieur composé, pas de $\ln$.
- Mots-clés : *domaine $> 0$ d'abord, regrouper puis $\exp$, $\ln$ croissante (ordre conservé), CC ($\ln$ perd), vérifier.*

## 8. Sources de ce chapitre

- National Maths SX 2020 Rattrapage Problème (réel, SP) : $g = e^{1-x}+1/x-2$, $f = (1-x)e^{1-x}-x^2+5x-3-2\ln x$ (limites, $f' = (x-2)g$, variations) — https://etude-generale.com/examen-national-math-2020-science-physique-corrige/ + National 2020 Normale Ex.3 (réel, SP) : $g = 2\sqrt{x}-2-\ln x$ ($g'$, encadrements $\ln$, CC $(\ln x)^3/x^2 \to 0$) — https://etude-generale.com/correction-dexamen-national-2020-math-science-physique/ ; + synthèse prof (canon national) ; miroir M07, outils M04, M02 (dérivées).

## 9. Le « pourquoi » profond — pourquoi $\ln$ existe 🔬

**Pourquoi l'inverse de $\exp$ mérite-t-il un nom ?** Parce que les questions inverses sont partout : « en combien de temps mon capital double-t-il ? » ($2 = e^{rt}$ → $t = \ln 2/r$) ; « de combien remonter pour diviser la pression par 10 ? » ; « quel pH pour cette concentration ? ». $\ln$ est la machine à **remonter les exponentielles** — sans lui, toute équation $e^{(\dots)} = \text{nombre}$ est insoluble. Il n'est pas un gadget : c'est la moitié manquante de M07.

**Pourquoi $(\ln)' = 1/x$ (et pas autre chose) ?** Dérivation des réciproques : si $y = \ln x$ alors $x = e^y$, dériver : $1 = e^y \cdot y'$ → $y' = 1/e^y = 1/x$. La pente de $\ln$ en $x$ est l'inverse de la pente de $\exp$ au point miroir — et comme $\exp$ monte de plus en plus vite, $\ln$ monte de plus en plus lentement (concavité, croissance « escargot »). Tout est cohérent : *pente miroir = inverse.*

**Pourquoi $\ln$ perd-il contre toutes les puissances ?** CC : $\ln x / x \to 0$. Intuition : $\ln x$ compte les multiplications par $e$ pour atteindre $x$ — pour $x = e^{1000}$ (nombre de 435 chiffres !), $\ln x = 1000$ seulement. Le compteur grandit en comptant les chiffres, pas le nombre. C'est cette lenteur qui fait de $\ln$ l'outil des échelles (pH, décibels, Richter) : **il écrase les ordres de grandeur pour les rendre lisibles.**

**Liens croisés :** M07 — miroir $\exp$/$\ln$ (propriétés, courbes symétriques par $y = x$) ; M04 — $\ln$ né comme primitive de $1/x$ ; M02 — $(\ln u)' = u'/u$ partout dans les études ; M10 — $t_{1/2} = \ln 2/\lambda$ ; PC — pH, décibels, datation ($t = -\ln(N/N_0)/\lambda$).

## 10. Les 3 confusions qui coûtent des points 😵

**1. « $\ln(a + b) = \ln a + \ln b$. »** Le piège n°1. **Le déclic :** teste avec $a = b = 1$ : $\ln 2 \approx 0,69 \neq 0$. *Le $\ln$ distribue sur $\times$, jamais sur $+$.* Cinq secondes de test numérique tuent le réflexe à vie.

**2. « $\ln x^2 = 2\ln x$. »** Seulement si $x > 0$ ! Si $x < 0$, $\ln x$ n'existe pas mais $\ln(x^2)$ si. **Le déclic :** écris systématiquement $\ln(x^2) = 2\ln|x|$ — les barres coûtent rien et sauvent tout.

**3. « $(\ln x)' = 1/x$ donc primitive de $1/x$ = ... euh. »** Les deux sens se mélangent. **Le déclic :** $(\ln|x|)' = 1/x$ (dériver) ⟺ $\int 1/x = \ln|x| + C$ (primitiver) — *même égalité lue à l'envers.* Si tu sais l'un, tu sais l'autre.

## 11. Signaux adaptatifs — prérequis + plan B 🧭

**Prérequis :** $\exp$ (M07 : miroir, $e^{\ln x} = x$), dérivées composées (M02 : $(u^n)'$, $(e^u)'$ → $(\ln u)'$ pareil), équations (collège). **Test 30 s :** $e^{\ln 5}$ → $5$ ; $\ln(e^3)$ → $3$ ; $(\ln(2x+1))'$ → $2/(2x+1)$.

**Plan B — le plus dur (l'étude de fonction $\ln$ au bac) :** déroule le film : ① domaine ($> 0$ !) ② limites (bornes : $0^+$ → $-\infty$ ? $+\infty$ → CC ?) ③ dérivée $(\ln u)' = u'/u$ → signe = signe de $u'$ ($u > 0$) ④ tableau ⑤ question cachée (souvent : signe de $f$ via $f(x_0) = 0$, ou TVI). Cinq gestes, dans l'ordre, sans réfléchir — puis rédiger.

**Fiche réflexes :** *miroir de $\exp$ · domaine $> 0$ d'abord · $\times \to +$ (jamais $+$ !) · $(\ln u)' = u'/u$ · $\ln$ perd vs $x^n$ · vérifier le domaine à la fin.*
