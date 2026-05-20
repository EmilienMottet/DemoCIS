# Démo CIS — Équipe Innovation Michelin

**Public** : scientifiques R&D (matériaux, mécanique, chimie polymères)
**Durée** : ~30 min
**Pré-requis technique** : Claude Code lancé dans ce dossier (les skills CIS apparaissent dans `/`)

---

## Pré-flight (5 min avant la démo)

```
/bmad-help
```

Vérifier que les 11 skills CIS apparaissent dans la liste. Tester aussi rapidement :

```
/bmad-cis-agent-creative-problem-solver
bonjour, présente-toi en 2 lignes
```

→ Si Dr. Quinn répond, tout est OK.

---

## Plan (30 min)

| Temps | Bloc |
|---|---|
| 2 min | Ouverture — leurs innovations cartographiées sur des méthodes connues |
| 3 min | Le toolkit en une slide |
| 20 min | Démo live — « pneu auto-cicatrisant » |
| 3 min | Reveal complet du kit |
| 2 min | Question retour ouverte |

---

## 1. Ouverture (2 min)

Phrase d'accroche :
> « Vos innovations récentes utilisent déjà — intuitivement — des méthodes d'ideation formalisées. Ce que CIS apporte, c'est de rendre la démarche **systématique, reproductible, auditable**. »

Tableau à projeter :

| Innovation Michelin | Méthode CIS sous-jacente |
|---|---|
| Gants en gomme (fauteuils roulants) | **Cross-Pollination** : transfert d'une propriété matériau vers un domaine adjacent |
| Pneu vélo airless | **TRIZ — contradiction physique** : structurellement rigide ET souple sans pression |
| Pneu agraire basse pression | **Morphological Analysis** : matrice [pression × largeur × profondeur crampons] |

---

## 2. Toolkit en une slide (3 min)

CIS = 6 agents + 4 workflows installables dans n'importe quel IDE (Claude Code, Cursor, etc.).

Pour aujourd'hui on en active **3** :

- **Dr. Quinn** — *Master Problem Solver*. Canalise Altshuller (TRIZ) et Donella Meadows (systems thinking).
- **Carson** — *Elite Brainstorming Specialist*. Méthodes : first principles, morphological analysis, cross-pollination.
- **Victor** — *Disruptive Innovation Oracle*. Innovation Ambition Matrix, Three Horizons, Disruption Theory (Christensen), Scenario Planning.

Les 3 autres (Maya, Sophia, Caravaggio) — montrés à la fin.

---

## 3. Démo live — « Pneu auto-cicatrisant » (18 min)

> **Ligne de contexte à coller en tout premier**, avant les prompts ci-dessous, pour calibrer le niveau de réponse (et éviter mode vulgarisation) :
>
> ```
> Contexte : équipe R&D industrielle, profils ingénieurs matériaux / polymères /
> mécanique pneu. Réponds à un niveau scientifique avancé (terminologie
> technique OK, pas de simplification grand public). Sois concret : pour chaque
> principe, donne un exemple matériau ou architectural exploitable en labo.
> ```
>
> Volontairement **pas de mention "Michelin"** : risque d'hallucination sur des produits/brevets internes + dérive vers un registre marketing.

### Étape 1 — Lancer Dr. Quinn (TRIZ)

```
/bmad-cis-agent-creative-problem-solver

Voici notre défi R&D : concevoir un pneu qui s'auto-cicatrise après
crevaison ou abrasion micro. Contradictions de départ :
  - il doit être structurellement rigide (tenir la charge, le profil, la pression)
  - ET capable de fluer/se reformer localement (cicatrisation)
  - sans dégrader le grip, l'usure, ni la dissipation thermique

Joue la méthode TRIZ : identifie la contradiction principale, propose 3 à 5
principes inventifs (sur les 40) applicables, et illustre chacun par un
exemple matériau ou architectural.
```

> **Attendu** : segmentation (1), dynamisation (15), changement de propriétés (35), matériaux composites (40), structures poreuses (31)… Très visuel pour des ingénieurs.

### Étape 2 — Pivot biomimétisme (même agent)

```
Maintenant méthode biomimétique : quelles stratégies de cicatrisation
observées dans le vivant pourraient inspirer la structure ou le compound ?
Pour chacune, indique le mécanisme biologique et le transfert possible.
```

