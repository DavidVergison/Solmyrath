# Règles de base — Isekai YZE

> Noyau mécanique du système. Basé sur le Year Zero Engine (SRD Free League Publishing).

---

## Attributs

Le personnage est défini par quatre attributs, notés de **2 à 5** à la création.

| Attribut | Ce qu'il représente |
|----------|---------------------|
| **Force** | Puissance musculaire brute et courage |
| **Agilité** | Maîtrise du corps, vitesse et habileté motrice |
| **Esprit** | Perception sensorielle, intelligence et santé mentale |
| **Empathie** | Charisme personnel et capacité à influencer les autres |

**Répartition à la création** : 14 points à distribuer librement entre les quatre attributs (minimum 2, maximum 5 par attribut).

---

## Jauges

Les jauges ne sont pas des attributs : elles mesurent la capacité du personnage à encaisser avant d'être **brisé**.

### Santé

> Combien de dégâts physiques le personnage peut subir avant de s'effondrer.

```
Santé = ⌈(Force + Agilité) / 2⌉ + 1
```

Chaque point de dégât physique réduit la Santé courante de 1. Quand elle atteint **0**, le personnage est **brisé** : il s'effondre et doit effectuer un jet de **blessure critique**.

### Résolution

> Combien de stress, de peur et de pression mentale le personnage peut endurer avant de craquer.

```
Résolution = ⌈(Esprit + Empathie) / 2⌉ + 1
```

La Résolution intervient dans la mécanique de magie (voir `magie.md`). Quand elle atteint **0**, le personnage est **brisé** mentalement et subit un effet de **trauma**.

---

## Compétences

Chaque compétence est liée à un attribut. Le **pool de dés** d'une action est :

```
Pool = Attribut lié + Niveau de compétence (+ dés d'Équipement éventuels)
```

Un personnage peut tenter une action sans posséder la compétence correspondante : il lance alors uniquement les **dés de Base** (l'attribut seul, compétence à 0).

### Liste des 20 compétences (5 par attribut)

#### Force

| Compétence | Usage |
|------------|-------|
| **Puissance** | Soulever, forcer, pousser |
| **Mêlée** | Combat au corps à corps |
| **Endurance** | Résister à la fatigue, marche forcée |
| **Artisanat** | Fabriquer, forger, réparer |
| **Intimidation** | Menace physique, cri de guerre, imposer sa présence |

#### Agilité

| Compétence | Usage |
|------------|-------|
| **Discrétion** | Se cacher, se déplacer silencieusement |
| **Escamotage** | Pickpocket, tours de passe-passe, crocheter |
| **Déplacement** | Courir, sauter, escalader, nager |
| **Tir** | Armes à distance |
| **Équitation** | Montures, combat monté, poursuites |

#### Esprit

| Compétence | Usage |
|------------|-------|
| **Fouille** | Détecter, pister, percevoir |
| **Érudition** | Connaissances, langues, savoirs académiques |
| **Survie** | Orientation, chasse, milieu sauvage |
| **Perspicacité** | Lire une situation, analyser un problème, détecter un mensonge |
| **Arcanes** | Lancer des sorts, identifier la magie, traditions magiques |

#### Empathie

| Compétence | Usage |
|------------|-------|
| **Manipulation** | Persuader, mentir, négocier, séduire |
| **Prestance** | Inspirer, divertir, charisme public |
| **Soins** | Médecine, premiers soins |
| **Dressage** | Apprivoiser, commander des animaux |
| **Commandement** | Diriger un groupe, coordonner en combat, donner des ordres |

**Répartition à la création** : toutes les compétences démarrent à **0**. Les compétences d'archétype sont fixées entre 1 et 3. Le joueur répartit ensuite des points supplémentaires librement (nombre exact à calibrer — voir point d'attention ci-dessous).

> **Point d'attention** : avec 20 compétences au lieu de 12, l'ancien barème (toutes à 1 + 10 points) n'est plus adapté. Le nombre de points à distribuer doit être recalibré pour que les personnages restent compétents dans leur niche sans être bons partout. Sujet à trancher séparément.

---

## Mécanique de résolution

### Lancer les dés

Constituer le pool de dés et lancer. Chaque **6** est un **succès**.

- **1 succès** = l'action réussit.
- **Chaque succès excédentaire** peut être dépensé en **prouesse** (effet supplémentaire, dégâts bonus, avantage tactique, etc.).
- **Aucun 6** = échec.

### Pousser le jet (*Push*)

Après un jet raté (ou jugé insuffisant), le joueur peut **pousser** :

1. Relancer tous les dés qui n'affichent **pas** un 6. Les succès déjà obtenus sont conservés.
2. Un jet ne peut être poussé qu'**une seule fois**.

**Conséquences du push selon le type de dé :**

