# Systeme de Magie

> Document de regles en cours de conception. Base sur le Year Zero Engine.

---

## Principes de design

- **Coherence YZE** : La magie utilise le meme systeme de base que toute autre action (pool de d6, 1 succes = reussite, extras = effets bonus).
- **Equilibre martial/mage** : La magie est puissante mais couteuse. Le guerrier est fiable et endurant. Les deux sont utiles et amusants a jouer.
- **Risque/recompense** : Plus un sort est puissant, plus il est risque. Le mage choisit son niveau d'engagement.
- **Rarete** : Dans le monde, la plupart des gens n'ont pas acces a la magie (consequence historique). Les PJ et certains PNJ, venus d'un autre monde ou descendants de gens d'autres mondes, font exception.

---

## Acces a la magie

### A la creation du personnage

- Les **archetypes magiques** (mage, druide, pretre, etc.) commencent avec :
  - La competence **Arcanes** (liee a Esprit) a un niveau de depart (1-3)
  - 1 a 3 sorts de cercle 1
  - Acces aux talents magiques

- Les **autres archetypes** ne possedent pas la competence Arcanes et n'ont pas de sorts.

### En cours de jeu (via XP)

- N'importe quel personnage peut acheter la competence Arcanes (niveau 1) et apprendre des sorts, mais le **cout en XP est majore** pour les non-specialistes (ex : x2).
- Les non-specialistes ne peuvent pas depasser un certain niveau d'Arcanes (ex : niveau 2) ni acceder aux sorts de cercle 3.
- Les **talents magiques avances** sont reserves aux archetypes magiques.

---

## Competence : Arcanes (Esprit)

La competence Arcanes est liee a l'attribut **Esprit**. Elle couvre :
- Le lancer de sorts
- L'identification de phenomenes magiques
- La connaissance des traditions et des rituels

---

## Cantrips

Les cantrips sont des sorts mineurs que tout mage maitrise instinctivement. Ils representent la magie de base — l'equivalent de l'epee du guerrier.

### Principe

- **Pas de cout en Resolution** : les cantrips ne consomment pas de des de Magie.
- **Pool** : `Esprit + Arcanes` uniquement (des de Base + des de Competence).
- **Push** : le push fonctionne normalement (risque sur les des de Base = degat a Esprit), mais il n'y a pas de des de Magie a relancer, donc **pas de risque de blessure magique**.
- **Prouesses** : les succes excedentaires sur un cantrip generent des prouesses normalement (portee, duree, precision, etc.).

### Acces

- Chaque ecole de magie propose **2-3 cantrips** specifiques.
- Des **cantrips communs** sont accessibles a toutes les ecoles.
- Un personnage connait les cantrips de son ecole + les cantrips communs des la creation.

### Limites

Les cantrips sont des outils de base, pas des armes de guerre :
- Leurs effets restent **mineurs et utilitaires** (en dessous du cercle 1 en puissance).
- Ils ne remplacent pas les sorts payants — ils les completent.

> **Design** : le mage sans Resolution a toujours quelque chose a faire. Il n'est pas un guerrier sans epee.

---

## Lancer un sort

### Constitution du pool de des

```
Pool = Esprit + Arcanes + des de Resolution depenses
```

Les **des de Resolution depenses** fonctionnent comme les des d'Equipement du guerrier : ils augmentent le pool mais comportent un risque specifique en cas de push.

| Composante        | Couleur des des | Role                                |
|-------------------|-----------------|-------------------------------------|
| Esprit            | Des de Base     | Attribut du lanceur                 |
| Arcanes           | Des de Competence | Entrainement magique              |
| Resolution depensee | Des de Magie (couleur dediee) | Puissance injectee dans le sort |

### Resolution du sort

1. Le mage depense entre 1 et X points de Resolution (selon le cercle du sort et son choix).
2. Il constitue son pool : Esprit + Arcanes + des de Resolution depenses.
3. Il lance tous les des.
4. **1 succes (6) = le sort fonctionne.**
5. Chaque succes supplementaire ameliore l'effet (portee, duree, degats, nombre de cibles — selon le sort).

### Pousser un jet de sort (Push)

Comme tout jet YZE, le mage peut pousser son jet s'il n'a pas obtenu assez de succes. Les regles de push s'appliquent normalement, avec une consequence specifique pour les des de Magie :

