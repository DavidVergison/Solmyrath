# Guide d'equilibrage des talents — Reference de conception

> Synthese des patrons de design observes dans **Forbidden Lands** (FL) et **Symbaroum** (SYM).
> Sert de grille de lecture pour creer, adapter ou equilibrer les talents du systeme Isekai YZE.

---

## 1. Architecture des talents dans les sources

### Forbidden Lands

- **3 categories** : Peuple (inne, 1 rang), Profession (role, 3 rangs, cout en VOL), General (acquis, 3 rangs, generalement passif)
- **3 rangs** par talent (sauf peuple) — cumulatifs (on conserve les effets des rangs inferieurs)
- **Economie** : les talents de peuple et profession coutent des points de Volonte (VOL) ; les talents generaux sont majoritairement passifs (pas de cout)
- **Acquisition** : talents de profession = acces exclusif a la profession ; talents generaux = 3 XP pour debloquer

### Symbaroum

- **Traits** (innes, raciaux) vs **Talents** (acquis, entrainement)
- **3 niveaux** : Novice → Adepte → Maitre — cumulatifs
- **5 types d'actions** : Active (cout d'action), Gratuite (pas de cout), Passive (permanente), Reactive (declenchee), Speciale (conditions propres)
- **Restrictions** : certains talents lies a un archetype (Guerrier/Mystique/Roublard) ou a une carriere specifique
- **Corruption** comme cout alternatif pour les talents mystiques

### Convergences

Les deux systemes partagent :
- Une structure en **3 rangs progressifs**
- Une distinction entre **capacites innees** (peuple/trait) et **acquises** (profession/talent)
- Un schema de puissance croissante : bonus modeste → option tactique → capacite culminante
- Des talents generiques accessibles a tous vs des talents reserves a un role

---

## 2. Echelle de puissance — Les 3 paliers

### Rang 1 (Novice / mineur) — "J'ai acces"

**Philosophie** : un avantage modeste, une porte ouverte, un bonus lineaire.

