# /commit

> Commande pour créer un commit Git propre dans ce workspace.

---

## Mission

Quand je lance `/commit`, exécute la séquence suivante :

### Étape 1 : État des lieux

Lance en parallèle :
- `git status` pour voir les fichiers modifiés et non suivis
- `git diff` pour voir les changements non indexés
- `git diff --staged` pour voir ce qui est déjà indexé

### Étape 2 : Vérification de sécurité

Avant tout `git add`, vérifie qu'aucun fichier sensible ne risque d'être committé :
- Si `.env` ou une variante non listée dans `.gitignore` apparaît dans les fichiers non suivis ou modifiés, alerte-moi avant de continuer
- Si un fichier ajouté au staging contient une clé API, un token ou un secret visible dans le diff, alerte-moi avant de continuer

### Étape 3 : Sélection des fichiers

Par défaut, ajoute tous les fichiers modifiés et nouveaux pertinents (hors fichiers déjà exclus par `.gitignore`).

Si je précise une consigne (ex : "commit seulement livrables/"), respecte-la et n'ajoute que les fichiers concernés.

### Étape 4 : Message de commit

Analyse les changements et rédige un message de commit court et clair en français, qui explique le pourquoi plutôt que le quoi.

Présente-moi le message avant de committer :

```
Voici le commit que je m'apprête à faire :

[message proposé]

Fichiers concernés :
- [liste]

Tu valides ?
```

### Étape 5 : Créer le commit

Une fois validé :
1. `git add` des fichiers concernés
2. `git commit` avec le message validé
3. `git status` pour confirmer que tout est propre

### Étape 6 : Confirmer

```
Commit créé : [hash court] - [message]
```

---

## Règles importantes

- Ne jamais committer sans avoir présenté le message et reçu ma validation
- Ne jamais utiliser `git add -A` ou `git add .` à l'aveugle : vérifier ce qui est ajouté
- Ne jamais forcer un commit (`--no-verify`, `--amend` sur un commit déjà poussé) sauf demande explicite
- Ne jamais push automatiquement, `/commit` ne fait que committer en local
- Pas de tirets longs (em dashes) dans les écritures
- Communication en français systématique