| Type de de   | Effet d'un 1 au push                              |
|--------------|----------------------------------------------------|
| De de Base (Esprit) | -1 point a l'attribut Esprit (comme d'habitude) |
| De de Competence (Arcanes) | Aucun effet negatif (comme d'habitude) |
| De de Magie (Resolution) | **Blessure magique** : -1 en Resolution permanente (jusqu'a soin) |

---

## Blessure magique

### Declenchement

Un **1 sur un de de Magie** lors d'un push provoque une blessure magique. Chaque 1 sur un de de Magie lors du push inflige une blessure magique separee.

### Effet

Chaque blessure magique **reduit la Resolution maximale de 1** jusqu'a ce qu'elle soit soignee.

Consequences en cascade :
- Le mage a moins de Resolution disponible pour ses prochains sorts.
- Il est plus vulnerable au stress, a la peur et a l'horreur (meme jauge).
- Sa capacite a encaisser la pression mentale diminue.

C'est **auto-equilibrant** : plus le mage force, moins il peut forcer ensuite.

### Soin des blessures magiques

Les blessures magiques ne guerissent pas comme les blessures physiques :
- **Repos prolonge** (plusieurs jours de repos complet) : recupere 1 point de Resolution maximale par periode de repos.
- **Soin magique** : un autre pratiquant peut tenter un jet d'Arcanes pour soigner une blessure magique (un succes = 1 point restaure).
- **Lieux de pouvoir** : certains endroits permettent une guerison acceleree (a definir selon le setting).

### Resolution a 0 : Trauma magique

Si la Resolution maximale d'un mage tombe a **0** suite a des blessures magiques, il subit un **trauma magique**. Jet sur la table de sequelles magiques :

| d6 | Sequelle |
|----|----------|
| 1 | **Coupure temporaire** : impossible de lancer tout sort pendant 1d6 jours |
| 2 | **Stigmate magique** : marque physique visible (yeux changeants, veines lumineuses, etc.) -- permanent, consequence sociale |
| 3 | **Instabilite** : la magie du mage devient erratique. -1 de permanent a tous les jets d'Arcanes tant que non soigne par un rituel |
| 4 | **Resonance douloureuse** : le mage subit 1 point de stress a chaque fois qu'il est en presence de magie |
| 5 | **Perte de sort** : le mage oublie un sort aleatoire. Il peut le reapprendre normalement. |
| 6 | **Eveil incontrolable** : un effet magique aleatoire se declenche (au choix du MJ). Le mage perd connaissance. |

> Cette table est volontairement moderee : le trauma magique est un handicap serieux mais pas une mort de personnage. Le but est la tension, pas la punition.

---

## Les cercles de sorts

Les sorts sont organises en trois cercles. Le cercle determine le **cout minimum en Resolution** et les **conditions d'acces**, mais pas le nombre de succes requis (toujours 1 pour reussir).

### Cercle 1 : Sorts mineurs

- **Cout minimum** : 1 point de Resolution
- **Acces** : Tout personnage avec Arcanes 1+
- **Puissance** : Effets modestes et locaux
- **Exemples** : Allumer un feu, detecter la magie a proximite, soigner une blessure legere, renforcer un objet temporairement, message telepathique court

### Cercle 2 : Sorts standards

- **Cout minimum** : 2 points de Resolution
- **Acces** : Arcanes 2+ (non-specialistes peuvent y acceder avec effort)
- **Puissance** : Effets significatifs
- **Exemples** : Projectile magique, bouclier de force, guerison d'une blessure critique, vision a distance, alteration d'un element

### Cercle 3 : Sorts majeurs

- **Cout minimum** : 3 points de Resolution
- **Acces** : Arcanes 3+ et **talent magique avance** (archetypes magiques uniquement)
- **Puissance** : Effets spectaculaires et transformateurs
- **Exemples** : Tempete d'eclairs localisee, teleportation courte distance, animation d'un objet/creature, guerison de masse, controle mental

### Amplification

Le mage peut toujours depenser **plus de Resolution que le cout minimum** pour augmenter son pool de des. Cela augmente ses chances de succes et d'effets supplementaires, mais augmente aussi le nombre de des de Magie (et donc le risque de blessure magique au push).

---

## Comparaison guerrier / mage

| Aspect | Guerrier | Mage |
|--------|----------|------|
| **Pool typique** | Force + Melee + des d'Equipement (arme) | Esprit + Arcanes + des de Magie (Resolution) |
| **Risque au push** | Degat a Force + deterioration de l'arme | Degat a Esprit + blessure magique (Resolution) |
| **Ressource consommee** | Arme (reparable par Artisanat) | Resolution (guerissable par repos/soin) |
| **Fiabilite** | Haute -- peut attaquer chaque round sans cout | Variable -- chaque sort coute de la Resolution |
| **Puissance de pointe** | Reguliere et stable | Haute mais episodique |
| **Vulnerabilite** | Degats physiques | Stress, peur, horreur (Resolution entamee) |
| **Avantage en longue duree** | Le guerrier tient la distance | Le mage s'epuise et doit gerer ses ressources |

---

## Interaction avec le stress de combat

Le systeme actuel (voir resume.md) ajoute le stress au pool de des en combat, avec un risque sur les 1 des des de stress.

Pour un mage en combat :
- Le stress s'ajoute normalement a ses jets de sort (comme a tout jet).
- Un mage stresse lance plus de des (bien) mais risque des effets de stress ET des blessures magiques (mal).
- La Resolution etant partagee entre magie et resistance au stress, un mage qui a beaucoup lance de sorts est aussi plus vulnerable a la panique.

---

## Questions ouvertes

- [ ] **Liste des sorts** : a concevoir pour chaque cercle
- [ ] **Traditions/ecoles de magie** : faut-il des sous-specialisations (feu, guerison, illusion...) ou un systeme unifie ?
- [ ] **Rituels** : sorts longs, cooperatifs, potentiellement freeform ? Regles dediees ?
- [ ] **Magie divine vs arcane** : un seul systeme ou des variantes mecaniques selon la source du pouvoir ?
- [ ] **Table de sequelles magiques** : a etoffer (passer au d66 pour plus de variete ?)
- [x] **Cantrips** : **adoptes** — categorie dediee, sans cout en Resolution, pool = Esprit + Arcanes, 2-3 par ecole + communs (voir `sorts-draft.md`)
- [ ] **Le setting** : d'ou vient la magie ? Pourquoi les locaux l'ont perdue ? Comment est-elle percue ?
