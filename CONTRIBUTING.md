# Contribuer au Café Associatif

Ce dépôt est développé en équipe. Avant de modifier un fichier, inspectez son contenu et l’état Git pour préserver le travail en cours des autres contributeurs.

## Organisation Git et workflow

Les branches partagées ont les rôles suivants :

- `dev` : branche de développement collaboratif ; les changements y sont développés directement.
- `preprod` : branche de validation avant production.
- `main` : branche de production, soumise à ses règles de protection.

Workflow obligatoire :

1. Développer directement sur `dev`. Ne pas créer de branche de fonctionnalité.
2. Examiner les changements et vérifier les fichiers concernés avant de les partager.
3. Créer des commits explicites, avec des messages clairs décrivant le changement.
4. Pousser les commits sur `dev`.
5. Créer une Pull Request de `dev` vers `preprod` pour promouvoir les changements en validation.
6. Après validation requise, créer une Pull Request de `preprod` vers `main`.

Ne pas contourner les protections de `main` et ne pas fusionner une Pull Request avant d’avoir reçu toutes les validations requises.

## Conventions de développement

- Écrire du HTML5 sémantique et conserver une hiérarchie de titres cohérente.
- Structurer les styles en CSS3 dans la feuille existante `styles/styles.css`.
- Respecter la charte graphique et réutiliser les variables et classes communes existantes.
- Préfixer ou autrement isoler les classes propres à une section ou une page afin de limiter les collisions CSS.
- Rendre chaque page utilisable sur ordinateur, tablette et mobile ; éviter les débordements horizontaux.
- Préserver l’accessibilité : textes alternatifs pertinents, navigation clavier, focus visible, contrastes lisibles et respect des préférences de réduction des animations.
- Ne pas supprimer, écraser ou remplacer le travail des autres collaborateurs. Vérifier l’historique et le diff en cas de conflit.
- Ne pas ajouter de JavaScript, framework ou dépendance sans décision collective préalable.
- Vérifier les liens, les chemins relatifs des ressources et les fichiers modifiés avant de proposer un changement.

## Pull Requests

Chaque Pull Request doit comporter :

- un titre descriptif ;
- une description concise du besoin et des modifications ;
- la liste ou une vérification claire des fichiers modifiés ;
- les contrôles effectués et les éventuels points restant à valider manuellement.

Pour promouvoir les changements, respecter le parcours `dev` vers `preprod`, puis `preprod` vers `main`. Suivre les protections de `main` et ne fusionner qu’après les validations requises.
