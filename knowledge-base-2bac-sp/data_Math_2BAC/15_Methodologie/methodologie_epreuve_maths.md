---
chapitre: "15 - Méthodologie de l'épreuve de Maths au national"
unite: "Transverse (tous chapitres)"
filiere: "2BAC Sciences Physiques (SP/PC) - Maroc"
source: "Cadre de référence examen national + annales 2015-2025 + synthèse prof"
date_collecte: "2026-09-14"
type: "methodology"
langues: "FR + Darija + LaTeX"
---

# Méthodologie — Réussir l'épreuve de Maths au national (2BAC SP)

## 1. Ce que le correcteur veut (barème maths)

En maths le barème est **par étapes** : chaque question rapporte des points par petits bouts (formule juste, calcul intermédiaire, conclusion). Donc :
1. **Toujours écrire la formule/le théorème invoqué** avant de calculer (même si le calcul échoue, la formule = points).
2. **Numéroter exactement comme le sujet** (1.a, 1.b, 2...) — le correcteur ne doit jamais chercher.
3. **Encadrer les résultats**, conclure chaque question par une phrase.
4. **Ne jamais laisser une question blanche** : écrire l'idée de départ (figure, formule, 1ère ligne) rapporte souvent 0,25-0,5.

> بالدارجة: فالماط النقاط كيتفرقو على المراحل — حتى إلا ما كملتيش الجواب، كتب القاعدة والبداية باش تخطف النقاط ديالها. الورقة الخاوية = صفر مضمون، المحاولة = نقاط محتملة!

## 2. Les 3 structures de preuve à connaître par cœur

**a) Récurrence** (suites, inégalités, divisibilité) — plan imposé en 3 lignes :
- *Initialisation* : vérifier pour $n_0$ (le premier rang, souvent 0 ou 1).
- *Hérédité* : supposer $P(n)$ vraie, **montrer** $P(n+1)$ (les calculs sont là).
- *Conclusion* : « Donc par récurrence, $P(n)$ est vraie pour tout $n \ge n_0$. »
- Piège : oublier l'initialisation = preuve invalide = 0.

**b) Contraposée** : pour montrer « Si A alors B », montrer « Si non-B alors non-A » (ex. parité, raisonnements sur les ensembles).

**c) Absurde** : supposer le contraire, arriver à une contradiction (ex. irrationalité, unicité après existence).

Mots de liaison obligatoires : *Soit... Montrons que... Or... Donc... D'après (théorème)... On en déduit... CQFD.*

## 3. Réflexes par question-type (check-list examen)

**Limites / formes indéterminées** : ① factoriser (polynômes/rationnelles), ② quantité conjuguée (racines), ③ taux d'accroissement $\frac{f(a+h)-f(a)}{h}$ (formes avec sin/ln/exp en un point), ④ croissances comparées ($e^x$ bat $x^n$ bat $\ln x$), ⑤ encadrement/gendarmes (sin, cos, $(-1)^n$).

**Continuité / TVI** : pour « montrer que $f(x) = k$ admet une solution unique sur $I$ » → ① $f$ **continue** sur $I$ (à justifier !), ② $f$ **strictement monotone** sur $I$, ③ $k$ compris entre les limites/bornes → conclusion corollaire du TVI. Oublier la continuité = question ratée.

**Étude de fonction** : domaine → limites aux bornes → dérivée + signe → tableau de variations → branches infinies/asymptotes → graphe. Toujours justifier le signe de $f'$ (pas « on voit que »).

**Suites** : ① nature (arithmétique ? géométrique ? récurrente ?) → ② monotonie (différence $u_{n+1}-u_n$ ou quotient si termes $> 0$, ou récurrence) → ③ convergence (bornée + monotone, ou point fixe pour $u_{n+1} = f(u_n)$ : **vérifier $f$ continue** puis passer à la limite $l = f(l)$) → ④ limite + interprétation.

