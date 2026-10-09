# Suivi des tickets : markdown local

Ce dépôt n'utilise pas les issues GitHub. Les cartes et tickets sont des fichiers markdown dans `wayfinder/`.

## Opérations Wayfinder

- **Carte** : `wayfinder/<nom-de-la-carte>/map.md`, étiquette `wayfinder:map` en tête de fichier.
- **Ticket** : `wayfinder/<nom-de-la-carte>/tickets/NN-<slug>.md`. Le titre (`# …`) est le nom du ticket.
- **En-tête d'un ticket** (lignes juste sous le titre) :
  - `Type :` `wayfinder:research` | `wayfinder:prototype` | `wayfinder:grilling` | `wayfinder:task`
  - `Statut :` `ouvert` | `fermé` | `hors périmètre`
  - `Assigné :` nom de la personne qui pilote la carte (vide = libre). Assigner un ticket = le prendre.
  - `Bloqué par :` liens vers les tickets bloquants (vide = débloqué).
- **Frontière** : les tickets `ouvert`, sans `Assigné`, dont tous les bloquants sont `fermé`.
- **Résolution** : ajouter une section `## Résolution` au ticket, passer `Statut : fermé`, puis ajouter une ligne dans « Décisions prises » de la carte.
- **Liens** : toujours par le nom du ticket, en lien markdown relatif.
