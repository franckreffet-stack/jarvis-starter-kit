# livrables/

Ce dossier contient tous les livrables produits par Claude pour Franck (sites, applications, contenus, livrables clients/formation).

## La règle d'or

- **`context/import/`** = les inputs. Tout ce que Franck fournit à Claude (documents, exports, captures, notes) pour analyse ou contexte.
- **`livrables/`** = les outputs. Tout ce que Claude produit pour Franck (fichiers finaux, livrables de travail, drafts avancés).

Ne jamais mélanger les deux : un input ne va pas dans `livrables/`, un output ne va pas dans `context/import/`.

## Organisation

Deux logiques de classement coexistent, et l'une prime sur l'autre :

1. **Par entité d'abord.** Si un livrable est produit pour Chatflow ou Builderia, il va dans `cabinet/` ou `ecole/`, quel que soit son type (site, appli, automatisation, contenu pédagogique...). Ces deux dossiers regroupent tout ce qui concerne cette entité, peu importe la thématique.
2. **Par thématique ensuite.** Pour tout le reste (autres clients, projets génériques, usage perso), on classe par type de livrable.

| Dossier | Contenu |
|---------|---------|
| `cabinet/` | Tout ce qui est produit pour le cabinet de conseil Chatflow, quel que soit le type de livrable |
| `ecole/` | Tout ce qui est produit pour Builderia, quel que soit le type de livrable |
| `sites-web/` | Sites internet pour d'autres clients (ex : vitrines d'artisans) |
| `applications/` | Outils, scripts, automatisations hors Chatflow/Builderia |
| `youtube/` | Briefs vidéos, scripts, hooks, calendrier éditorial |

Si `cabinet/` ou `ecole/` accumulent beaucoup de livrables de nature différente (site, appli, contenu pédagogique...), créer des sous-dossiers par type à l'intérieur (ex : `ecole/site-web/`, `ecole/automatisations/`) plutôt que de les redistribuer dans les dossiers thématiques.

## Convention de nommage des projets

Format : `AAAA-MM-JJ_nom-du-projet_nom-du-livrable.ext`

Exemples :
- `2026-08-30_plombier-dupont_site-vitrine-v1.html`
- `2026-09-05_chatflow_audit-ia-client-x.pdf`
- `2026-09-10_youtube_calendrier-editorial-septembre.md`

Si un projet génère plusieurs livrables liés, créer un sous-dossier au nom du projet (en kebab-case) dans le dossier thématique concerné, plutôt que d'entasser les fichiers en vrac.
