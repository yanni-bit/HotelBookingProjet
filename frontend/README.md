# README – Frontend du projet HotelBookingProjet

## Présentation

Ce dossier contient la partie frontend du projet **HotelBookingProjet**.
Il s'agit de l'interface utilisateur du site de réservation hôtelière, développée avec **HTML**, **CSS**, **JavaScript** et **Bootstrap** (dernière version stable).
Le frontend communique avec le backend Medusa via des appels API REST.

L’objectif de cette partie du projet est de fournir une interface claire, responsive et performante permettant aux utilisateurs de :

* consulter les chambres disponibles,
* effectuer une réservation,
* accéder à leurs informations de profil et leurs réservations passées.

---

## Structure du dossier

```
frontend/
├── public/              # Ressources statiques (images, favicon)
├── src/
│   ├── components/      # Composants réutilisables (cartes, formulaires, etc.)
│   ├── pages/           # Fichiers HTML ou JS spécifiques à chaque page
│   ├── scripts/         # Logique JavaScript du site
│   ├── services/        # Fonctions pour communiquer avec l'API backend
│   ├── styles/          # Feuilles de style CSS
│   ├── utils/           # Fonctions utilitaires
│   └── fonts/           # Polices personnalisées
├── index.html           # Page d’accueil du site
├── package.json         # Dépendances éventuelles (si build tool utilisé)
├── .gitignore
└── README.md
```

---

## Structure du dossier styles/

```
styles/
├── base.css         # Reset CSS, typographie, variables globales, boutons généraux
├── layout.css       # Structure globale (header, footer, conteneurs, grilles)
├── components.css   # Styles pour les composants réutilisables (cartes, formulaires...)
├── home.css         # Styles spécifiques à la page d’accueil
├── rooms.css        # Styles spécifiques à la page de liste ou détail des chambres
└── booking.css      # Styles spécifiques à la page de réservation
```

Chaque fichier CSS a un rôle défini afin de faciliter la maintenance et la clarté du projet.
Les fichiers spécifiques par page ne sont chargés que lorsque nécessaire.

---

## Structure du dossier scripts/

```
scripts/
├── main.js         # Point d’entrée global (initialisation générale, écouteurs communs)
├── utils.js        # Fonctions utilitaires partagées (formatage, validation, etc.)
├── home.js         # Logique spécifique à la page d’accueil
├── rooms.js        # Logique spécifique à la page chambres (affichage, filtres, etc.)
└── booking.js      # Gestion du processus de réservation (formulaire, validation, envoi)
```

Cette organisation permet de séparer les comportements par page ou fonctionnalité, tout en centralisant le code global dans `main.js`.

---

## Standards de développement

* Utilisation du **dernier Bootstrap stable** pour la grille et les composants UI.
* Styles écrits en **CSS standard (non SCSS)**, structurés par rôle et par page.
* Scripts écrits en **JavaScript ES6**, avec des **fonctions classiques** et non fléchées.
* Code organisé et commenté pour faciliter la maintenance et l’évolutivité.

---

## Objectif du frontend

L’objectif principal est de construire une base solide, claire et extensible
sur laquelle les futures fonctionnalités (authentification, panier de réservation, intégration API, etc.) viendront se greffer progressivement.
