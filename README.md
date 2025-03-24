# GETDESK

Office Booking est une application open source permettant la réservation de bureaux en entreprise. Ce projet vise à faciliter la gestion des espaces de travail en offrant une interface intuitive et une API performante.

## Fonctionnalités

- Gestion des bureaux et des disponibilités
- Réservation en temps réel avec confirmation
- Authentification et gestion des utilisateurs
- Vue calendrier des réservations
- API REST pour intégration avec d'autres systèmes
- Notifications par e-mail pour les réservations
- Tableau de bord administrateur

## Technologies utilisées

- Backend : Symfony 7.2, API Platform
- Base de données : PostgreSQL
- Frontend : React avec Vite
- Conteneurisation : Docker, Docker Compose
- Authentification : JWT (LexikJWTAuthenticationBundle)

## Installation

### Prérequis

- Docker & Docker Compose
- PHP 8.2
- Composer
- Node.js et npm/yarn

### Déploiement local

1. Cloner le dépôt :
   ```bash
   git clone https://github.com/Neyo03/getdesk.git
   cd getdesk
   ```

2. Lancer les services avec Docker :
   ```bash
   docker-compose up -d
   ```

3. Installer les dépendances backend :
   ```bash
   composer install
   ```

4. Installer les dépendances frontend :
   ```bash
   cd frontend
   npm install  # ou yarn install
   ```

5. Exécuter les migrations :
   ```bash
   symfony console doctrine:migrations:migrate
   ```

6. Accéder à l'application :
   - Frontend : `http://localhost:3000`
   - API : `http://localhost:8000/api`

## Contribution

Les contributions sont les bienvenues ! Merci de respecter les bonnes pratiques de développement et de soumettre une Pull Request après avoir forké le projet.

## Licence

Ce projet est sous licence MIT. Voir le fichier [LICENSE](LICENSE) pour plus d'informations.

