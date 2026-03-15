# Design et Equilibre des Systemes de Magie en JDR

Document de recherche sur la theorie du game design appliquee aux systemes de magie dans les JDR sur table, avec un focus sur le Year Zero Engine.

---

## Table des matieres

1. [Le probleme martial/lanceur de sorts](#1-le-probleme-martiallanceur-de-sorts)
2. [Archetypes de systemes de magie](#2-archetypes-de-systemes-de-magie)
3. [Principes de design pour l'equilibre](#3-principes-de-design-pour-lequilibre)
4. [Ce qui rend la magie FUN](#4-ce-qui-rend-la-magie-fun)
5. [La magie dans le Year Zero Engine](#5-la-magie-dans-le-year-zero-engine)
6. [Synthese et recommandations](#6-synthese-et-recommandations)

---

## 1. Le probleme martial/lanceur de sorts

### 1.1. Le constat historique

Le desequilibre entre personnages martiaux et lanceurs de sorts est l'un des problemes les plus anciens et les plus documentes du JDR. Il est souvent appele le "Linear Fighter, Quadratic Wizard" problem : la puissance d'un guerrier progresse de maniere lineaire (meilleur bonus d'attaque, plus de PV, meilleur equipement) tandis que celle d'un mage progresse de maniere exponentielle (acces a des sorts de plus en plus puissants qui redefissent les regles du jeu).

**Les trois axes du probleme :**

- **Axe du combat** : A bas niveau, le mage est fragile et lance un sort par jour. Le guerrier domine. A haut niveau, le mage peut arreter le temps, teleporter le groupe, desintegrer des murs. Le guerrier peut... frapper un peu plus fort.
- **Axe de l'exploration/utilite** : Le guerrier peut escalader un mur. Le mage peut voler, se teleporter, devenir invisible, lire les pensees, invoquer des serviteurs... La magie offre des solutions a des problemes que les martiaux ne peuvent tout simplement pas aborder.
- **Axe narratif** : Les sorts de haut niveau (Wish, Miracle, etc.) permettent aux mages de transformer le monde. Les martiaux restent limites a des actions physiquement plausibles.

### 1.2. Comment les differents jeux abordent le probleme

#### D&D 5e : Echec partiel

D&D 5e a tente de reduire l'ecart en ajoutant des capacites surnaturelles aux martiaux (manoeuvres du Battle Master, Rage du Barbare comme quasi-surnaturel) et en limitant les sorts (concentration comme goulet d'etranglement). Cependant :
- Le systeme de concentration est une bonne idee : il empeche le "buff stacking" (empiler les sorts d'amelioration). Un mage ne peut maintenir qu'un seul sort de concentration a la fois.
- Les cantrips (sorts a volonte) ont paradoxalement aggrave le probleme : le mage n'a plus jamais de "mauvais tour" ou il est reduit a l'arbalete.
- Les "short rest vs long rest classes" creent un desequilibre selon le rythme de jeu du MJ.
- A partir du niveau 9-11, l'ecart redevient flagrant.

**Lecon a retenir** : Limiter le nombre de sorts actifs simultanement (concentration) est une excellente mecanique. Mais donner des sorts a volonte sans contrepartie erode le role des martiaux.

#### Burning Wheel : Magie couteuse et risquee

Dans Burning Wheel, la magie est puissante mais extremement couteuse :
- Chaque sort requiert un test de competence qui prend du temps (plusieurs actions en combat).
- L'echec a des consequences narratives reelles.
- Le mage doit sacrifier des points de stat (Forte, la stat physique) pour alimenter sa magie, le rendant physiquement faible.
- Le systeme de progression ("Artha") recompense les joueurs qui jouent les croyances de leur personnage, pas ceux qui optimisent mecaniquement.

**Lecon a retenir** : Quand la magie coute quelque chose de tangible et d'irreversible (pas juste un "slot" qui revient apres une nuit de sommeil), elle s'equilibre naturellement. Le mage de Burning Wheel est puissant mais paye le prix.

#### Dungeon World : Equilibre narratif

Dungeon World (Powered by the Apocalypse) utilise une approche radicalement differente :
- Tous les personnages ont des "moves" (actions speciales) de puissance comparable.
- Le move "Cast a Spell" du Wizard sur un 7-9 force un choix : le sort attire l'attention, le sort est oublie, le sort coute de la fatigue.
- La fiction (narration) est le principal limiteur : le MJ fait des "moves" en retour.
- Pas de scaling vertical — le jeu est concu pour des campagnes courtes/moyennes.

**Lecon a retenir** : Un systeme ou la magie implique toujours un choix difficile (meme en cas de reussite partielle) cree une tension narrative qui est a la fois equilibree et engageante. Le "succes a un cout" est un outil de design puissant.

#### Shadow of the Demon Lord : Progression contrainte

Shadow of the Demon Lord offre un design elegant :
- Tout le monde peut prendre des traditions magiques, mais cela a un cout d'opportunite (on ne prend pas les talents martiaux).
- Les sorts sont divises en traditions avec des niches claires.
- Les martiaux obtiennent des capacites quasi-surnaturelles a haut niveau (un berserker peut litteralement fendre la terre).
- La progression est fixe et courte (10 niveaux), evitant la derive du scaling infini.

**Lecon a retenir** : Permettre aux martiaux d'atteindre des exploits quasi-mythiques a haut niveau est une approche saine. Si seuls les mages peuvent "casser" la realite, les martiaux seront toujours en retard.

#### Symbaroum : La corruption comme prix

Symbaroum est l'un des meilleurs exemples de magie equilibree par le risque :
- Chaque sort genere de la Corruption (temporaire ou permanente).
- La Corruption permanente transforme le personnage en monstre. A un certain seuil, le personnage devient un PNJ.
- Les mages sont dans une course contre la montre contre leur propre pouvoir.
- Les traditions magiques (Theurgie, Sorcellerie, etc.) offrent des voies pour reduire la corruption mais avec des contraintes narratives.
- Les guerriers ne subissent pas de corruption, leur stabilite est une force en soi.

**Lecon a retenir** : La corruption est un mecanisme de feedback negatif brillant. Plus on utilise la magie, plus le risque augmente. Le mage se retrouve a devoir gerer une ressource qui ne se regenere pas simplement, et qui menace son existence meme.

#### Warhammer Fantasy Roleplay (WFRP) : Magie dangereuse

WFRP (surtout la 2e edition) rend la magie terrifiante :
- Les jets de magie utilisent des des speciaux ("Chaos dice").
- Les doubles et triples sur ces des declenchent des "misfires" dont les effets vont du desagreable (perte de cheveux) au catastrophique (portail demoniaque).
- Les mages sont surveilles par des chasseurs de sorcieres (consequence sociale).
- Les sorts mineurs sont relativement surs, les sorts majeurs sont une roulette russe.

**Lecon a retenir** : La gradation du risque est cle. Les petits sorts sont accessibles, les grands sorts sont terrifiants. Cela cree une courbe d'utilisation ou le joueur doit peser le risque a chaque utilisation puissante.

#### The One Ring / L'Anneau Unique : Fatigue et Ombre

The One Ring utilise un double systeme elegant :
- La magie (limitee, coherente avec le cadre tolkienien) coute de la Fatigue, la meme ressource que les voyages et les efforts physiques.
- Certains pouvoirs attirent l'Ombre (corruption), creant un deuxieme axe de cout.
- Les personnages non-magiques ont des capacites de combat et de voyage tout aussi impactantes.

**Lecon a retenir** : Quand la magie consomme la meme ressource que les actions physiques (fatigue, endurance), elle entre en competition directe avec la survie. Le mage qui se vide pour lancer des sorts est aussi vulnerable que le guerrier qui s'epuise au combat.

#### GURPS : Flexibilite et couts multiples

GURPS offre plusieurs systemes de magie optionnels, dont le systeme de base en fatigue :
- Chaque sort coute des points de fatigue (les memes que pour les actions physiques).
- Les sorts puissants ont des prerequis (il faut connaitre 5 sorts de feu avant de lancer Boule de Feu).
- Le systeme de points de personnage rend la magie couteuse a l'achat : un mage puissant a investi enormement de points, un guerrier polyvalent a pu diversifier.
- Les extensions "Thaumatology" offrent des variantes (magie rituelle, a composantes, etc.).

**Lecon a retenir** : Le systeme de prerequis cree un investissement progressif qui empeche le "cherry-picking" des sorts les plus puissants. L'arbre de prerequis est une forme de gating elegante.

### 1.3. Synthese du probleme

| Approche | Forces | Faiblesses |
|---|---|---|
| Slots/Vancien (D&D) | Simple, previsible | Le repos annule le cout ; scaling vertical |
| Corruption (Symbaroum, WFRP) | Tension dramatique, cout permanent | Peut decourager l'utilisation de la magie |
| Fatigue partagee (TOR, GURPS) | Equilibre naturel avec les martiaux | Peut sembler "generique" |
| Narratif (Dungeon World) | Flexible, toujours interessant | Depend fortement du MJ |
| Cout d'opportunite (SotDL) | Equilibre structural | Moins de "wow factor" pour la magie |
| Risque d'echec (Burning Wheel) | Tension a chaque jet | Peut frustrer les joueurs de mages |

---

## 2. Archetypes de systemes de magie

### 2.1. Magie Vancienne (spell slots)

**Principe** : Le mage memorise un nombre fixe de sorts par jour, qu'il "depense" en les lancant. Inspire des romans de Jack Vance (La Terre Mourante).

**Exemples** : D&D (toutes editions), Pathfinder.

**Avantages** :
- Facile a equilibrer numeriquement (le MJ sait exactement combien de sorts un mage a).
- Force la gestion de ressources et la planification.
- Cree des moments "clutch" ou le dernier sort compte.

**Inconvenients** :
- Le mage qui n'a plus de sorts est souvent inutile ("le mage sac a dos de l'aventure du matin").
- La gestion de liste de sorts peut etre lourde.
- Le repos long annule tout le cout — le rythme de jeu du MJ determine l'equilibre plus que les regles.
- Peu intuitif narrativement ("pourquoi j'oublie le sort que je viens de lancer ?").

**Verdict** : Systeme classique mais vieillissant. Fonctionne mieux avec des contraintes de repos strictes.

### 2.2. Points de mana / Points de pouvoir

**Principe** : Le mage a une reserve de points qu'il depense pour lancer des sorts. Les sorts coutent plus ou moins cher selon leur puissance.

**Exemples** : Shadowrun (drain), GURPS (fatigue comme mana), Savage Worlds (Power Points), de nombreux jeux video.

**Avantages** :
- Plus flexible que le Vancien : le mage choisit comment repartir ses ressources.
- Intuitif (tout le monde comprend "j'ai 20 points, ce sort coute 5").
- Permet du scaling fin (un sort peut couter 3, 5 ou 8 points).

**Inconvenients** :
- Tend vers l'optimisation mathematique ("quel sort a le meilleur ratio cout/effet ?").
- Sans contraintes supplementaires, le mage peut spammer le sort le plus efficace.
- La regeneration de mana doit etre soigneusement calibree.

**Variantes notables** :
- **Mana avec cout croissant** : Chaque sort supplementaire du meme type coute plus cher dans la meme scene (anti-spam).
- **Mana liee a une stat** : Les points de pouvoir sont derives d'un attribut, creant un lien stat-magie.
- **Drain** (Shadowrun) : Lancer un sort cause du drain (degats) au mage, basculant vers un modele de risque.

**Verdict** : Flexible et intuitif, mais necessite des garde-fous contre l'optimisation excessive.

### 2.3. Magie basee sur les competences (roll to cast)

**Principe** : Lancer un sort est un jet de competence comme un autre. On peut echouer, reussir partiellement, ou reussir brillamment.

**Exemples** : Ars Magica, Burning Wheel, Runequest, Mage: The Ascension, le Year Zero Engine (Forbidden Lands).

**Avantages** :
- Unifie la magie avec le reste du systeme de jeu (meme mecanique de base).
- L'echec cree de la tension et de la narration.
- Permet des degrees de reussite (plus de succes = effet plus puissant).
- Naturellement compatible avec le YZE (pool de d6, compter les 6).

**Inconvenients** :
- Si le jet est sans consequence en cas d'echec, on relance simplement — pas de vrai cout.
- Il faut definir ce qui se passe en cas d'echec critique.
- Risque de "whiff factor" : le mage rate son sort, perd son tour, ne se passe rien d'interessant.

**Variantes notables** :
- **Ars Magica** : Le systeme Verbe + Nom (Creo Ignem = Creer + Feu) est d'une elegance remarquable. La difficulte vient de la combinaison choisie. C'est le systeme de magie libre le plus influence dans l'histoire du JDR.
- **Mage: The Ascension** : Les Spheres definissent ce que le mage peut affecter (Forces, Life, Mind...). La difficulte depend de l'ecart avec la realite consensuelle. Paradigme du personnage = limitation narrative.

**Verdict** : Excellent pour le YZE car coherent avec la mecanique de base. Doit etre combine avec un cout (fatigue, corruption, etc.) pour eviter le spam.

### 2.4. Systemes de corruption / backlash

**Principe** : La magie est inherement dangereuse. Chaque utilisation risque d'alterer le mage ou le monde autour de lui.

**Exemples** : Symbaroum, Warhammer FRP, Zweihander, Dark Heresy, Dungeon Crawl Classics (DCC).

**Avantages** :
- Cree un ton specifique : la magie est quelque chose qu'on craint et respecte.
- Auto-equilibrant : plus on utilise la magie, plus les consequences s'accumulent.
- Genere des histoires emergentes (le mage qui sombre, la quete pour purifier sa corruption).
- Chaque lancer de sort est un moment de tension.

**Inconvenients** :
- Peut decourager completement l'utilisation de la magie si le risque est trop punitif.
- L'accumulation de malus permanents peut rendre le personnage injouable avant la fin de la campagne.
- Necessite des tables de corruption/backlash bien concues (assez variees pour ne pas lasser, assez coherentes pour le ton).

**Exemples detailles de backlash** :
- **DCC** : Chaque sort a sa propre table de resultats (du fiasco a l'effet divin). Les echecs critiques provoquent de la "corruption" physique (mutation, etc.). C'est chaotique, fun, et totalement imprevisible.
- **Warhammer** : La table des Tzeentch's Curse va du benin (nez qui saigne) au catastrophique (apparition d'un demon). La gradation cree une escalade narrative.

**Verdict** : Ideal pour un setting dark/gritty. Compatible avec le YZE si la corruption est liee aux 1 sur les des de base ou de stress.

### 2.5. Systemes bases sur la fatigue

**Principe** : La magie epuise physiquement ou mentalement le lanceur. La fatigue est souvent la meme ressource que pour les efforts physiques.

**Exemples** : The One Ring, GURPS, The Witcher TRPG, certaines variantes de Savage Worlds.

**Avantages** :
- Tres intuitif ("lancer un sort, c'est epuisant").
- Cree un equilibre naturel avec les martiaux (meme pool de ressources).
- Le mage epuise est vulnerable — cela cree des dynamiques de protection.
- Encourage la cooperation (le groupe doit proteger le mage apres un gros sort).

**Inconvenients** :
- Peut encourager le "nova" (tout depenser d'un coup, puis se reposer).
- La fatigue qui se recupere facilement annule le cout.
- Peut sembler mundane ("la magie, c'est juste fatiguant").

**Lien avec le YZE** : Le YZE a deja des mecaniques de jauges (Sante, Resolution). Lier la magie a la Resolution (stress mental) est une piste naturelle et coherente.

**Verdict** : Excellent point de depart pour le YZE. Simple, equilibre, coherent avec le systeme existant.

### 2.6. Magie libre / narrative (freeform)

**Principe** : Pas de liste de sorts fixes. Le mage decrit ce qu'il veut accomplir, et le systeme determine la difficulte et le cout.

**Exemples** : Ars Magica, Mage: The Ascension/Awakening, Barbarians of Lemuria, Whitehack, Maze Rats (tables de generation aleatoire).

**Avantages** :
- Creativite maximale pour les joueurs.
- Pas de "liste de courses" de sorts a gerer.
- Chaque utilisation est unique et memorable.
- Encourage la reflexion et la resolution creative de problemes.

**Inconvenients** :
- Tres difficile a equilibrer (le joueur creatif trouvera toujours un angle brise).
- Depend enormement de l'arbitrage du MJ — source de conflits potentiels.
- Peut paralyser les joueurs qui preferent des options definies.
- Le "scope" de la magie doit etre clairement delimite ou le systeme explose.

**Approche hybride recommandee** :
Beaucoup de jeux modernes combinent sort fixes + improvisation :
- **Sorts connus** : Le mage a une liste de sorts definis avec des effets precis.
- **Improvisation** : Le mage peut tenter un effet hors-liste, mais a un cout/difficulte majore.
- **Rituels** : Les effets puissants et libres sont reserves a des rituels longs et couteux.

**Verdict** : La magie libre pure est difficile a gerer. Un systeme hybride (sorts definis + improvisation penalisee + rituels libres) offre le meilleur des deux mondes.

---

## 3. Principes de design pour l'equilibre

### 3.1. Des couts de ressources qui comptent

**Principe** : Le prix de la magie doit etre reel et tangible, pas juste comptable.

**Mauvais exemple** : Les spell slots de D&D 5e dans un jeu avec un seul combat par long rest. Le mage depense tout, dort, recommence. Le "cout" est illusoire.

**Bons exemples** :
- **Couts permanents** : La corruption de Symbaroum ne disparait pas. Chaque sort laisse une marque.
- **Couts en actions** : Dans Burning Wheel, lancer un sort prend plusieurs tours de combat. Pendant ce temps, le mage est vulnerable.
- **Couts partages** : La magie coute de la Resolution (stress mental) dans un systeme ou cette meme jauge protege contre la folie et la terreur.
- **Couts narratifs** : Le sort fonctionne, mais il attire l'attention des ennemis, ou il revele la position du mage.

**Regle de design** : Un cout qui se regenere completement apres un repos n'est pas un vrai cout — c'est un budget quotidien. Les meilleurs systemes combinent des couts a court terme (fatigue/mana qui se regenere) et des couts a long terme (corruption, consequences narratives).

### 3.2. Le cout d'opportunite : que sacrifie-t-on pour etre mage ?

**Principe** : Etre mage doit impliquer des renoncements significatifs.

**Axes de cout d'opportunite** :

1. **Cout en points de creation** : Si la magie coute des points de competence/talent, le mage est moins bon dans d'autres domaines. C'est le cas dans Forbidden Lands (YZE) ou investir dans les talents magiques signifie ne pas investir dans les talents de combat.

2. **Cout en equipement** : Certains jeux interdisent aux mages de porter une armure ou de manier certaines armes. D&D le faisait historiquement, mais l'a assoupli. L'idee reste valable : si le mage ne peut pas se proteger physiquement, le guerrier a un role clair de "bouclier".

3. **Cout en attributs** : Si la magie depend d'un attribut mental (Esprit), investir dedans signifie moins de Force ou d'Agilite. Le mage est naturellement plus fragile physiquement.

4. **Cout social/narratif** : Dans certains settings, les mages sont persecutes, crains, ou lies a des ordres stricts. Etre mage limite les interactions sociales ou impose des obligations.

5. **Cout en action economique** : Si le mage doit passer du temps a etudier, mediter, ou preparer ses sorts, il ne peut pas faire d'autres activites entre les aventures. Ars Magica excelle ici avec son systeme saisonnier.

**Regle de design** : Le meilleur cout d'opportunite est celui qui est inherent a la creation du personnage et qui ne peut pas etre contourne en jeu. "Tu as investi tes points dans la magie, donc tu es mediocre en combat rapproche" est plus sain que "tu ne peux pas porter d'armure parce que les regles le disent".

### 3.3. Risque et recompense

**Principe** : La magie devrait impliquer un risque proportionnel a sa puissance.

**Modele a trois paliers** :
- **Magie mineure** : Peu de risque, effets modestes. Le mage peut les utiliser librement. Equivalent des attaques de base du guerrier.
- **Magie standard** : Cout significatif (fatigue, mana, stress), risque modere d'echec ou de complication. Equivalent des manoeuvres speciales du guerrier.
- **Magie majeure** : Cout eleve, risque de backlash/corruption, effet potentiellement transformateur. Equivalent des exploits heroiques du guerrier... mais en plus spectaculaire, compense par le danger.

**Le "pushing" du YZE comme modele** : Le YZE a deja une mecanique de risque/recompense brillante — le "push" (relancer les des non-6, mais les 1 causent des degats/stress). Appliquer ce principe a la magie est une piste naturelle :
- Le mage lance son pool de des.
- Il peut "pousser" le sort (relancer) mais subit des consequences sur les 1.
- Pour la magie, les consequences des 1 pourraient etre de la corruption ou du backlash plutot que du stress ordinaire.

### 3.4. Protection de niche

**Principe** : Chaque archetype doit avoir des domaines ou il excelle et que les autres ne peuvent pas facilement envahir.

**Exemples de niches a proteger** :

| Archetype | Niche exclusive |
|---|---|
| Guerrier | Domination au corps a corps, encaissement de degats, controle de la zone |
| Rodeur/eclaireur | Exploration, pistage, survie, premiere frappe |
| Voleur/roublard | Infiltration, pieges, information, coups critiques |
| Mage | Effets surnaturels, connaissance arcane, rituals puissants |
| Pretre/soigneur | Guerison, protection, bannissement de l'horreur |

**Erreurs classiques** :
- Le mage qui soigne aussi bien que le pretre (pourquoi jouer pretre ?).
- Le mage qui fait plus de degats en melee que le guerrier grace a des buffs magiques.
- Le mage qui est meilleur en infiltration grace a l'invisibilite.

**Solutions** :
- **Superiorite locale** : Le guerrier est TOUJOURS meilleur en combat direct, meme contre un mage buffe. La magie offre de la versatilite, pas de la superiorite dans chaque domaine.
- **Limites de la magie** : La magie ne peut pas tout faire. Definir clairement ce que la magie ne peut PAS accomplir est aussi important que definir ce qu'elle peut faire.
- **Synergie** : Les meilleurs sorts sont ceux qui amplifient les capacites des allies plutot que de les remplacer. Un sort qui donne +2 aux attaques du guerrier renforce le groupe sans ecraser la niche du guerrier.

### 3.5. Le probleme du scaling

**Principe** : La magie ne doit pas devenir exponentiellement plus puissante que les capacites martiales a mesure que les personnages progressent.

**Strategies anti-scaling** :

1. **Plafond de progression bas** : Limiter la campagne a un petit nombre de niveaux (Shadow of the Demon Lord : 10 niveaux ; Forbidden Lands : pas de niveaux, progression par XP depenses).

2. **Scaling lateral plutot que vertical** : Les mages gagnent plus de sorts (versatilite) mais pas des sorts drastiquement plus puissants. Comme un artisan qui apprend plus de techniques plutot que de devenir surhumain.

3. **Scaling parallele des martiaux** : Si les mages deviennent mythiques, les guerriers aussi. A haut niveau, un guerrier peut fendre un rocher, un mage peut invoquer la foudre. Les deux sont impressionnants.

4. **Cout qui scale aussi** : Si les sorts puissants coutent proportionnellement plus cher (corruption exponentielle, fatigue massive), le scaling s'auto-limite.

5. **Pas de "sorts de niveau 9"** : Eviter completement les sorts qui reecrivent la realite (Wish, Time Stop, Gate). Si la magie la plus puissante est equivalente a "invoquer un eclair devastateur", l'ecart avec "un guerrier qui coupe trois ennemis en un seul coup" reste gerable.

---

## 4. Ce qui rend la magie FUN

L'equilibre est necessaire, mais insuffisant. Un systeme de magie parfaitement equilibre mais ennuyeux est un echec de design. Voici ce qui rend la magie engageante :

### 4.1. Le choix significatif

La magie est fun quand chaque utilisation implique un choix interessant :
- **Quel sort utiliser ?** (plusieurs options, chacune avec des compromis)
- **Quand l'utiliser ?** (gestion de ressources : maintenant ou garder pour plus tard ?)
- **A quel prix ?** (accepter la corruption ? pousser le sort ? risquer le backlash ?)
- **Pour quel effet ?** (dans un systeme libre ou a degres de reussite)

**Anti-pattern** : Le mage qui lance le meme sort chaque tour (Eldritch Blast en D&D 5e). Pas de choix = pas de fun.

### 4.2. L'expression creative

Les joueurs de mages veulent se sentir malins et creatifs :
- Combiner des sorts de maniere inattendue.
- Utiliser un sort de maniere detournee ("je lance Graisse sur le sol sous le geant").
- Resoudre des problemes que le combat ne peut pas resoudre.
- Sentir que leur intelligence de joueur se traduit en puissance du personnage.

**Implication de design** : Un systeme avec un minimum de flexibilite (sorts avec des applications multiples, ou un composant freeform) sera plus satisfaisant qu'une liste rigide d'effets numeriques.

### 4.3. La sensation de puissance calibree

La magie doit donner la sensation d'etre speciale et puissante :
- Les effets magiques doivent etre visuellement/narrativement impressionnants.
- Le mage doit avoir des moments "spotlight" ou sa magie resout un probleme majeur.
- Mais ces moments doivent etre espaces et merites, pas routiniers.

**L'analogie du dessert** : Si on mange du gateau a chaque repas, il cesse d'etre special. Les gros sorts doivent etre rares et significatifs. Les sorts mineurs gèrent le quotidien.

### 4.4. La tension et le risque

Paradoxalement, la possibilite d'echec ou de backlash rend la magie PLUS fun, pas moins :
- Le frisson du "est-ce que ca va marcher ?" est addictif.
- Les echecs spectaculaires creent des histoires memorables.
- Gerer le risque est un jeu dans le jeu.
- Le sentiment d'avoir "ose" un sort dangereux et reussi est extremement satisfaisant.

**Exemple DCC** : Les joueurs de Dungeon Crawl Classics adorent les tables de corruption et de backlash parce que chaque sort est un evenement. Meme les echecs sont spectaculaires et memorables.

### 4.5. La progression ressentie

Le joueur doit sentir que son mage evolue et que de nouvelles possibilites s'ouvrent :
- Apprendre un nouveau sort doit etre un evenement marque.
- Debloquer une nouvelle "ecole" ou "tradition" est une recompense narrative.
- La progression ne doit pas etre seulement numerique (+1 au jet) mais qualitative (acces a de nouveaux types d'effets).

### 4.6. L'identite magique

Chaque mage doit se sentir unique :
- Les traditions/ecoles de magie permettent la specialisation.
- Le choix de sorts definit un style de jeu.
- L'esthetique de la magie (composantes verbales, gestuelles, focaliseurs) personalise le personnage.
- Le background du mage influence sa pratique magique (un mage autodidacte ne lance pas ses sorts comme un mage academique).

---

## 5. La magie dans le Year Zero Engine

### 5.1. Forbidden Lands : Le modele de reference

Forbidden Lands est le jeu YZE avec le systeme de magie le plus developpe :

**Mecaniques** :
- La magie est une competence (basee sur Esprit).
- Lancer un sort = jet de pool de d6 (Esprit + competence Magie).
- Chaque sort a un niveau de puissance, le mage doit obtenir un nombre de succes egal ou superieur.
- Le mage peut "pousser" le jet (relancer les des non-6), mais chaque 1 sur un de de base cause un point de dommage a l'attribut Esprit.
- Pousser un sort est donc dangereux : on risque de se vider mentalement.
- Les sorts sont organises en "ecoles" (chemins du sang, de la mort, etc.).
- Certains sorts coutent des Points de Volonte (une ressource limitee).

**Forces du modele Forbidden Lands** :
- Coherent avec le YZE de base (meme mecanique de jet).
- Le "push" est le principal mecanisme de risque — elegant et deja compris des joueurs.
- Les degats a l'attribut sont un cout tangible (Esprit reduit = moins de des pour TOUT ce qui utilise Esprit).
- Les Points de Volonte comme seconde ressource ajoutent de la profondeur.

**Faiblesses** :
- Le systeme est relativement simple — peu de marge pour la magie libre ou l'improvisation.
- Le scaling est limite (peu de sorts de haut niveau vraiment transformateurs).
- La corruption est peu presente (c'est un choix de ton, pas un defaut en soi).

### 5.2. Autres implementations YZE

- **Vaesen** : La magie est quasi-absente pour les PJ (coherent avec le setting). Les rituels sont rares, longs, et dangereux. L'accent est sur l'enquete.
- **Alien RPG** : Pas de magie, mais le systeme de stress est un modele de mecanique de "pression croissante" applicable a la magie.
- **Twilight 2000 (4e ed)** : Pas de magie, mais les mecaniques de fatigue et de stress montrent comment le YZE gere l'epuisement des ressources.
- **The Bitter Reach (extension Forbidden Lands)** : Ajoute de nouveaux sorts et la magie demoniaque, avec des couts plus eleves.

### 5.3. Compatibilite avec le systeme en cours de conception

En se referant au systeme defini dans `resume.md`, voici les points d'ancrage naturels pour la magie :

**Attribut de reference** : Esprit (logique pour la magie intellectuelle) ou Empathie (pour une magie plus intuitive/spirituelle). Possible d'avoir deux traditions avec des attributs differents.

**Competence** : Ajouter une competence "Magie" (ou "Arcanes", "Sorcellerie" — selon le ton) liee a Esprit. Ou plusieurs competences magiques specialisees.

**Jauge de cout** : La Resolution (Esprit + Empathie) est la candidate naturelle comme "reservoir" pour la magie. Le mage depense de la Resolution pour lancer des sorts, la meme jauge qui le protege du stress mental. C'est un cout reel : un mage qui a beaucoup lance de sorts est plus vulnerable psychologiquement.

**Stress en magie** : Le systeme de combat utilise deja le stress comme amplificateur risque (des de stress ou un 1 = echec automatique). On pourrait creer un "stress magique" equivalent qui s'ajoute au pool mais dont les 1 causent de la corruption/du backlash.

**Push** : Le push est le mecanisme central du risque. Pousser un sort devrait avoir des consequences specifiques a la magie (corruption, backlash), pas juste des degats d'attribut comme en Forbidden Lands.

---

## 6. Synthese et recommandations

### 6.1. Principes directeurs pour le systeme

En combinant les lecons des differents jeux et la structure YZE existante, voici les principes recommandes :

1. **Coherence mecanique** : La magie doit utiliser le meme systeme de base (pool de d6, compter les 6) que le combat et les autres actions. Pas de sous-systeme parallele.

2. **Triple cout** :
   - **Cout immediat** : Resolution depensee (fatigue mentale), s'applique a chaque sort.
   - **Cout de risque** : Le push et/ou les des de stress magique generent des complications (corruption, backlash).
   - **Cout d'opportunite** : Investir dans la magie signifie ne pas investir dans le combat ou les competences sociales.

3. **Gradation du risque** : Les sorts mineurs sont relativement surs. Les sorts majeurs sont dangereux. Les rituels sont terrifiants mais puissants.

4. **Protection des niches** :
   - Le guerrier domine le combat direct — aucun sort ne devrait surpasser un guerrier optimise en melee.
   - Le mage excelle dans la versatilite, la connaissance, et les effets surnaturels impossibles autrement.
   - Les sorts de soutien (buffs, soins) renforcent le groupe plutot que de remplacer les specialistes.

5. **Scaling controle** : Pas de sorts de type "Wish". La magie la plus puissante est comparable a un phenomene naturel extreme (eclair, tremblement de terre localize), pas a la recriture de la realite.

6. **La magie est speciale** : Chaque utilisation doit etre un evenement, pas une routine. Le mage ne "spam" pas — il choisit ses moments.

### 6.2. Pistes de mecaniques concretes

**Piste A : Magie par Resolution + Corruption**
- Lancer un sort = jet Esprit + Competence Magique.
- Le sort coute X points de Resolution (selon puissance).
- Le mage peut "pousser" le sort : relance les des, mais les 1 generent de la Corruption.
- La Corruption est une jauge separee avec des paliers d'effets negatifs.
- A 0 Resolution, le mage est "brise" mentalement (comme les PV a 0).

**Piste B : Des de magie (variante du stress)**
- Lancer un sort = Esprit + Competence Magique + des de Magie (d'une couleur specifique).
- Les des de Magie fonctionnent comme les des de Stress : les 1 causent un backlash.
- Le nombre de des de Magie ajoutes depend de la puissance du sort voulu.
- Plus le sort est puissant, plus on ajoute de des de Magie, plus le risque de backlash est eleve.
- Cree une tension delicieuse : plus de des = plus de chances de reussir ET plus de chances de backlash.

**Piste C : Systeme hybride**
- Sorts mineurs : jet simple, cout en Resolution modeste, pas de risque.
- Sorts standards : jet + cout en Resolution + possibilite de push avec corruption.
- Rituels : freeform, cout eleve, temps long, plusieurs participants possibles, table de backlash dediee.

### 6.3. Erreurs a eviter

1. **La magie gratuite** : Si un mage peut lancer des sorts a volonte sans aucun cout, il n'y a aucune raison de ne pas etre mage.

2. **La magie trop punitive** : Si chaque sort risque de tuer le personnage, personne ne jouera mage. Le plaisir vient du risque gerable, pas de la punition.

3. **Le "mage inutile"** : Entre deux gros sorts, le mage doit pouvoir contribuer. Des cantrips/sorts mineurs ou des competences non-magiques utiles sont necessaires.

4. **Le mage-guerrier** : Si un personnage peut etre a la fois un bon mage et un bon guerrier, le guerrier pur n'a aucune raison d'exister. Le multiclassage magique doit avoir un cout d'opportunite reel.

5. **L'inflation magique** : Si tout le monde a acces a la magie, elle cesse d'etre speciale. Dans un setting ou la magie est rare, la limiter a certains archetypes renforce son impact narratif.

6. **Les sorts qui annulent le jeu** : Eviter les sorts qui rendent des pans entiers du jeu irrelevants (teleportation qui annule l'exploration, detection qui annule l'enquete, guerison infinie qui annule le danger).

### 6.4. Questions ouvertes pour la conception

- **Qui peut faire de la magie ?** Tous les archetypes ou seulement certains ? Un guerrier peut-il apprendre un sort mineur ?
- **Combien de traditions/ecoles ?** Trop peu = tous les mages se ressemblent. Trop = complexite excessive.
- **Quelle place pour les rituels ?** Un systeme de rituels (longs, couteux, cooperatifs) peut offrir la magie "libre" sans desequilibrer le jeu.
- **La magie et le worldbuilding** : D'ou vient la magie ? Comment est-elle percue socialement ? Ces choix de setting influencent le design mecanique.
- **La magie divine vs arcane ?** Un seul systeme unifie ou deux sous-systemes avec des couts differents ?

---

## Annexe : Sources et references cles

### Jeux analyses
- **D&D 5e** (Wizards of the Coast) — Systeme Vancien moderne, concentration
- **Burning Wheel** (Luke Crane) — Magie couteuse en stats, echec significatif
- **Dungeon World** (Sage LaTorra, Adam Koebel) — Moves narratifs, 7-9 comme succes a un cout
- **Shadow of the Demon Lord** (Robert Schwalb) — Traditions, progression courte, martiaux mythiques
- **Symbaroum** (Free League / Jarnringen) — Corruption permanente, tension croissante
- **Warhammer Fantasy Roleplay** (Cubicle 7) — Backlash aleatoire, magie comme roulette russe
- **The One Ring** (Free League) — Fatigue et Ombre, double cout
- **GURPS** (Steve Jackson Games) — Fatigue comme mana, prerequis de sorts
- **Ars Magica** (Atlas Games) — Verbe + Nom, magie libre structuree
- **Mage: The Ascension/Awakening** (White Wolf/Onyx Path) — Spheres, paradigme, Paradoxe
- **Dungeon Crawl Classics** (Goodman Games) — Tables de corruption, magie imprevisible et fun
- **Forbidden Lands** (Free League) — Magie YZE de reference, push, degats d'attribut
- **Savage Worlds** (Pinnacle) — Power Points, systeme generique equilibre

### Concepts de game design references
- "Linear Fighter, Quadratic Wizard" — analyse du scaling martial/caster
- "Niche protection" — chaque role doit avoir une zone d'excellence exclusive
- "Opportunity cost" — le choix de ce qu'on ne fait pas est aussi important que le choix de ce qu'on fait
- "Risk/reward curve" — la puissance doit etre proportionnelle au risque
- "Resource attrition" — l'erosion des ressources au fil de l'aventure comme source de tension
- "Spotlight sharing" — chaque joueur doit avoir ses moments de gloire
