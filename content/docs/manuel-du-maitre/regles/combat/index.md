---
title: "Combat"
subtitle: "Rounds · Attaque · Défense · Dégâts"
description: "Les règles de combat d'Isekai YZE : structure du round, attaque et défense, dégâts, armure, zones et guérison."
weight: 20
draft: false
---

> *Le combat n'est pas une suite d'échanges propres — c'est une pression qui monte, des choix faits en une fraction de seconde, des corps qui cèdent avant les esprits.*

---

## Séquence d'un échange

Chaque fois qu'un personnage attaque, les étapes se déroulent dans cet ordre :

1. **L'attaquant lance son pool** — Force + Mêlée (ou Agilité + Tir) + bonus d'arme. Chaque 6 est un succès.
2. **Le défenseur réagit** — il peut parer (Agilité + Mêlée) ou esquiver (Agilité + Déplacement). Chaque succès en défense annule un succès de l'attaquant.
3. **Les succès restants deviennent des dégâts** — valeur de base de l'arme, augmentée par les succès excédentaires dépensés.
4. **L'armure absorbe une partie des dégâts** — le défenseur lance ses dés d'armure ; chaque 6 annule 1 point de dégât.
5. **Les dégâts restants réduisent la Santé** du défenseur. Si elle atteint 0, il est brisé.

---

## Structure du round

Le combat se déroule en **rounds**. Chaque round, chaque participant dispose de :

- **1 action lente** — attaquer, soigner, persuader, activer un talent complexe…
- **1 action rapide** — se déplacer d'une zone, dégainer, se mettre à couvert, se relever…

Il est possible d'échanger l'action lente contre une seconde action rapide.

---

## Initiative

L'initiative détermine l'ordre dans lequel les participants agissent chaque round.

> La méthode exacte (cartes d'initiative, jet d'Agilité, approche narrative) est encore à l'étude. Le MJ peut utiliser la méthode qui correspond le mieux au ton de sa table.

---

## Zones et déplacement

Le combat n'utilise pas de grille. L'espace est organisé en **zones abstraites**, définies librement par le MJ selon l'environnement.

| Portée | Distance approximative | Armes adaptées |
|---|---|---|
| **Engagée** | Au contact, corps à corps | Armes de mêlée, couteaux |
| **Courte** | Même zone, quelques mètres | Arbalètes légères, javelots |
| **Moyenne** | Zone adjacente, ~10–25 m | Arcs, arbalètes |
| **Longue** | 2–3 zones, ~25–100 m | Arcs longs |
| **Extrême** | Au-delà de 100 m | Arcs de siège, situations rares |

Se déplacer vers une zone adjacente coûte **une action rapide**. Traverser plusieurs zones demande plusieurs actions ou un effort particulier.

{{< hint info >}}
Les zones sont volontairement abstraites. Une pièce entière peut être une zone unique ; une ruelle peut en contenir deux ou trois. Le MJ adapte selon la situation.
{{< /hint >}}

---

## Attaque

### Corps à corps

```
Pool = Force + Mêlée + Bonus d'arme (0 à 2)
```

- **1 succès** = la frappe touche.
- **Succès excédentaires** = convertis en dégâts supplémentaires ou en prouesses de combat.

### Tir

```
Pool = Agilité + Tir + Bonus d'arme (0 à 2)
```

Même logique que le corps à corps. La portée de l'arme détermine si la cible est à portée valide.

---

## Défense

Lorsqu'une attaque touche, le défenseur peut tenter de l'annuler avec une réaction.

| Réaction | Pool | Limite |
|---|---|---|
| **Parade** | Agilité + Mêlée | Disponible à chaque attaque reçue |
| **Esquive** | Agilité + Déplacement | Une seule fois par round — empêche toute parade ou esquive ultérieure jusqu'au prochain tour |

Chaque succès en défense **annule un succès de l'attaquant**. Si tous les succès sont annulés, l'attaque ne touche pas et aucun dégât n'est infligé.

{{< hint warning >}}
Après une esquive, le personnage ne peut plus parer ni esquiver jusqu'à son prochain tour. Esquiver est efficace mais coûteux.
{{< /hint >}}

---

## Dégâts

Les succès non annulés par la défense se convertissent en dégâts.

```
Dégâts = Valeur de base de l'arme + succès excédentaires dépensés
```

Ces dégâts sont d'abord soumis à l'armure, puis déduits de la **Santé** du défenseur.

---

## Armure

L'armure absorbe une partie des dégâts avant qu'ils n'atteignent la Santé. Ce jet se fait après le calcul des dégâts, indépendamment du jet de défense.

Chaque armure possède un **indice de protection** (de 1 à 8 selon le type). Le défenseur lance un nombre de dés égal à cet indice :

```
Chaque 6 obtenu = 1 point de dégât annulé
```

Les dés d'armure sont des dés noirs (Équipement). Un 1 au push sur un dé d'armure réduit l'indice de protection de 1 — l'armure s'use sous les coups.

| Type d'armure | Indice approximatif |
|---|---|
| Vêtements épais, cuir souple | 1–2 |
| Cuir durci, brigandine | 3–4 |
| Cottes de mailles | 5–6 |
| Armure de plates | 7–8 |

---

## Santé et brisure

Les dégâts qui passent l'armure réduisent la **Santé** courante du défenseur.

```
Santé = ⌈(Force + Agilité) / 2⌉ + 1
```

Quand la Santé atteint **0**, le personnage est **brisé** : il s'effondre et ne peut plus agir normalement. Il doit alors effectuer un jet de **blessure critique**.

{{< hint danger >}}
Un personnage brisé est hors de combat. Sans soins rapides, la blessure critique peut avoir des conséquences durables — voire fatales.
{{< /hint >}}

---

## Guérison

La Santé et les attributs ne récupèrent pas d'eux-mêmes entre deux rounds. Il faut du temps, du repos, ou des soins.

| Méthode | Effet |
|---|---|
| Jet de Soins réussi | +1 point d'attribut par succès |
| Repos court (quelques heures) | Permet un jet de Soins |
| Repos long (nuit complète) | Récupère 1 point d'attribut |
| Repos prolongé (plusieurs jours) | Nécessaire pour les blessures critiques |

Les blessures critiques requièrent un traitement spécifique et du temps de récupération pour être surmontées.
