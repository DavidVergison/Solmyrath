# Isekai YZE — Systeme de JDR

Conception d'un systeme de regles et d'un univers de JDR base sur le **Year Zero Engine** (SRD libre de droits), avec un setting isekai/portails. Claude agit comme co-auteur et game designer.

## Fichiers du projet

- `lore/` : univers (genese, peuples)
- `systeme/` : regles du jeu (magie, sorts, competences, professions, equilibrage)
- `fiches/kins/` : fiches detaillees des Kins (lore + mecanique + prompts image)
- `scenario/` : scenarios de campagne
- `existing-rules/` : reference YZE SRD, Forbidden Lands, Symbaroum (talents .txt), PDFs exportables via `pdftotext`
- `comfyui-prompt-library-flux2klein.md` : bible visuelle et prompts image (Flux 2 Klein / Qwen3, langage naturel, pas de tags SDXL)
- Racine : drafts et documents de travail (`isekai-yze-kins-draft.md`, `ecoles.md`, `genese.md`, `resume.md`)

## Conventions

- Langue : francais
- Format : markdown
- Brainstorming iteratif : proposer des options, discuter, trancher
- Coherence mecanique avec le YZE — pas de sous-systeme parallele
- Lire les fichiers pertinents avant de creer du contenu
- Ne jamais contredire une decision deja prise sans le signaler explicitement
- Si une information n'existe pas encore, le signaler et proposer de l'ajouter
- Lors de la conception d'un peuple : conscience de l'heritage Visiteur ? statut social des mages ? magie non reconnue comme telle ?
- Prompts image : suivre `comfyui-prompt-library-flux2klein.md` — langage naturel, prompts complets et directement utilisables (pas d'instructions de remplacement)
- Prompts image — visages humains obligatoires : tous les personnages ont une figure humaine. Ne jamais decrire de fourrure, ecailles ou museau couvrant le visage. Les traits animaux (oreilles, queue, griffes, ecailles partielles) se limitent au corps.
- Prompts image — pas de label animal : ne jamais utiliser les mots "therian", "feline", "canine", "ursine", "lagomorph", "rapace", "reptilian" etc. dans un prompt. Decrire uniquement les traits concrets (oreilles de chat, queue de loup, plumage sur les bras, ecailles sur le cou).
- Prompts image — ordre (Flux poids les premiers tokens plus fort) : visage humain + traits distinctifs → style anchor → corps/equipement → pose → environnement → palette/mood

## Decisions cles (ne pas remettre en question)

### Systeme
- 4 Attributs : Force, Agilite, Esprit, Empathie
- Jauges : Sante (Force+Agilite), Resolution (Esprit+Empathie)
- Magie via competence Arcanes (liee a Esprit) + des de Resolution depenses
- 3 cercles de sorts (mineur/standard/majeur)
- Cantrips : categorie dediee, sans cout Resolution, pool Esprit+Arcanes
- Archetypes magiques vs non-magiques : acces different a Arcanes
- Structure personnage : Kin x Profession (a la Forbidden Lands)

### Lore
- Tous les peuples jouables sont arrives via des portails
- Les Elfes ont vole la magie aux autres — tous les peuples les detestent ; les Elfes sont PNJ uniquement
- Les Demi-Elfes sont bannis par les Elfes et ostracises par les autres
- Dryade et Elementaire de Terre sont PNJ uniquement
- Visiteur classique : arrive corps et ame, conserve ses souvenirs
- Visiteur-Joueur (PJ) : ame seule, dans le corps d'un natif dont l'ame a disparu via un rituel
- Les Visiteurs-Joueurs ne peuvent pas rentrer chez eux (revelation scenario 5-6, raisons a definir)
- Vulpin : heritage magique diffus dans toute l'espece (unions strategiques avec les Visiteurs)
- Genetique Therian : un parent Therian → enfant toujours Therian ; deux Therians → race de la mere
- Presentation des Kins : ne jamais expliquer l'origine des peuples par la "magie primordiale" ou la meteorite — formuler neutre ("natifs depuis les temps les plus recules", etc.)

## Questions ouvertes

### Mecaniques
- Effets mecaniques detailles des sorts
- Rituels : regles dediees ?
- Nombre max de sorts connus par personnage ?
- Sorts ameliorables vs remplaces par cercle superieur ?
- Traditions/sous-specialisations au sein des ecoles ?

### Lore / Kins
- Vulpin : sous-type Canin ou Kin a part entiere ?
- Reptilien : Kin unique ou sous-types separes ?
- Demi-Elfe : Kin autonome ou background ?
- Reversibilite du rituel elfique — factions a concevoir
