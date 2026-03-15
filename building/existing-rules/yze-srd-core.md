# Year Zero Engine (YZE) -- Document de Reference Systeme (SRD)

> **Source** : Year Zero Engine SRD par Free League Publishing. Systeme ouvert et libre (OGL).
> **Note** : Ce document est une synthese de reference basee sur le SRD officiel du Year Zero Engine. Pour le texte original en anglais, consulter le SRD sur le site de Free League Publishing (freeleaguepublishing.com).

---

## Table des matieres

1. [Presentation generale](#1-presentation-generale)
2. [Mecaniques de base](#2-mecaniques-de-base)
3. [Attributs](#3-attributs)
4. [Competences](#4-competences)
5. [Pousser un jet (Pushing)](#5-pousser-un-jet-pushing)
6. [Talents](#6-talents)
7. [Combat](#7-combat)
8. [Degats, armure et blessures critiques](#8-degats-armure-et-blessures-critiques)
9. [Conditions et etats](#9-conditions-et-etats)
10. [Stress et panique (variante Alien RPG)](#10-stress-et-panique-variante-alien-rpg)
11. [Equipement et encombrement](#11-equipement-et-encombrement)
12. [Experience et progression](#12-experience-et-progression)
13. [Autres mecaniques fondamentales](#13-autres-mecaniques-fondamentales)

---

## 1. Presentation generale

Le **Year Zero Engine** (YZE) est un systeme de jeu de role generique cree par **Free League Publishing** (Fria Ligan). Il a ete utilise comme base pour de nombreux jeux :

- **Mutant: Year Zero** (le jeu originel du systeme)
- **Coriolis -- Le Troisieme Horizon**
- **Tales from the Loop / Things from the Flood**
- **Forbidden Lands**
- **ALIEN -- Le Jeu de Role**
- **Vaesen**
- **The One Ring** (2e edition, variante)
- **Blade Runner -- Le Jeu de Role**
- **Twilight: 2000** (4e edition)

Le SRD (System Reference Document) est mis a disposition gratuitement par Free League sous une licence ouverte (Year Zero Engine License), permettant aux createurs tiers de concevoir leurs propres jeux bases sur ce moteur.

### Philosophie du systeme

- **Simplicite et rapidite** : resolution en un seul jet de des.
- **Narration avant tout** : les mecaniques soutiennent le recit, pas l'inverse.
- **Danger et consequences** : pousser un jet a un cout ; les combats sont dangereux.
- **Modularite** : le SRD fournit un noyau que chaque jeu adapte selon son theme.

---

## 2. Mecaniques de base

### 2.1 Pools de des (Dice Pools)

Le YZE utilise des **pools de d6** (des a six faces). Le principe fondamental :

1. Le joueur constitue un pool de des egal a **Attribut + Competence** (+ eventuels modificateurs).
2. Il lance tous les des simultanement.
3. Chaque de affichant un **6** compte comme un **succes**.
4. **Un seul succes suffit** pour reussir l'action.
5. Des succes supplementaires (au-dela du premier) sont des **succes excedentaires** qui peuvent etre depenses pour des effets additionnels (appeles **stunts** ou **prouesses** dans certains jeux).

### 2.2 Difficulte

Par defaut, il n'y a **pas de seuil de difficulte variable**. Une action est soit :
- **Contestee** : l'adversaire lance aussi un pool de des ; celui qui obtient le plus de succes l'emporte.
- **Non contestee** : un seul succes suffit.

Certaines variantes du YZE introduisent des **modificateurs** qui ajoutent ou retirent des des du pool (bonus/malus de +1 a +3 ou -1 a -3 des).

### 2.3 Types de des (variante selon les jeux)

Dans la version "classique" (Mutant: Year Zero, Forbidden Lands), il y a **trois types de des d6**, differencies par la couleur :

| Type de de | Couleur typique | Role |
|---|---|---|
| **Des de Base** (Attribut) | Jaune/Vert | Representent l'attribut physique ou mental |
| **Des de Competence** (Skill) | Bleu | Representent l'entrainement et l'expertise |
| **Des d'Equipement** (Gear) | Noir/Gris | Representent la qualite de l'equipement utilise |

- Sur **tous les des** : un resultat de **6 = succes**.
- Sur les **des de Base** : un resultat de **1 = degat a l'attribut** (uniquement en cas de **push**).
- Sur les **des d'Equipement** : un resultat de **1 = deterioration de l'equipement** (uniquement en cas de **push**).
- Les **des de Competence** n'ont **jamais** de consequence negative sur un 1.

> **Variante simplifiee** (Tales from the Loop, Vaesen, ALIEN) : tous les des sont identiques (pas de distinction Base/Competence/Equipement). Le push a d'autres consequences (stress, conditions, etc.).

---

## 3. Attributs

Le YZE definit generalement **quatre attributs** principaux, notes de **1 a 5** :

| Attribut | Description |
|---|---|
| **Force** (Strength) | Puissance physique brute, endurance, resistance |
| **Agilite** (Agility) | Rapidite, reflexes, coordination, discretion |
| **Intelligence** (Wits) | Perception, raisonnement, connaissances |
| **Empathie** (Empathy) | Charisme, intuition sociale, manipulation |

### Points d'attribut et degats

Chaque attribut a un score courant qui peut **diminuer** suite a des degats, de la fatigue, du stress ou des conditions. Quand un attribut tombe a **0**, le personnage subit un etat critique lie a cet attribut :

| Attribut a 0 | Consequence |
|---|---|
| Force = 0 | **Brise** : le personnage s'effondre physiquement, risque de blessure critique |
| Agilite = 0 | **Epuise** : le personnage ne peut plus bouger efficacement |
| Intelligence = 0 | **Hébete** : le personnage est confus, desoriente |
| Empathie = 0 | **Desespere** : le personnage craque psychologiquement |

> Les noms et consequences exactes varient selon le jeu. Le mecanisme de base reste : attribut a 0 = etat critique + jet sur une table de blessures/trauma critiques.

---

## 4. Competences

### 4.1 Liste typique

Chaque competence est liee a un attribut et notee de **0 a 5**. La liste standard du SRD comporte generalement **12 competences** :

**Competences de Force :**
- **Puissance** (Might) -- soulever, forcer, pousser
- **Endurance** (Endurance) -- resister a la fatigue, marche forcee

**Competences d'Agilite :**
- **Mêlee** (Melee) -- combat rapproche
- **Discretion** (Stealth) -- se cacher, se deplacer silencieusement
- **Deplacement** (Move) -- courir, sauter, escalader, nager
- **Tir** (Marksmanship) -- armes a distance

**Competences d'Intelligence :**
- **Fouille** (Scout) -- observer, detecter, pistage
- **Comprehension** (Comprehend) -- analyser, dechiffrer
- **Survie** (Survival) -- orientation, chasse, premiers soins en milieu sauvage
- **Artisanat** (Craft) -- fabriquer, reparer

**Competences d'Empathie :**
- **Manipulation** (Manipulate) -- persuader, mentir, negocier
- **Prestance** (Performance) -- inspirer, diriger, divertir
- **Soins** (Heal) -- premiers soins, medecine

> **Note** : La liste exacte varie selon le jeu. Forbidden Lands, Coriolis et Mutant: Year Zero ont chacun leur propre selection. Le SRD fournit un cadre adaptable.

### 4.2 Resolution : Attribut + Competence

Pour toute action non triviale :

```
Pool de des = Attribut lie + Niveau de Competence (+ bonus d'equipement eventuel)
```

**Exemple** : Un personnage avec Agilite 3 et Tir 2 utilisant un bon fusil (+2 des d'equipement) lance **3 + 2 + 2 = 7 des**.

### 4.3 Competences a 0

Un personnage peut tenter une action correspondant a une competence qu'il ne possede pas (niveau 0). Il lance alors uniquement les **des de l'attribut** associe, sans des de competence.

---

## 5. Pousser un jet (Pushing)

Le **push** (pousser un jet) est une mecanique centrale et distinctive du YZE.

### 5.1 Principe

Apres un jet rate (ou insuffisamment reussi), le joueur peut choisir de **pousser le jet** :

1. Il **relance tous les des qui n'affichent pas un 6** (les succes deja obtenus sont conserves).
2. Les des affichant deja un **1** ne sont **pas relances** (dans la version classique).
3. On ne peut pousser qu'**une seule fois** par jet.

### 5.2 Consequences du push (version classique)

Apres le push, on compte tous les resultats :

- Chaque nouveau **6** est un succes supplementaire.
- Chaque **1 sur un de de Base** (attribut) inflige **1 point de degat a l'attribut** correspondant.
- Chaque **1 sur un de d'Equipement** reduit le **bonus d'equipement de 1** (usure).
- Les **1 sur les des de Competence** n'ont **aucune consequence**.

> **C'est le dilemme central du YZE** : pousser donne plus de chances de succes, mais au prix potentiel de degats a soi-meme et a son equipement. Cela cree une tension narrative forte.

### 5.3 Consequences du push (version simplifiee)

Dans les jeux sans des distincts (ALIEN, Vaesen, Tales from the Loop) :

- **ALIEN** : chaque 1 sur un **de de Stress** declenche potentiellement une **reaction de panique**. Le push ajoute un de de Stress au pool.
- **Tales from the Loop** : le push inflige une **Condition** au personnage (Epuise, Effraye, Blesse, etc.).
- **Vaesen** : le push inflige des Conditions similaires.
- **Forbidden Lands** : version classique avec des colores.

### 5.4 Points de Volonte (Willpower Points)

Dans plusieurs variantes du YZE, pousser un jet **genere un Point de Volonte** (Willpower Point / WP). Ces points peuvent ensuite etre depenses pour :

- Activer certains **talents** speciaux.
- Utiliser des **capacites de classe/role**.
- Alimenter des **pouvoirs speciaux** (mutations dans Mutant: Year Zero, magie dans Forbidden Lands, etc.).

Ce mecanisme cree un cycle : **prendre des risques (push) alimente les capacites heroiques (WP)**.

---

## 6. Talents

### 6.1 Principe general

Les **talents** sont des capacites speciales qui personnalisent le personnage au-dela de ses attributs et competences. Ils fonctionnent comme des "feats" ou "edges" dans d'autres systemes.

### 6.2 Types de talents

Le SRD definit generalement trois categories :

| Categorie | Description |
|---|---|
| **Talents generaux** | Accessibles a tous les personnages |
| **Talents de role/classe** | Lies a un archetype ou une profession specifique |
| **Talents uniques/speciaux** | Lies a la race, l'origine, ou obtenus en jeu |

### 6.3 Niveaux de talents

Certains talents ont **plusieurs niveaux** (rang 1, 2, 3), offrant des effets de plus en plus puissants a mesure qu'on investit des points d'experience dedans.

### 6.4 Fonctionnement typique

Un talent peut :

- **Accorder un bonus passif** : +1 de a un certain type de jet.
- **Permettre une action speciale** : une manoeuvre de combat unique, une capacite sociale.
- **Modifier une regle** : ignorer un malus dans certaines circonstances.
- **Couter un Point de Volonte** pour s'activer (talents actifs).
- **Se declencher automatiquement** dans certaines conditions (talents reactifs).

### 6.5 Exemples de talents typiques

- **Tueur-ne** (Killer Instinct) : +1 de de bonus aux jets d'attaque en melee quand on est blesse.
- **Dur a cuire** (Hard to Kill) : permet de relancer un jet sur la table de blessures critiques.
- **Sixieme sens** (Sixth Sense) : le personnage ne peut pas etre surpris.
- **Rapide comme l'eclair** (Lightning Fast) : permet de degainer et attaquer dans la meme action.
- **Persuasion** (Silver Tongue) : +2 des aux jets de Manipulation dans certaines conditions.
- **Guerison naturelle** (Natural Healer) : soigne un point d'attribut supplementaire lors du repos.

---

## 7. Combat

### 7.1 Structure du combat

Le combat dans le YZE est divise en **rounds**. Chaque round, chaque participant agit une fois.

### 7.2 Initiative

L'initiative determine l'ordre d'action dans un round :

- **Methode par cartes** (Forbidden Lands, Twilight: 2000) : on distribue des **cartes d'initiative** numerotees. Chaque joueur tire une carte ; l'ordre va du chiffre le plus bas au plus eleve.
- **Methode par attribut** (Mutant: Year Zero, Coriolis) : l'initiative est basee sur un jet de des ou directement sur la valeur d'un attribut (souvent **Agilite**).
- **Methode narrative** (Tales from the Loop) : les joueurs decident entre eux de l'ordre.

> Dans tous les cas, les PJ agissent generalement avant les PNJ en cas d'egalite, sauf en cas d'embuscade.

### 7.3 Actions par round

Chaque personnage dispose lors de son tour de :

- **Une action lente** (Slow Action) : une action majeure qui prend du temps.
- **Une action rapide** (Fast Action) : une action mineure, rapide.

**OU** bien le personnage peut effectuer **deux actions rapides** au lieu d'une lente + une rapide.

#### Actions lentes typiques :
| Action | Description |
|---|---|
| Attaquer (melee ou tir) | Jet de Melee ou Tir |
| Premiers soins | Jet de Soins |
| Persuader/Intimider | Jet de Manipulation |
| Recharger une arme | Preparation de l'arme |
| Fuir le combat (Sprint) | Jet de Deplacement |

#### Actions rapides typiques :
| Action | Description |
|---|---|
| Se deplacer | Se deplacer d'une zone a une autre (portee courte) |
| Degainer/Ranger une arme | Preparer ou ranger son equipement |
| Se mettre a couvert | Obtenir un bonus defensif |
| Parer | Preparer une parade (reaction) |
| Utiliser un objet | Boire une potion, activer un appareil |
| Se relever | Se remettre debout apres une chute |
| Crier un ordre | Communiquer brievement |

### 7.4 Attaque en melee

1. Le joueur constitue son pool : **Agilite + Melee** (+ bonus d'arme eventuel).
2. Il lance les des.
3. Chaque **6** = un succes.
4. Il faut **au moins 1 succes** pour toucher.
5. L'adversaire peut tenter de **parer** ou **esquiver** (action rapide) :
   - **Parade** : jet d'Agilite + Melee. Chaque succes annule un succes de l'attaquant.
   - **Esquive** : jet d'Agilite + Deplacement. Chaque succes annule un succes de l'attaquant. Apres l'esquive, le defenseur ne peut plus esquiver ni parer jusqu'a son prochain tour.
6. Les **succes restants** apres la defense determinent les degats et les effets.

### 7.5 Attaque a distance

1. Pool : **Agilite + Tir** (+ bonus d'arme).
2. **Modificateurs de portee** :
   - **Courte portee** : aucun modificateur
   - **Moyenne portee** : -1 de
   - **Longue portee** : -2 des
   - **Extreme portee** : -3 des
3. Autres modificateurs :
   - Cible a couvert : -1 a -2 des
   - Cible en mouvement : -1 de
   - Visee (action lente precedente) : +1 de
   - Obscurite : -1 a -2 des
4. L'esquive est generalement **impossible** contre les armes a distance (sauf talents speciaux).

### 7.6 Jets opposes (combat en melee)

Variante utilisee dans certains jeux : au lieu d'un jet d'attaque suivi d'un jet de defense, les deux combattants lancent simultanement. Celui qui obtient le plus de succes touche l'autre. La difference de succes determine les degats de base.

### 7.7 Succes excedentaires (Stunts)

Les succes au-dela du premier peuvent etre depenses en **prouesses de combat** :

| Prouesse | Cout en succes | Effet |
|---|---|---|
| **Degats supplementaires** | 1 succes | +1 de degats par succes depense |
| **Desarmement** | 2 succes | L'adversaire lache son arme |
| **Mise a terre** | 2 succes | L'adversaire tombe au sol |
| **Saisie** (Grapple) | 2 succes | L'adversaire est agrippe |
| **Position avantageuse** | 2 succes | Bonus au prochain jet |
| **Coup de grace narratif** | Variable | Effet narratif spectaculaire |

> Les prouesses disponibles et leur cout varient selon le jeu.

### 7.8 Zones et mouvement

Le YZE n'utilise generalement **pas de grille** ni de distances en metres. L'espace est divise en **zones** abstraites :

| Portee | Description |
|---|---|
| **Engagee** (Engaged) | Au contact, corps a corps |
| **Courte** (Short) | Quelques metres, dans la meme zone |
| **Moyenne** (Medium) | Zone adjacente, environ 10-25 metres |
| **Longue** (Long) | 2-3 zones de distance, environ 25-100 metres |
| **Extreme** (Extreme) | Au-dela de 100 metres |

Se deplacer d'une zone a une zone adjacente coute **une action rapide**.

---

## 8. Degats, armure et blessures critiques

### 8.1 Calcul des degats

Les degats dependent du type d'attaque :

```
Degats = Degats de base de l'arme + succes excedentaires depenses en degats
```

Chaque arme a une **valeur de degats de base** (typiquement 1 a 3 pour les armes de melee, 1 a 4 pour les armes a feu).

### 8.2 Armure

L'armure fournit un **indice de protection** (typiquement 2 a 8 selon le type).

1. Le defenseur lance un nombre de des egal a son **indice d'armure**.
2. Chaque **6** obtenu **annule 1 point de degat**.
3. Les degats restants sont appliques a un attribut (generalement **Force**).

> Dans certaines variantes, l'armure reduit simplement les degats d'un montant fixe au lieu d'un jet de des.

### 8.3 Application des degats

Les degats reduisent le score courant de l'attribut cible (generalement **Force** pour les degats physiques). Chaque point de degat retire 1 point d'attribut.

### 8.4 Blessures critiques

Quand un attribut atteint **0** suite a des degats, ou quand un personnage subit des degats alors qu'il est deja a 0, il doit effectuer un **jet de blessure critique** sur une table dediee.

#### Table de blessures critiques (exemple generique)

Le joueur lance un **d66** (deux d6 lus comme dizaines et unites : 11 a 66) :

| Resultat | Blessure | Effet |
|---|---|---|
| 11-16 | Souffle coupe | Etourdi 1 round, pas de malus permanent |
| 21-26 | Entorse / Contusion | -1 a un attribut physique pour la duree de la guerison |
| 31-33 | Fracture mineure | -2 a Force ou Agilite, guerison en jours |
| 34-36 | Laceration profonde | Saignement : perd 1 point de Force par round sans soins |
| 41-43 | Fracture grave | Membre inutilisable, guerison en semaines |
| 44-46 | Hemorragie interne | Saignement interne, mort en heures sans chirurgie |
| 51-53 | Organe endommage | Effet grave, guerison en semaines |
| 54-56 | Colonne touchee | Risque de paralysie, guerison longue |
| 61-64 | Blessure mortelle | Mort en d6 rounds sans intervention |
| 65 | Blessure fatale | Mort en d6 minutes |
| 66 | Mort instantanee | Le personnage est tue sur le coup |

> Chaque jeu YZE a sa propre table de blessures critiques adaptee au ton. Forbidden Lands est tres mortel ; Tales from the Loop ne tue jamais les enfants.

### 8.5 Guerison

- **Guerison naturelle** : un point d'attribut recupere par jour de repos complet.
- **Premiers soins** (jet de Soins) : permet de recuperer des points d'attribut immediatement (1 point par succes, generalement).
- **Blessures critiques** : necessitent un traitement specifique et un temps de guerison indique par la table.
- Le push d'un jet de soins peut aggraver la situation.

---

## 9. Conditions et etats

### 9.1 Systeme de conditions (version simplifiee)

Dans les jeux YZE simplifies (Tales from the Loop, Vaesen, etc.), au lieu de perdre des points d'attribut, les personnages accumulent des **Conditions** :

| Condition | Effet |
|---|---|
| **Epuise** (Exhausted) | -1 de a tous les jets physiques |
| **Effraye** (Scared) | -1 de a tous les jets mentaux |
| **Blesse** (Injured) | -1 de a tous les jets physiques (cumulable avec Epuise) |
| **Demoralise** (Upset) | -1 de a tous les jets sociaux/mentaux |

- Chaque condition se coche sur la feuille de personnage.
- Les conditions se cumulent et empilent les malus.
- Si un personnage doit prendre une condition qu'il a deja, il est **hors de combat** (Broken).
- **Un personnage Broken** ne peut plus agir et doit etre aide par un autre personnage.

### 9.2 Recuperation des conditions

- Le repos, les soins, ou certaines scenes narratives (un repas chaud, un moment de reconfort) permettent de retirer une condition.
- Chaque condition a generalement une methode de recuperation specifique :
  - **Epuise** : dormir une nuit complete
  - **Effraye** : etre reconforte par un allie, atteindre un lieu sur
  - **Blesse** : recevoir des soins medicaux
  - **Demoralise** : moment de repos emotionnel, soutien social

---

## 10. Stress et panique (variante ALIEN RPG)

Le systeme de Stress est l'une des variantes les plus distinctives du YZE, utilisee principalement dans ALIEN RPG.

### 10.1 Des de Stress

- Le personnage a un compteur de **Stress** (de 0 a 10+).
- A chaque jet, le joueur ajoute un nombre de **des de Stress** (d'une couleur differente, typiquement jaune) egal a son niveau de Stress actuel.
- Les des de Stress comptent normalement pour les succes (un 6 = succes).
- **MAIS** : chaque **1** sur un de de Stress declenche un **test de Panique**.

### 10.2 Accumulation du Stress

Le Stress augmente dans les situations suivantes :
- Etre temoin d'une scene horrifique ou violente
- Etre blesse
- Etre dans le noir
- Un allie est tue ou grievement blesse
- Echouer a une action critique
- Pousser un jet (+1 Stress)
- Effets de certaines creatures ou situations

### 10.3 Table de Panique

Quand la panique se declenche, le joueur lance **1d6 + niveau de Stress actuel** :

| Resultat | Reaction |
|---|---|
| 1-6 | Pas d'effet visible |
| 7 | Tremblement : -1 de au prochain jet |
| 8 | Cri de terreur : attire l'attention |
| 9 | Peur debilitante : laisse tomber un objet tenu |
| 10 | Fuite : le personnage doit fuir (action rapide) |
| 11 | Evanouissement : le personnage s'evanouit 1 round |
| 12 | Terreur : attaque un allie proche ou fuit en hurlant |
| 13 | Folie passagere : comportement irrationnel pour d6 rounds |
| 14 | Catatonie : le personnage est paralyse, ne fait rien pendant d6 rounds |
| 15+ | Crise cardiaque / Effondrement : le personnage subit des degats critiques |

> **La panique est contagieuse** : quand un personnage panique, les allies proches gagnent +1 Stress.

### 10.4 Reduction du Stress

- **Repos** dans un endroit sur : -1 Stress
- **Soutien d'un allie** (jet d'Empathie reussi) : -1 Stress
- **Reussir une action importante** : -1 Stress (certains MJ)
- **Consommables** (medicaments, alcool) : reduction temporaire

---

## 11. Equipement et encombrement

### 11.1 Bonus d'equipement

Chaque objet utile peut apporter un **bonus d'equipement** sous forme de des supplementaires (des d'Equipement, noirs) :

| Qualite de l'equipement | Bonus |
|---|---|
| Improvise / mediocre | +0 |
| Standard | +1 |
| Bon / Superieur | +2 |
| Exceptionnel / Chef-d'oeuvre | +3 |

### 11.2 Deterioration de l'equipement

Quand on **pousse un jet** et que des des d'Equipement affichent un **1** :

- Chaque 1 reduit le **bonus de l'equipement de 1**.
- Quand le bonus atteint **0**, l'objet est **casse** et inutilisable jusqu'a reparation.
- La reparation necessite un jet d'**Artisanat** et du temps/materiaux.

### 11.3 Encombrement

Le systeme d'encombrement varie selon le jeu mais suit generalement ces principes :

- Chaque objet a un **poids en unite d'encombrement** (typiquement 1 pour un objet leger, 2-4 pour un objet lourd).
- La **capacite de transport** est liee a la **Force** du personnage (generalement Force x 2).
- Depasser sa capacite impose des malus aux jets physiques.

### 11.4 Consommables

Le YZE utilise un systeme de **Des de Ressource** (Resource Die) pour gerer les consommables (nourriture, eau, munitions, torches) :

1. Le consommable a un **de de ressource** (d6, d8, d10, d12).
2. A chaque utilisation (ou a intervalles reguliers), on lance le de de ressource.
3. Un resultat de **1 ou 2** signifie que le de **diminue d'un cran** (d12 -> d10 -> d8 -> d6).
4. Quand le d6 donne 1 ou 2, la ressource est **epuisee**.

> Ce systeme evite le comptage fastidieux unite par unite et cree une tension narrative autour de la rarefaction des ressources.

---

## 12. Experience et progression

### 12.1 Points d'experience (XP)

Les personnages gagnent des **points d'experience** (XP) a la fin de chaque session ou scenario. Les criteres typiques :

- **Participation a la session** : 1 XP
- **Surmonter un defi significatif** : 1 XP
- **Jouer selon son role/archetype** : 1 XP
- **Mettre en jeu ses defauts/relations** : 1 XP
- **Apprendre quelque chose de nouveau** : 1 XP

### 12.2 Depenses d'XP

| Amelioration | Cout typique |
|---|---|
| Augmenter une competence de 1 niveau | 5-10 XP (x nouveau niveau) |
| Acquerir un nouveau talent | 5-10 XP |
| Ameliorer un talent existant (rang superieur) | 5-10 XP (x nouveau rang) |
| Augmenter un attribut | Tres couteux (15-20 XP), souvent limite |

> Les attributs sont rarement augmentables par l'XP dans le YZE. La progression se fait surtout via les **competences** et les **talents**.

### 12.3 Progression narrative

Le YZE encourage aussi une progression non mecanique :
- Acquisition d'allies, de reputation, de territoire.
- Evolution des relations avec les PNJ.
- Changement de la situation du monde (surtout dans Mutant: Year Zero avec la gestion de la communaute).

---

## 13. Autres mecaniques fondamentales

### 13.1 Jets de groupe

Quand plusieurs personnages cooperent :
- Un personnage est designe comme **leader**.
- Chaque assistant qui reussit un jet accorde **+1 de** au leader.
- Seul le leader fait le jet final.

### 13.2 Jets etendus

Certaines taches complexes necessitent plusieurs succes accumules sur plusieurs tours/periodes :
- Le MJ fixe un **nombre total de succes requis**.
- A chaque tour/periode, le personnage fait un jet et accumule les succes.
- L'echec ou les complications peuvent survenir entre les jets.

### 13.3 Rencontres aleatoires

Le SRD prevoit des mecaniques pour les **rencontres aleatoires** lors des voyages ou explorations :
- A intervalles reguliers, le MJ lance un d6.
- Sur un 1, un evenement se produit (rencontre, meteo, decouverte).

### 13.4 Repos et recuperation

Le YZE distingue generalement :
- **Repos court** (quelques heures) : recuperation limitee, un jet de soins possible.
- **Repos long** (nuit complete) : recuperation d'un ou plusieurs points d'attribut, retrait de certaines conditions.
- **Repos prolonge** (plusieurs jours) : necessaire pour guerir les blessures critiques.

### 13.5 Points sombres / Points de destin (Dark Points)

Dans certaines variantes du YZE :
- Quand les joueurs poussent des jets, le MJ recoit des **Points Sombres** (Darkness Points dans Coriolis).
- Le MJ peut depenser ces points pour activer des effets narratifs negatifs, des complications ou des capacites des antagonistes.
- Cela cree une **economie de tension** : les joueurs veulent pousser pour reussir, mais alimentent ainsi les menaces du MJ.

### 13.6 Relations et PNJ

Chaque personnage a generalement :
- Un **PNJ Protecteur** (Buddy/NPC to Protect) : quelqu'un qu'il veut proteger.
- Un **PNJ Rival** : quelqu'un avec qui il est en conflit.
- Un **Objet precieux** (Big Dream / Pride) : un objectif personnel ou un trait de fierte.
- Un **Defaut** (Dark Secret / Problem) : un probleme qui le poursuit.

Ces elements sont des leviers narratifs que le MJ est encourage a utiliser pour creer du drame.

### 13.7 Magie et pouvoirs speciaux (variantes)

Selon le jeu, le YZE peut inclure des sous-systemes pour :

- **Mutations** (Mutant: Year Zero) : pouvoirs alimentes par les Points de Mutation (obtenus en poussant des jets). Utiliser une mutation peut causer des degats ou des effets secondaires.
- **Magie** (Forbidden Lands) : les sorts consomment des Points de Volonte et peuvent etre surcharges pour plus de puissance, au risque d'un contrecoup magique (mishap).
- **Prieres mystiques** (Coriolis) : alimentees par les Points Sombres, creant un pacte faustien avec les tenebres.
- **Pouvoirs psychiques** ou technologiques selon le cadre.

### 13.8 Vehicules

Le SRD propose un cadre pour les vehicules :
- Les vehicules ont leurs propres **attributs** (Coque, Moteur, etc.) et des **bonus d'equipement**.
- Le combat vehiculaire suit les memes principes que le combat personnel, avec des adaptations de portee et d'echelle.
- Les vehicules peuvent subir des **avaries critiques** similaires aux blessures critiques.

### 13.9 Construction de base / Gestion communautaire

Certains jeux YZE (Mutant: Year Zero, Forbidden Lands) incluent un sous-systeme de gestion :
- Les PJ gerent un **lieu** (Arche dans Mutant, Forteresse dans Forbidden Lands).
- Ils investissent des ressources dans des **projets** de developpement.
- Des evenements aleatoires menacent la communaute entre les sessions.

---

## Resume des mecaniques cles du YZE

| Mecanique | Description |
|---|---|
| **Pool de d6** | Attribut + Competence + Equipement |
| **Succes** | Chaque 6 = 1 succes |
| **Push** | Relancer les non-6, mais risque de degats (1 sur des de Base/Equipement) |
| **Points de Volonte** | Gagnes en poussant, depenses pour talents/pouvoirs |
| **Actions** | 1 action lente + 1 action rapide par round |
| **Degats** | Reduisent les attributs ; attribut a 0 = blessure critique |
| **Armure** | Jet de des d'armure, chaque 6 annule 1 degat |
| **Conditions** | Etats negatifs (-1 de), cumul possible |
| **Zones** | Espace abstrait, pas de grille |
| **Consommables** | De de Ressource decroissant |
| **Progression** | XP pour competences et talents |

---

## Notes pour la conception d'un systeme personnalise

Points forts du YZE a considerer :
- La mecanique de **push** est la pierre angulaire : risque/recompense elegant.
- Le systeme de **zones** fluidifie les combats sans sacrifier la tactique.
- Les **des d'equipement** ajoutent une dimension strategique sans alourdir le jeu.
- Le **de de Ressource** pour les consommables est elegant et anti-comptabilite.
- La modularite permet d'ajouter ou retirer des sous-systemes (stress, magie, vehicules) selon le besoin.

Points a adapter :
- La mortalite est tres variable selon les tables de critiques -- a calibrer selon le ton souhaite.
- Le nombre d'attributs (4) et de competences (12) peut etre ajuste.
- Le systeme de Push peut etre modifie pour des consequences differentes selon le genre (horreur = stress, heroique = fatigue, etc.).
- Les stunts/prouesses en combat sont un levier important de personalisation tactique.

---

> *Document de reference compile pour le projet de conception de systeme de JdR personnalise.*
> *Basee sur le Year Zero Engine SRD de Free League Publishing.*