**Complexes** : forme algébrique pour $+$ et $\times$ ; **module/argument** pour $\div$, puissances, équations géométriques. $|z| = r$, $\arg(z) = \theta$ : toujours préciser $\theta$ modulo $2\pi$. Lieux : $|z - a| = r$ = cercle ; $|z-a| = |z-b|$ = médiatrice.

**Intégrales** : ① primitive directe ? ② IPP ($\int u'v$) avec $u, v$ bien choisis (ln/arctan en $v$, polynômes/exp en dérivation) ? ③ aire = intégrale de (courbe du haut − courbe du bas) **en valeur absolue si signe douteux**. Toujours vérifier la continuité sur le segment.

**Probas** : **arbre pondéré d'abord** (même au brouillon), définir les événements avec lettres ($A$ : « ... »), formules : $P(A\cap B) = P(A)\times P_A(B)$, probas totales, Bayes si demandé. Loi binomiale : justifier les 3 conditions (épreuves répétées, indépendantes, 2 issues) avant $\mathcal{B}(n,p)$.

**Géométrie espace** : vecteur normal $\vec{n}$ d'un plan $ax+by+cz+d = 0$ = $(a,b,c)$ ; produit scalaire $= 0$ ⟺ orthogonalité ; produit vectoriel $\vec{u}\wedge\vec{v}$ = vecteur normal aux deux ; distance point-plan $d = \frac{|ax_0+by_0+cz_0+d|}{\sqrt{a^2+b^2+c^2}}$.

## 4. Erreurs qui coûtent le plus cher (top 10 vu dans les copies)

1. Diviser par une expression sans vérifier qu'elle est non nulle. 2. $\sqrt{a^2} = a$ (faux si $a<0$ : c'est $|a|$). 3. Simplifier une limite FI en « remplaçant » sans lever l'indétermination. 4. Dérivée de composée fausse : $(f\circ g)' = g' \times f'\circ g$ (ne pas oublier le $g'$ !). 5. Oublier $+C$ / confondre primitive et intégrale définie. 6. Appliquer le TVI sans continuité ni monotonie. 7. $\ln(ab) = \ln a + \ln b$ avec $a,b \le 0$ (conditions !). 8. Module d'un produit/somme : $|z_1 + z_2| \neq |z_1| + |z_2|$ (inégalité triangulaire !). 9. Probas : confondre $P_A(B)$ et $P_B(A)$. 10. Copier la question suivante comme « admise » sans le dire — **si tu admets un résultat, écris « admis »** et continue (les points des questions suivantes restent gagnables !).

## 5. Gestion des 3 heures (plan de bataille)

| Bloc | Temps | Conseil |
|---|---|---|
| Lecture totale + ordre perso | 10 min | Commencer par l'exercice le mieux maîtrisé (confiance + points rapides) |
| Exercice « fort » (souvent complexes/probas/géo) | 30-35 min | Verrouiller les points faciles |
| 2e exercice moyen | 30-35 min | Idem |
| **Problème d'analyse** (le gros) | 60-70 min | Avancer question par question ; admettre et continuer si bloqué |
| Dernier exercice + relecture | 25-30 min | Vérifier calculs, encadrés, copies des énoncés |

> بالدارجة: القاعدة الذهبية — **ما تحبسش!** إلا وحلتي فسؤال، كتب «نفترض النتيجة» وكمل اللي موراه، حيت الأسئلة اللاحقة غالباً مستقلة والنقاط ديالها ما كيضيعوش. والتحليل (المسألة الكبيرة) خصو أكبر وقت — ما تخليهش للخر ملي كتكون عيان.

## 6. Rédaction modèle (à copier)

- Annoncer : « Soit $f$ définie sur $I$ par... Montrons que... »
- Justifier chaque étape : « car... », « d'après le théorème de... », « puisque ... > 0 ».
- Conclure : « Donc $\boxed{\lim_{x\to+\infty} f(x) = ...}$ » / « L'équation admet une unique solution $\alpha \in I$. »
- Figure : repère + courbe + éléments cités (asymptotes, points), titre si demandée.

*Fiches réflexes détaillées par chapitre : voir `EXERCICES_TYPES.md` de chaque chapitre (Phase 2-4).*
