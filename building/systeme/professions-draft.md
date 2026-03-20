# Professions — Index & Notes de conception

> Les fiches détaillées sont dans `building/professions/`. Ce fichier conserve les conventions, tableaux récapitulatifs et notes d'équilibrage.

---

## Conventions

- **Attribut-clé** : l'attribut privilégié par la profession (guide la répartition des points à la création)
- **Compétences de départ** : 3-4 compétences recevant des niveaux gratuits (entre parenthèses). Niveaux de 1 à 3 selon l'importance pour le rôle
- **Arcanes** : niveau de départ en compétence Arcanes. `—` = pas d'accès privilégié (le personnage peut toujours prendre Arcanes via héritage Visiteur ou Kin magique)
- **École** : école de magie associée. Détermine les sorts accessibles
- **Talents exclusifs** : 2-3 talents à 3 rangs, réservés à la profession. Suivent l'échelle du guide d'équilibrage :
  - **R1** (Novice) : bonus modeste, ouverture
  - **R2** (Adepte) : option tactique, effet secondaire
  - **R3** (Maître) : capacité culminante, redéfinit les règles
- **Kins bien assorties** : suggestions thématiques, jamais restrictives

---

## Liste des professions

### Combat
1. [Lame-Lige](../professions/lame-lige.md) — Guerrier (Force)
2. [Sentinelle](../professions/sentinelle.md) — Archer / Éclaireur (Agilité)
3. [Lame-Vive](../professions/lame-vive.md) — Roublard combattant (Agilité)
4. [Poing-du-Vide](../professions/poing-du-vide.md) — Moine (Force)

### Magie
5. [Érudit des Arcanes](../professions/erudit-des-arcanes.md) — Mage (Esprit)
6. [Porteur de Pacte](../professions/porteur-de-pacte.md) — Occultiste (Esprit)
7. [Oracle du Temps](../professions/oracle-du-temps.md) — Chronomancien (Esprit)
8. [Artisan Runique](../professions/artisan-runique.md) — Forgeur d'enchantements (Force)
9. [Herboriste](../professions/herboriste.md) — Alchimiste / Apothicaire (Esprit)

### Support
10. [Main-qui-Guérit](../professions/main-qui-guerit.md) — Clerc (Empathie)
11. [Chantelame](../professions/chantelame.md) — Barde (Empathie)
12. [Maître des Liens](../professions/maitre-des-liens.md) — Dresseur / Invocateur (Empathie)

### Hybrides
13. [Gardien Sylvestre](../professions/gardien-sylvestre.md) — Druide-Ranger (Empathie)
14. [Porte-Honneur](../professions/porte-honneur.md) — Samurai / Paladin (Force)
15. [Ombre-Marchande](../professions/ombre-marchande.md) — Espion / Négociant (Agilité)

### Trait de background
- [Visiteur](../professions/visiteur.md) — Âme d'un autre monde

---

## Tableaux récapitulatifs

### Distribution par attribut-clé

| Attribut | Professions | Nombre |
|----------|-------------|--------|
| Force | Lame-Lige, Poing-du-Vide, Artisan Runique, Porte-Honneur | 4 |
| Agilité | Sentinelle, Lame-Vive, Ombre-Marchande | 3 |
| Esprit | Érudit des Arcanes, Porteur de Pacte, Oracle du Temps, Herboriste | 4 |
| Empathie | Main-qui-Guérit, Chantelame, Maître des Liens, Gardien Sylvestre | 4 |

### Distribution magique

| Type | Professions | Nombre |
|------|-------------|--------|
| Non-magique | Lame-Lige, Sentinelle, Lame-Vive, Ombre-Marchande | 4 |
| Magique pur | Érudit, Porteur de Pacte, Oracle, Artisan, Herboriste, Main-qui-Guérit, Chantelame, Maître des Liens | 8 |
| Hybride (Arcanes 1) | Poing-du-Vide, Porte-Honneur | 2 |
| Hybride nature | Gardien Sylvestre | 1 |

### Écoles de magie couvertes

| École | Profession(s) |
|-------|---------------|
| Savante | Érudit des Arcanes |
| Adeptes Corporels | Poing-du-Vide |
| Druidique | Gardien Sylvestre |
| Divine | Main-qui-Guérit, Porte-Honneur (choix) |
| Pactisée | Porteur de Pacte |
| Alchimique | Herboriste |
| Chronique | Oracle du Temps |
| Bardique | Chantelame |
| Totémique | Maître des Liens, Porte-Honneur (choix) |
| Artisans Runique | Artisan Runique |

