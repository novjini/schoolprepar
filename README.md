# SchoolPrepar — Plateforme d'Orientation Scolaire

> Projet réalisé dans le cadre du TP1 – IT 232 – Développement Web II  
> Année Académique 2025–2026 | Licence GL | iP Net Institute of Technology

---

## Présentation

**SchoolPrepar** est une plateforme numérique d'orientation scolaire et professionnelle.  
Elle permet aux élèves de :
- Rechercher des filières et établissements
- Accéder à des conseils personnalisés de mentors et conseillers
- Passer des quiz d'orientation et tests de personnalité
- Rejoindre une communauté éducative active

---

## Stack Technique

| Technologie     | Version     |
|-----------------|-------------|
| PHP             | 8.2+        |
| Symfony         | 6.4.*       |
| Twig            | 3.x         |
| Doctrine ORM    | 3.x         |
| MySQL           | 8.x         |
| Git             | 2.x         |

---

##  Installation

### Prérequis
- PHP >= 8.2
- Composer
- Symfony CLI
- MySQL

### Étapes

```bash
# 1. Cloner le dépôt
git clone https://github.com/VOTRE_USERNAME/schoolprepar.git
cd schoolprepar

# 2. Installer les dépendances
composer install

# 3. Configurer l'environnement
cp .env .env.local
# Modifier DATABASE_URL dans .env.local

# 4. Créer la base de données
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate

# 5. Lancer le serveur
symfony server:start
```

Accéder à l'application : **http://localhost:8000**

---

## Structure du Projet

```
schoolprepar/
├── assets/               # Fichiers JS/CSS front-end
├── config/               # Configuration Symfony (routes, services...)
├── migrations/           # Migrations Doctrine
├── public/               # Point d'entrée (index.php)
├── src/
│   ├── Controller/       # Contrôleurs MVC
│   ├── Entity/           # Entités Doctrine
│   ├── Form/             # Formulaires Symfony
│   ├── Repository/       # Requêtes BDD
│   └── Service/          # Services métier
├── templates/            # Vues Twig
│   ├── base.html.twig    # Layout principal
│   └── ...
├── tests/                # Tests unitaires et fonctionnels
├── .env                  # Variables d'environnement
├── composer.json
└── README.md
```

---



## Acteurs de la Plateforme

| Acteur            | Rôle                                              |
|-------------------|---------------------------------------------------|
| Élève             | Recherche, quiz, prise de RDV, forum              |
| Conseiller        | Accompagnement, gestion disponibilités            |
| Ancien élève      | Partage d'expérience, mentorat                    |
| Professionnel     | Témoignages, visioconférences                     |
| Administrateur    | Gestion CRUD, statistiques, contenus              |

---

##  Modélisation

Les diagrammes suivants sont disponibles dans le dossier `/docs` :
- Diagramme des cas d'utilisation
- Diagramme Entité–Relation (ERD)

---

##  Auteur

**OUMONGOU NIHADE** — Licence [GL]  
iP Net Institute of Technology  
Chargé de cours : M. EDOU Dodji

---

## Licence

Projet académique — Tous droits réservés © 2025–2026