hotel-booking/
├── backend/
│   ├── src/
│   │   ├── api/                     ← routes / endpoints personnalisés (REST)  
│   │   │   ├── rooms/              
│   │   │   │   └── route.ts         
│   │   │   └── bookings/
│   │   │       └── route.ts
│   │   ├── modules/                 ← mes modules personnalisés ou extensions
│   │   │   ├── rooms/
│   │   │   │   ├── service.ts
│   │   │   │   ├── models/
│   │   │   │   ├── migrations/
│   │   │   │   └── index.ts         ← export du module  
│   │   │   └── bookings/
│   │   │       ├── service.ts
│   │   │       ├── models/
│   │   │       ├── migrations/
│   │   │       └── index.ts
│   │   ├── loaders/                 ← scripts à exécuter au démarrage (ex : seed, initialisation)  
│   │   ├── subscribers/             ← “écouteurs” d’événements Medusa (ex : après création réservation)  
│   │   ├── migrations/              ← migrations générales  
│   │   ├── models/                   ← entités / schémas personnalisés  
│   │   ├── repositories/             ← si je veux des classes d’accès à la base personnalisées  
│   │   ├── services/                  ← services utilitaires partagés entre modules  
│   │   ├── utils/                     ← helpers, validations, conversion, etc.  
│   │   └── index.ts                  ← point d’entrée (initialisation custom)  
│   ├── medusa-config.ts              ← config de Medusa v2 (plugins, etc.)  
│   ├── .env                           ← variables d’environnement  
│   ├── .env.template                  ← modèle d’exemple  
│   ├── package.json  
│   ├── tsconfig.json  
│   ├── tsconfig.server.json  
│   ├── tsconfig.admin.json  
│   ├── .gitignore  
│   └── README.md
│
├── frontend/
│   ├── public/
│   │   ├── images/
│   │   └── favicon.ico
│   ├── src/
│   │   ├── components/                ← “blocs” réutilisables (ex : carte de chambre)  
│   │   ├── pages/                     ← pages (home, liste chambres, détail, réservation, profil)  
│   │   ├── services/                  ← fonctions pour appeler l’API backend (fetch, axios)  
│   │   ├── utils/                      ← fonctions utilitaires en frontend  
│   │   ├── styles/                     ← fichiers CSS ou SCSS  
│   │   └── main.js                     ← point d’entrée JS  
│   ├── index.html  
│   ├── package.json (si j'utilises bundleur ou outils JS)  
│   ├── .gitignore  
│   └── README.md
│
├── docs/                             ← cahier des charges, maquettes, diagrammes, wireframes  
│
├── documentations/                   ← documentation technique :  
│   ├── installation.md               ← guide d’installation du projet  
│   ├── architecture.md               ← explication de la structure du code  
│   ├── api-reference.md              ← endpoints et exemples d’appels API  
│   ├── backend-notes.md              ← notes techniques sur Medusa.js  
│   └── frontend-notes.md             ← logique côté client, intégration API  
│
├── scripts/                          ← scripts utilitaires (seed DB, nettoyage, etc.)  
├── .gitignore  
├── README.md                         ← aperçu global du projet  
└── LICENSE (optionnel)
