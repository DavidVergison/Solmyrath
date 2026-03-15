# Isekai YZE — Site & Conception

**Univers : Solmyrath**

Projet de JDR (Year Zero Engine, setting isekai/portails). Deux volets :
- `building/` : conception du jeu (règles, lore, kins, scénarios) — voir `building/CLAUDE.md` pour le détail
- Racine : site Hugo (thème hugo-book) pour exposer le contenu au public

## Structure

- `building/` : documents de conception (source de vérité)
- `content/` : articles Hugo générés à partir de `building/`
- `layouts/`, `assets/`, `static/` : templates et ressources Hugo
- `hugo.toml` : configuration du site
- `themes/hugo-book/` : thème Hugo Book (copié, pas un submodule)

## Workflow

- Les articles dans `content/` sont rédigés à partir des documents de `building/`
- Toujours lire le document source dans `building/` avant de créer un article
- Ne jamais modifier `building/` quand on travaille sur le site, et inversement, sauf demande explicite
- Hugo : `hugo server` pour le dev, `hugo` pour le build

## Conventions

- Langue : français (contenu et communication)
- Format : markdown
- Lire les fichiers pertinents avant de créer du contenu
- Ne jamais contredire une décision déjà prise sans le signaler