> **Attendu** : peau (collagène / cellules basales), coagulation (cascade enzymatique), écorce d'arbre (callosité), byssus de moule (liaisons ioniques), os trabéculaire (porosité auto-réparante)…

### Étape 3 — Bascule vers Carson (first principles + cross-pollination)

```
/bmad-cis-agent-brainstorming-coach

On a 4-5 directions matériaux/architecturales. Avant de converger,
méthode First Principles : déconstruis le concept de « pneu » jusqu'aux
fonctions physiques irréductibles (transmission de force, dissipation,
compliance, étanchéité, etc.).

Ensuite Cross-Pollination : pour chaque fonction, quels champs scientifiques
ou industriels ont résolu un problème analogue ?
```

> **Attendu** : décomposition fonctionnelle nette + analogies vers aérospatial (composites auto-réparants NASA), biomédical (hydrogels), bâtiment (béton auto-cicatrisant à bactéries), électronique (polymères Diels-Alder réversibles)…

### Étape 4 — Clôture par Victor (Innovation Ambition Matrix)

```
/bmad-cis-agent-innovation-strategist

Sur la base des 4-5 pistes matériaux/architecturales qu'on vient de générer
(TRIZ + biomimétisme + first principles + cross-pollination), applique
l'Innovation Ambition Matrix : pour chaque piste, classe-la en
core / adjacent / transformational, en argumentant sur les axes
(marché cible, technologie nouvelle, modèle d'affaires).

Termine par une recommandation de portefeuille : quel mix entre les 3
catégories serait raisonnable pour les 24 prochains mois ?
```

> **Attendu** : matrice 2D claire (où chaque piste est placée), avec justification courte. Les pistes "remplir un additif réactif" partent en core/adjacent, les pistes "compound vivant à culture bactérienne" en transformational. Le mix de clôture donne un artefact concret que l'équipe pourra réutiliser.

### Étape 5 — Pause et débat avec le public

Couper la démo et demander :
> « Sur la matrice, où mettriez-vous vos priorités ? Et quelle piste vous tenteriez en labo la semaine prochaine ? »

C'est **le moment clé** : ils voient que CIS structure la discussion sans la remplacer — du divergent (Carson, Dr. Quinn) au convergent stratégique (Victor).

---

## 4. Reveal du kit complet (5 min)

| Agent CIS | Quand l'utiliser en R&D Michelin |
|---|---|
| **Dr. Quinn** *(problem-solver)* | TRIZ, biomimétisme, root cause, Theory of Constraints — **cœur de l'usage scientifique** |
| **Carson** *(brainstorming-coach)* | First principles, morphological analysis, provocation, cross-pollination |
| **Victor** *(innovation-strategist)* | **Innovation Ambition Matrix**, Three Horizons, Scenario Planning, Disruption Theory (Christensen) |
| **Maya** *(design-thinking-coach)* | Quand un produit doit rencontrer un utilisateur (cas wheelchair gloves) |
| **Sophia** *(storyteller)* | Pitcher une innovation à un comité de direction |
| **Caravaggio** *(presentation-master)* | Préparer une présentation scientifique percutante |

Workflows complémentaires : `bmad-cis-design-thinking`, `bmad-cis-innovation-strategy`, `bmad-cis-problem-solving`, `bmad-cis-storytelling`.

---

## 5. Closing (2 min)

> « Demain matin, vous avez le choix : continuer à brainstormer en post-its sur un mur, ou avoir un coach TRIZ + biomimétisme disponible 24/7 dans votre IDE. **Quelle contradiction R&D vous bloque en ce moment ?** »

---

## Filets de sécurité

- **Si une commande slash ne répond pas** : vérifier que Claude Code a bien été relancé après l'install (les skills sont en `.claude/skills/`).
- **Si la réponse de l'agent dérape** : couper, dire « OK, recadrons », et utiliser une variante : `Reprends avec uniquement les principes TRIZ 1, 15, 35.`
- **Si le réseau lâche** : ce fichier DEMO.md contient l'arc narratif — tu peux dérouler à l'oral en montrant juste les prompts.

## Ressources

- BMAD-METHOD : https://github.com/bmad-code-org/BMAD-METHOD
- Module CIS : https://github.com/bmad-code-org/bmad-module-creative-intelligence-suite
- Docs : https://docs.bmad-method.org
