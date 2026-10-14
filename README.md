# Café Associatif

Site vitrine collaboratif du Café Associatif. Il présente le lieu, ses activités et son équipe, et oriente les visiteurs vers les pages de contact et d'information.

Le projet ne décrit pas d'adresse, d'horaires ni de coordonnées qui ne sont pas confirmés par l'association.

## Pages et fonctionnalités

- **Accueil** (`index.html`) : navigation commune, hero avec diaporama CSS, aperçu des activités, présentation de l'équipe et appel à contacter l'association.
- **Activités** (`Pages/activite.html`) : page consacrée aux activités.
- **Équipe** (`Pages/equipe.html`) : présentation du projet et des membres Dolvine, Yvan et Faou. Les portraits individuels restent des emplacements provisoires.
- **Contact** (`Pages/contact.html`) : page de contact de l'association.

Les quatre activités présentées sur l'accueil sont les Soirées jeux de société, le Repair Café, le Café-langues et la Scène ouverte.

## Technologies

- HTML5 sémantique.
- CSS3, dont Grid, Flexbox, media queries et animations CSS.
- Aucune bibliothèque ou dépendance de développement à installer. Les typographies Playfair Display et DM Sans sont chargées depuis Google Fonts ; leur chargement nécessite un accès réseau.

## Structure du dépôt

```text
cafe_associatif/
├── Assets/                 # Répertoire disponible pour de futures ressources locales
├── Pages/
│   ├── activite.html
│   ├── contact.html
│   └── equipe.html
├── styles/
│   └── styles.css          # Styles communs et styles des pages
├── index.html
├── README.md
└── CONTRIBUTING.md
```

## Installation et lancement

Cloner le dépôt :

```bash
git clone https://github.com/christian225-eng/cafe_associatif.git
cd cafe_associatif
```

Ouvrir `index.html` directement dans un navigateur, ou lancer un serveur local avec l’extension **Live Server** de Visual Studio Code : ouvrir `index.html`, puis choisir **Open with Live Server**. Il n’y a pas d’étape de compilation.

## Images et ressources externes

Certaines photographies sont chargées directement depuis le CDN Pixabay au moyen d’URL présentes dans les pages HTML ou dans `styles/styles.css`. Elles ne sont pas copiées dans le dépôt. La photo de la présentation de l’équipe est illustrative et ne représente pas les membres réels ; les portraits des membres ne sont pas fournis.

Avant d’ajouter ou de remplacer une image, vérifier la fiche Pixabay, l’URL directe et les conditions de la licence en vigueur. Ne pas attribuer une photographie illustrative aux membres de l’association. Le répertoire `Assets/` peut accueillir des ressources locales ultérieurement, si l’équipe décide de les ajouter.

## Branches Git

- `dev` : développement collaboratif.
- `preprod` : validation des changements proposés.
- `main` : version de production.

Le workflow de contribution et de promotion est décrit dans [CONTRIBUTING.md](CONTRIBUTING.md).