> Les 10 écoles sont toutes rattachées à au moins une profession.

### Compétences de départ — vérification des doublons

| Profession | Comp 1 (3) | Comp 2 (2) | Comp 3 (1-2) | Comp 4 (1) |
|------------|------------|------------|--------------|------------|
| Lame-Lige | Mêlée | Endurance | Intimidation | Commandement |
| Sentinelle | Tir | Fouille, Discrétion | — | Survie |
| Lame-Vive | — | Mêlée, Discrétion, Déplacement | — | Escamotage |
| Poing-du-Vide | — | Mêlée, Déplacement | — | Endurance, Arcanes |
| Érudit | Arcanes | Érudition | — | Perspicacité, Fouille |
| Porteur Pacte | — | Arcanes, Manipulation, Perspicacité | — | Érudition |
| Oracle | — | Arcanes | Perspicacité (3) | Érudition, Fouille |
| Artisan Runique | Artisanat | Arcanes | — | Érudition, Puissance |
| Herboriste | — | Arcanes, Soins, Survie | — | Érudition |
| Main-qui-Guérit | Soins | Arcanes | — | Commandement, Prestance |
| Chantelame | Prestance | Arcanes | — | Manipulation, Érudition |
| Maître Liens | Dressage | Arcanes | — | Survie, +1 libre |
| Gardien Sylvestre | — | Survie, Arcanes | — | Mêlée, Dressage/Tir |
| Porte-Honneur | — | Mêlée, Endurance | — | Arcanes, Commandement/Prestance |
| Ombre-Marchande | — | Manipulation, Discrétion, Escamotage | — | Perspicacité |

> Aucun doublon exact — chaque profession a un profil de compétences unique.

---

## Points d'équilibrage et notes de conception

### Points à surveiller

1. **Esprit surchargé** : 4 professions magiques pures ont Esprit comme attribut-clé. Inhérent car Arcanes est lié à Esprit. Contrebalancé par Artisan Runique et Poing-du-Vide (Force).

2. **Lame-Vive vs Ombre-Marchande** : deux profils Agilité. Niches clairement distinctes — Lame-Vive = combat (Mêlée, Déplacement, Frappe Décisive), Ombre-Marchande = social/infiltration (Manipulation, Escamotage, Réseau). Pas de chevauchement significatif en talents.

3. **Hybrides** : Poing-du-Vide et Porte-Honneur commencent avec Arcanes 1. Moins bons mages ET moins bons guerriers purs que les spécialistes — leur valeur est la polyvalence et l'accès à des buffs personnels.

4. **Gardien Sylvestre vs Maître des Liens** : tous deux Empathie + magie nature. Distinction nette : Gardien = druide territorial (Changeforme, Territoire, survie en nature), Maître = dresseur/invocateur (compagnon animal, esprits, communication).

5. **Oracle du Temps** : profession potentiellement surpuissante en narratif (Transe Temporelle R3). Limitations strictes : 1 fois par session, forte dépendance du MJ pour la gestion. À tester en jeu.

6. **Équilibre talents R3** : chaque talent R3 est puissant mais limité (1x/session, 1x/combat, coût élevé en PV). Aucun R3 ne devrait rendre obsolète un autre talent de même rang.

### Règles d'interaction entre professions

- **Non-cumul des auras** : si deux talents accordent le même bonus de zone (ex: Dévotion R3 et Discipline du Code R3 donnent tous deux +1 dé résistance mentale), seul le plus fort s'applique — pas de cumul.
- **Herboriste vs Main-qui-Guérit (soin)** : chevauchement intentionnel. L'Herboriste excelle en soin logistique (potions hors combat, volume total élevé). La Main-qui-Guérit excelle en soin tactique (zone, instantané, bouclier). Les deux dans un groupe ne se cannibalisent pas.
- **Maître des Liens (action economy)** : à R3, le Maître peut avoir 3 entités actives (lui + compagnon autonome + esprit invoqué). Limitation : le Maître ne peut pas lancer de sort pendant qu'il utilise les sens du compagnon (concentration exclusive).

### Compétences non couvertes en départ

- **Équitation** : aucune profession ne la priorise. Normal — c'est une compétence de niche, accessible via les talents généraux ou le choix libre.

> Toutes les autres compétences sont couvertes par au moins une profession.
