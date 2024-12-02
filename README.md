# HotTakes / Piiquante 🌶️

Projet 6 du parcours Développeur Web d'OpenClassrooms : Création d'une API sécurisée pour une application d'évaluation de sauces piquantes.

## Scénario

Piiquante se dédie à la création de sauces épicées dont les recettes sont gardées secrètes. Pour tirer parti de son succès et générer davantage de buzz, l'entreprise a lancé une application web permettant aux utilisateurs de partager leurs sauces préférées et d'interagir avec la communauté.

## Fonctionnalités

Les utilisateurs peuvent :
- Créer un compte et se connecter de manière sécurisée
- Ajouter leurs propres sauces avec photo et description
- Modifier et supprimer leurs sauces
- Noter les sauces des autres utilisateurs (like/dislike)
- Voir la liste de toutes les sauces disponibles

## Stack Technique

### Frontend
- Angular 13.2.4
- Angular CLI
- Angular Material
- TypeScript
- SCSS

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT pour l'authentification
- Multer pour la gestion des fichiers
- Bcrypt pour le hashage des mots de passe
- Autres packages : 
  - Body-parser
  - CORS
  - Dotenv
  - Mongoose-errors
  - Mongoose-unique-validator
  - Password-validator
  - Serve-static
  - Validator

## Installation et Configuration

### Prérequis
- Node.js et npm
- MongoDB
- Angular CLI (`npm install -g @angular/cli`)

### Configuration du Backend
```bash
cd backend
npm install
# Créez un fichier .env avec vos variables d'environnement
npm start
```
Le serveur backend sera accessible sur `http://localhost:3000`

### Configuration du Frontend
```bash
cd frontend
npm install
ng serve
```
L'application sera accessible sur `http://localhost:4200`

## Guide du Développeur

### Commandes Frontend Angular
- `ng serve` : Lance le serveur de développement
- `ng build` : Compile l'application (les fichiers seront stockés dans le dossier `dist/`)
- `ng generate component component-name` : Génère un nouveau composant
- `ng test` : Lance les tests unitaires via [Karma](https://karma-runner.github.io)
- `ng e2e` : Lance les tests end-to-end
- `ng help` : Aide sur les commandes Angular CLI

### Documentation
Pour plus d'informations sur Angular CLI :
- [Angular CLI Overview and Command Reference](https://angular.io/cli)

## Sécurité

L'application implémente plusieurs mesures de sécurité :
- Authentification par token JWT
- Hashage des mots de passe avec bcrypt
- Validation des données côté serveur
- Protection contre les injections NoSQL
- Gestion sécurisée des fichiers uploadés
- Validation du mot de passe avec password-validator

## Structure du Projet

```
HotTakes/
├── backend/         # API Node.js + Express
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   └── routes/
└── frontend/        # Application Angular
    ├── src/
    ├── e2e/
    └── dist/
```

## Contribution

Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou à soumettre une pull request.

## Licence

Ce projet a été réalisé dans le cadre du parcours Développeur Web d'OpenClassrooms.