| Type de dé | Couleur | Effet d'un 1 au push |
|-----------|---------|----------------------|
| **Dés de Base** (Attribut) | Jaune | −1 point à l'attribut correspondant |
| **Dés de Compétence** | Bleu | Aucune conséquence |
| **Dés d'Équipement** | Noir | −1 au bonus de l'objet (usure) |
| **Dés de Résolution** (magie) | Violet | Blessure magique (voir `magie.md`) |

> Le push est le cœur du YZE : il offre une seconde chance, mais à un coût. C'est au joueur de décider si le risque vaut la peine.

---

## Points de Volonté (PV)

Les Points de Volonté représentent la détermination et la concentration du personnage. Ils alimentent les **talents actifs** (physiques et mentaux).

### Génération

Chaque fois qu'un joueur **pousse un jet**, il gagne **1 PV**, que le push réussisse ou échoue. Le push reste risqué (dégâts d'attribut, usure, blessure magique), mais il génère toujours cette ressource.

### Réserve maximale

```
Réserve PV max = meilleur attribut du personnage
```

Avec des attributs de 2 à 5, la réserve est typiquement de **3 à 5 PV**. Les PV excédentaires au-delà de la réserve max sont perdus.

### Début de session

Le personnage commence chaque session avec sa **réserve pleine**.

### Dépense

Les PV sont dépensés pour activer des **talents actifs**. Le coût en PV dépend du talent (voir `guide-equilibrage-talents.md`).

> **Note** : la Résolution reste exclusivement réservée à la magie (dés de Magie pour les sorts). Les PV couvrent tout le reste : talents de combat, de survie, de social, etc.

---

## Combat

### Principe

Le combat est divisé en **rounds**. Chaque round, chaque participant dispose de :

- **1 action lente** : attaquer, lancer un sort, soigner, persuader...
- **1 action rapide** : se déplacer d'une zone, dégainer, se mettre à couvert, se relever...

Ou bien **2 actions rapides** à la place.

### Initiative

À définir (cartes d'initiative, jet d'Agilité, ou méthode narrative — à trancher selon le ton souhaité).

### Attaque au corps à corps (guerrier)

```
Pool = Force + Mêlée + Bonus d'arme (0–2)
```

- Chaque couleur de dé est distincte pour identifier les conséquences au push.
- **1 succès** = touche. Chaque **succès excédentaire** peut être converti en dégâts supplémentaires ou en prouesses de combat.

### Défense

- **Parade** : jet d'Agilité + Mêlée. Chaque succès annule un succès de l'attaquant.
- **Esquive** : jet d'Agilité + Déplacement. Chaque succès annule un succès de l'attaquant. Après l'esquive, le défenseur ne peut plus esquiver ni parer jusqu'à son prochain tour.

### Dégâts

```
Dégâts = Valeur de base de l'arme + succès excédentaires dépensés
```

Les dégâts réduisent la **Santé** courante du défenseur. Si la Santé atteint **0**, le personnage est **brisé** et doit effectuer un jet de **blessure critique**.

### Armure

L'armure fournit un **indice de protection** (1 à 8 selon le type). Lancer un nombre de dés égal à cet indice : chaque **6** annule 1 point de dégât.

### Zones et déplacement

Le combat n'utilise pas de grille. L'espace est organisé en **zones** abstraites :

| Portée | Distance approximative |
|--------|----------------------|
| **Engagée** | Au contact, corps à corps |
| **Courte** | Quelques mètres, même zone |
| **Moyenne** | Zone adjacente, ~10–25 m |
| **Longue** | 2–3 zones, ~25–100 m |
| **Extrême** | Au-delà de 100 m |

Se déplacer d'une zone à une zone adjacente coûte **une action rapide**.

---

## Guérison

| Méthode | Effet |
|---------|-------|
| **Repos court** (quelques heures) | 1 jet de Soins possible |
| **Repos long** (nuit complète) | Récupère 1 point d'attribut |
| **Repos prolongé** (plusieurs jours) | Nécessaire pour les blessures critiques |
| **Jet de Soins réussi** | 1 point d'attribut récupéré par succès |

---

## Questions ouvertes

- [ ] Méthode d'initiative retenue ?
- [ ] Table de blessures critiques (d66 générique à adapter) ?
- [ ] Prouesses de combat disponibles et leurs coûts en succès ?
- [ ] **Défense et talents de Kin** : le talent "Sur ses gardes" (Vif) donne −1 dé attaquant si le Vif s'est déplacé ce round. À préciser : (1) "s'être déplacé" = avoir utilisé son action de déplacement, ou tout mouvement même gratuit ? (2) interaction avec l'esquive existante (Agilité + Déplacement) — cumul ou substitution ? (3) décider si les talents de Kin passifs peuvent modifier les jets adverses de façon générale.
- [x] Points de Volonté : **adoptés** — générés par le push (1 PV/push), dépensés pour les talents actifs, réserve max = meilleur attribut du personnage