| Type d'effet | Exemples |
|---|---|
| **Bonus numerique fixe** | +1 de a un jet precis (FL: Maitre des couteaux, Tireur d'elite) |
| **Substitution d'attribut** | Utiliser Force au lieu de Precision (SYM: Poigne de fer), Discretion au lieu de Precision (SYM: Feinte) |
| **Capacite conditionnelle simple** | 1 parade gratuite/round (FL: Defenseur R1), esquive d'une attaque libre (SYM: Acrobatie) |
| **Acces de base** | Fabriquer des objets ordinaires (FL: Forgeron R1), preparer des elixirs simples (SYM: Alchimie) |
| **Bonus de degats modeste** | +1d4 ou +1d6 sous condition (SYM: Berserker, Coup en traitre) |
| **Reussite automatique simple** | Trouver des provisions sans jet (FL: Voie de la Foret R1, 1 VOL) |

**Repere de calibrage** : un talent de rang 1 ne devrait jamais etre meilleur qu'un bon jet de des. C'est un bonus, pas un game-changer.

---

### Rang 2 (Adepte / standard) — "J'ai une option tactique"

**Philosophie** : une nouvelle dimension, un effet secondaire, une restriction levee.

| Type d'effet | Exemples |
|---|---|
| **Bonus augmente** | +1 supplementaire, ou extension du champ d'application |
| **Capacite supplementaire** | Attaque de riposte gratuite (SYM: Epeiste virtuose), parer pour un allie (FL: Voie du Bouclier R2) |
| **Reussite automatique elargie** | Resistance au froid sans jet (FL: Voie de la Foret R2), manipulation reussie auto (FL: Voie du Mensonge R2) |
| **Effet secondaire** | Hemorragie (SYM: Coup en traitre Adepte), aveuglement, mise a terre |
| **Crafting ameliore** | Objets de qualite +1, mais temps et difficulte accrus (FL: Forgeron R2) |
| **Reduction de contrainte** | Le berserker ignore 1d4 degats (SYM), le combattant peut fractionner son mouvement |

**Repere de calibrage** : un talent de rang 2 devrait creer des choix tactiques interessants. Il elargit le repertoire sans briser l'equilibre.

---

### Rang 3 (Maitre / majeur) — "Je redefinisles regles"

**Philosophie** : une capacite culminante qui altere fondamentalement le fonctionnement du personnage.

| Type d'effet | Exemples |
|---|---|
| **De d'artefact (d8)** | +1d8 au jet (FL: Maitre epeiste R3, Tireur d'elite R3) |
| **Immunite totale** | Immunite a la Manipulation (FL: Impassible R3), a la peur (FL: Vaillance R3) |
| **Suppression de limitation** | Parades illimitees (FL: Defenseur R3), esquives illimitees (FL: Preste R3) |
| **Degats scalables** | +1 degat par VOL depense (FL: Voie de l'Epee R3) |
| **Ignorer l'armure** | SYM: Tireur d'elite Maitre, Puissance a deux mains Maitre |
| **Capacite de controle** | Hypnose/soumission (FL: Voie de l'Assassin R3 ; SYM: Domination Maitre) |
| **Actions multiples** | Frapper tous les ennemis a portee (SYM: Armes articulees Maitre), tirer 2-3 fois (FL: Tir rapide R3, SYM: Tir en rafale) |
| **Riposte illimitee** | Contre-attaque a chaque defense reussie (SYM: Epeiste virtuose Maitre) |
| **Suppression de cout** | Zero Corruption temporaire (SYM: Baton mystique Maitre) |

**Repere de calibrage** : un talent de rang 3 est une recompense d'investissement long. Il doit etre puissant sans rendre les autres talents obsoletes. Verifier qu'il ne cree pas de boucle infinie (riposte illimitee + actions gratuites = abus potentiel).

---

## 3. Patrons de design recurrents

### A. Bonus numerique progressif (+1 / +2 / d8)

Le patron le plus simple et le plus courant dans FL.

```
R1 : +1 de ou +1 degat dans une situation precise
R2 : +2 ou extension du declencheur
R3 : +1d8 (de d'artefact) ou bonus scalable
```

**Risque** : ennuyeux si c'est tout ce que fait le talent. A combiner avec un effet qualitatif.

### B. Capacite conditionnelle debloquee puis etendue

```
R1 : peut faire X une fois par round (ex : parer, esquiver, riposte)
R2 : peut faire X dans des conditions elargies (pour un allie, en reaction)
R3 : peut faire X sans limite (illimite par round)
```

**Risque au R3** : la suppression totale de limitation est tres puissante. S'assurer qu'il existe un contre (cout en action, condition de declenchement).

### C. Substitution d'attribut (patron Symbaroum)

```
Novice : utiliser Attribut-A au lieu d'Attribut-B pour une action
```

Tres elegant. Permet a un personnage de jouer un archetype different sans sous-systeme. Exemple : un guerrier brutal (Force au lieu de Precision pour frapper) vs un duelliste agile.

**Application Isekai YZE** : parfaitement compatible. Permet de differencier des professions sans creer de regles supplementaires.

### D. Reussite automatique (patron FL)

```
R1 : reussite automatique a une tache de survie/social (cout : 1 VOL)
R2 : reussite automatique a une tache plus large
```

**Attention** : ne jamais rendre automatique quelque chose qui est au coeur du gameplay (combat, magie). Reserver aux taches de support (provisions, campement, navigation).

### E. Talent d'acces (cle magique)

```
R1 : debloquer les sorts de cercle 1
R2 : debloquer les sorts de cercle 2
R3 : debloquer les sorts de cercle 3
```

C'est le modele FL pour Druide/Sorcier. Le talent ne fait rien en soi — il ouvre l'acces. La puissance vient de la liste de sorts.

**Application Isekai YZE** : deja prevu via la competence Arcanes + cercles de sorts. Verifier si on veut un talent supplementaire en plus de la competence, ou si les cercles sont debloques autrement (XP, prerequis de rang Arcanes).

### F. Contrepartie integree

```
Effet puissant mais penalty associe (SYM: Berserker = +1d6 degats mais Defense reduite)
```

Le rang Maitre peut supprimer la contrepartie — c'est la recompense ultime.

**Attention** : bien calibrer la contrepartie. Si elle est trop faible, le talent est sous-cout. Si elle est trop forte, personne ne le prend.

### G. Talent de carriere exclusif

Un talent accessible uniquement a une profession ou a un archetype. Plus puissant qu'un talent general car il definit l'identite du role.

**Application Isekai YZE** : chaque Profession devrait avoir 2-3 talents exclusifs qui la definissent. Les talents generaux completeraient le build.

---

## 4. Pieges d'equilibrage observes

### Ecart combat vs utilitaire

FL presente un desequilibre net : les talents de combat (Defenseur, Preste, Tir rapide) sont spectaculaires, tandis que les talents utilitaires (Pecheur, Methodique, Tailleur) sont negligeables en jeu.

**Lecon** : les talents non-combat doivent avoir un **impact tangible en session** — pas juste un bonus logistique. Soit ils influencent le rythme (repos, provisions = survie), soit ils ouvrent des **options de jeu** (acces a des lieux, contacts, fabrication d'objets speciaux).

### Talents raciaux desequilibres

FL : Paix interieure (Elfe = guerison totale), Dur a cuire (Nain = push multiple), Energie psychique (Demi-elfe = reduction de cout) sont tres au-dessus d'Adaptation (Humain) ou Nocturne (Gobelin).

**Lecon** : les talents de Kin doivent etre calibres au meme niveau d'impact. Si un talent de Kin est transformatif, **tous** doivent l'etre. Si l'un est un bonus mineur, tous doivent etre mineurs.

### Accumulation de passifs

Les talents Passifs (SYM) et les talents generaux gratuits (FL) s'empilent sans cout. Un personnage avec 5+ talents passifs obtient un avantage structurel massif.

**Lecon** : limiter le nombre de talents simultanes, ou s'assurer que les talents passifs restent modestes (bonus +1, pas de transformation qualitative).

### Boucles de riposte

SYM : Epeiste virtuose Maitre (riposte illimitee) + haute Defense = un personnage qui inflige plus de degats en se defendant qu'en attaquant. Combine avec Coup bas Maitre (1d6 auto sans jet a chaque attaque recue), ca devient absurde.

**Lecon** : toujours verifier les **combinaisons** de talents au rang 3. Un talent puissant seul est acceptable ; deux talents qui se nourrissent mutuellement peuvent briser le jeu.

---

## 5. Grille de calibrage pour Isekai YZE

### Structure proposee

| Element | Decision |
|---|---|
| **Nombre de rangs** | 3 (coherent avec les cercles de sorts et les deux sources) |
| **Categories** | Kin (1 talent inne, 1 rang) / Profession (2-3 exclusifs, 3 rangs) / General (acces libre, 3 rangs) |
| **Economie** | Talents actifs = cout en Points de Volonte (PV) ; Talents passifs = pas de cout |
| **Nombre total vise** | 8-10 talents generaux, 2-3 par profession, 1 par Kin |

### Economie des Points de Volonte (PV)

Les talents actifs coutent des **Points de Volonte (PV)** pour etre actives. Les PV sont generes par le push (1 PV par push, que le push reussisse ou echoue). La reserve max de PV = ⌈(Esprit + Empathie) / 2⌉ + 1 (echelle typique : 3-6 PV).

**Couts typiques par rang :**

| Rang | Cout PV | Justification |
|------|---------|---------------|
| R1 | 1 PV | Effet modeste, usage frequent |
| R2 | 1-2 PV | Option tactique, usage reflechi |
| R3 | 1-3 PV | Capacite culminante, usage decisif |

**Talents passifs vs actifs :**

- **Passif** : toujours actif, pas de cout PV. Doit rester modeste (bonus +1, acces conditionnel). Exemples : bonus de degats fixe, substitution d'attribut.
- **Actif** : cout PV a chaque utilisation. Peut etre plus puissant car le cout agit comme limiteur naturel. Exemples : reussite automatique, capacite speciale declenchee.

> **Note** : la Resolution reste exclusivement reservee a la magie. Les PV couvrent tous les talents, physiques comme mentaux.

### Checklist par talent

Avant de valider un talent, verifier :

- [ ] **Rang 1 est-il utile sans etre indispensable ?** Il doit donner envie sans etre un prerequis automatique.
- [ ] **Rang 2 ajoute-t-il une dimension tactique ?** Pas juste "+1 de plus".
- [ ] **Rang 3 est-il puissant sans etre auto-win ?** Verifier les combos avec d'autres talents R3.
- [ ] **Le cout en PV est-il proportionnel ?** Un talent passif (gratuit) doit etre plus modeste qu'un talent actif (couteux en PV).
- [ ] **Est-il utile en session ?** Un talent qu'on n'active jamais est un piege-a-XP.
- [ ] **A-t-il un contre ?** Tout talent devrait avoir une situation ou il ne sert a rien.
- [ ] **Se combine-t-il raisonnablement ?** Verifier les 2-3 combinaisons les plus probables.

### Echelle de reference rapide

| Rang | Equivalent narratif | Effet typique | Exemples de benchmark |
|------|---------------------|---------------|----------------------|
| 1 | "J'ai un truc en plus" | +1 de, acces simple, bonus conditionnel | FL: Chasseur R1, SYM: Alchimie Novice |
| 2 | "J'ai un avantage tactique" | Capacite supplementaire, effet secondaire, restriction levee | FL: Voie du Bouclier R2, SYM: Epeiste virtuose Adepte |
| 3 | "Je suis un specialiste reconnu" | De d'artefact, immunite, actions multiples, capacite culminante | FL: Defenseur R3, SYM: Tireur d'elite Maitre |

---

## 6. Types d'actions (vocabulaire de design)

Adopter le vocabulaire de Symbaroum, adapte au YZE :

| Type | Definition | Impact equilibrage |
|------|------------|-------------------|
| **Active** | Coute une action (lente ou rapide) | Cout reel en tempo — peut etre plus puissant |
| **Passive** | Toujours active, pas de cout | Doit rester modeste (bonus +1, acces conditionnel) |
| **Reactive** | Se declenche en reaction a un evenement | Conditionnel = peut etre assez puissant |
| **Gratuite** | Pas de cout d'action, utilisable en plus | A surveiller — gratuit + puissant = abus |
| **Speciale** | Conditions propres (1x/scene, 1x/session, hors combat) | Le limiteur est la frequence |

---

## 7. Recapitulatif — Talents des sources par categorie

> Reference rapide pour s'inspirer ou adapter.

### Combat melee
- FL : Voie de l'Epee, Voie du Bouclier, Ambidextre, Berserker, Defenseur, Charge percutante, maitrise d'arme (x5)
- SYM : Berserker, Double Attaque, Poigne de fer, Epeiste virtuose, Lutte, Coup bas, Feinte, maitrise d'arme (hache, marteau, armes d'hast, armes articulees)

### Combat a distance
- FL : Voie de la Fleche, Tireur d'elite, Tir rapide, Frondeur
- SYM : Tireur d'elite, Bout portant, Tir cible, Tir en rafale, Sixieme sens

### Defense / Protection
- FL : Defenseur, Preste, Resistance a la douleur, Poigne ferme, Stabilite
- SYM : Homme d'armes, Garde du corps, Inebranlable, Acrobatie, Recuperation

### Leadership / Social
- FL : Voie du Cri de guerre, Intimidation, Langue de vipere, Vaillance
- SYM : Meneur ne, Domination

### Survie / Exploration
- FL : Voie de la Foret, Chasseur, Chef de camp, Explorateur, Herboriste, Pisteur, Sixieme sens
- SYM : Connaissance des betes, Instinct du chasseur

### Crafting / Artisanat
- FL : Forgeron, Facteur d'arc, Tailleur, Tanneur, Cuisinier, Batisseur, Empoisonneur
- SYM : Art de la forge, Alchimie, Creation d'artefacts, Expertise des pieges

### Magie (acces/tradition)
- FL : Voies (Clairvoyance, Guerison, Metamorphose, Mort, Pierre, Sang, Signes)
- SYM : Magie, Sorcellerie, Theurgie, Conjuration, Symbolisme, Baton mystique, Chant des trolls

### Capacites raciales / Traits
- FL : Adaptation, Paix interieure, Energie psychique, Dur a cuire, Insaisissable, Instinct du predateur, Nocturne, Inebranlable
- SYM : Vigoureux, Paria, Privilegie, Changeforme
