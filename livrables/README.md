# livrables/

Ce dossier contient tous les livrables produits par Claude pour Franck (sites, applications, contenus, livrables clients/formation).

## La règle d'or

- **`context/import/`** = les inputs. Tout ce que Franck fournit à Claude (documents, exports, captures, notes) pour analyse ou contexte.
- **`livrables/`** = les outputs. Tout ce que Claude produit pour Franck (fichiers finaux, livrables de travail, drafts avancés).

Ne jamais mélanger les deux : un input ne va pas dans `livrables/`, un output ne va pas dans `context/import/`.

## Organisation

| Dossier | Contenu |
|---------|---------|
| `sites-web/` | Sites internet (vitrines clients, pages, assets associés) |
| `applications/` | Outils, scripts, automatisations |
| `youtube/` | Briefs vidéos, scripts, hooks, calendrier éditorial |
| `cabinet/` | Livrables pour le cabinet de conseil Chatflow |
| `ecole/` | Livrables pour Builderia |

## Convention de nommage des projets

Format : `AAAA-MM-JJ_nom-du-projet_nom-du-livrable.ext`

Exemples :
- `2026-08-30_plombier-dupont_site-vitrine-v1.html`
- `2026-09-05_chatflow_audit-ia-client-x.pdf`
- `2026-09-10_youtube_calendrier-editorial-septembre.md`

Si un projet génère plusieurs livrables liés, créer un sous-dossier au nom du projet (en kebab-case) dans le dossier thématique concerné, plutôt que d'entasser les fichiers en vrac.
