# Portfolio — Bataya Crépin

Site en HTML/CSS pur (aucune dépendance à installer), prêt à déployer sur GitHub Pages.

## 1. Ajouter votre photo

- Prenez une photo où l'on voit **la tête** (portrait, cadrage serré, fond neutre de préférence).
- Renommez-la `photo.jpg` et placez-la dans le dossier `assets/`.
- La photo s'affiche automatiquement dans le rond en haut de page. Tant qu'il n'y a pas de photo, vos initiales **BC** s'affichent à la place.
- Si votre fichier n'est pas au format `.jpg`, changez l'extension dans `index.html`, ligne :
  `<img src="assets/photo.jpg" ...>`

## 2. Tester en local

Ouvrez simplement `index.html` dans votre navigateur.

## 3. Déployer sur GitHub Pages

1. Créez un dépôt GitHub, par exemple `portfolio`.
2. Mettez `index.html`, `style.css` et le dossier `assets/` (avec votre photo) à la racine du dépôt.
3. Dans le dépôt : **Settings → Pages**.
4. Sous **Build and deployment**, choisissez **Deploy from a branch**, branche `main`, dossier `/ (root)`.
5. Enregistrez. Votre site sera disponible après une minute ou deux à l'adresse :
   `https://crepinba.github.io/portfolio/`

## Contenu du site

- **Accueil** — nom, titre, photo, accès rapide au contact + téléchargement du CV
- **Profil** — résumé professionnel
- **Expérience** — Digital Hub Togo + stage entreprise locale
- **Projets professionnels** — BANDJELI (SaaS IA) + Gestion Électricité (Flutter) + EPHAB Togo (Laravel / Next.js)
- **Projets académiques** — 3 projets
- **Compétences techniques** — par catégorie
- **Formation** — Licence IFNTI + Baccalauréat
- **Contact** — formulaire interactif + email, téléphone, GitHub, téléchargement du CV

## Formulaire de contact

Pour recevoir directement les messages dans votre boîte mail sans backend :
1. Créez un compte gratuit sur [Formspree](https://formspree.io) ou [Web3Forms](https://web3forms.com).
2. Remplacez `https://formspree.io/f/placeholder` dans `index.html` par votre propre URL de formulaire Formspree.
3. Si l'URL contient `placeholder`, le formulaire redirige intelligemment vers votre application de messagerie par défaut avec les champs pré-remplis.

## Mode clair / sombre

Un bouton en haut à droite (icône soleil/lune) bascule entre les deux thèmes.
Le choix du visiteur est mémorisé (`localStorage`) ; par défaut, le site suit
la préférence système de l'appareil.

## Télécharger le CV

Le fichier `assets/CV-Bataya-Crepin.pdf` est votre CV actuel. Pour le mettre
à jour, remplacez ce fichier par une nouvelle version **en gardant exactement
le même nom**, `CV-Bataya-Crepin.pdf`.

## Animations

Les sections apparaissent en fondu au défilement et les éléments du hero
s'animent à l'ouverture de la page — une seule fois, sans clignotement,
et désactivées automatiquement si le visiteur a réduit les animations dans
les réglages de son système. Le contenu reste toujours lisible même si le
JavaScript est bloqué.

Pour modifier un texte, ouvrez `index.html` dans un éditeur de texte et cherchez le passage à changer. Les couleurs et la mise en page se règlent dans `style.css`.
