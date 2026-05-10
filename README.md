# Smart Management Platform

> **Projet Full Stack : Spring Boot · Angular · JWT Authentication · REST API**
> ENSET Mohammedia — Université Hassan II de Casablanca
> Module : Java Enterprise Applications & Web Frameworks

---

## 👨‍💻 Réalisé par

**Mostapha Bayi**

---

# 📌 Présentation du Projet

**Smart Management Platform** est une application web moderne permettant la gestion centralisée des données, utilisateurs et opérations métier à travers une architecture full-stack basée sur **Spring Boot** et **Angular**.

L’objectif principal du projet est de concevoir une plateforme sécurisée, performante et responsive capable de gérer différentes opérations via une API REST et une interface utilisateur dynamique.

Le système implémente :

* Authentification sécurisée avec JWT
* Gestion des utilisateurs et des rôles
* Architecture RESTful
* Communication Frontend ↔ Backend via HTTP/JSON
* Validation des données côté client et serveur
* Interface responsive moderne avec Angular

---

# 🗂️ Structure du Projet

```bash
project-root/
├── backend/      # API Spring Boot
│   ├── src/
│   ├── pom.xml
│   └── mvnw
│
└── frontend/     # Application Angular
    ├── src/
    ├── angular.json
    ├── package.json
    └── public/
```

---

# 🏗️ Architecture Générale

```text
┌──────────────────────────────┐
│         Client Web           │
│        Angular Frontend      │
│      Components · Services   │
└──────────────┬───────────────┘
               │ HTTP / JSON
               ▼
┌──────────────────────────────┐
│        Spring Boot API       │
│ Controllers · Services       │
│ Security · Business Logic    │
└──────────────┬───────────────┘
               ▼
┌──────────────────────────────┐
│          Database            │
│      MySQL / PostgreSQL      │
└──────────────────────────────┘
```

---

# ⚙️ Technologies Utilisées

## Backend

| Technologie     | Rôle                            |
| --------------- | ------------------------------- |
| Java 17         | Langage principal               |
| Spring Boot     | Développement Backend           |
| Spring Web      | Création API REST               |
| Spring Security | Authentification & Autorisation |
| JWT             | Sécurisation des requêtes       |
| Spring Data JPA | Accès aux données               |
| Hibernate       | ORM                             |
| Maven           | Gestion des dépendances         |
| Lombok          | Réduction du boilerplate        |

---

## Frontend

| Technologie    | Rôle                    |
| -------------- | ----------------------- |
| Angular        | Développement SPA       |
| TypeScript     | Typage statique         |
| RxJS           | Programmation réactive  |
| HTML5 / CSS3   | Interface utilisateur   |
| Angular Router | Navigation              |
| Angular Forms  | Gestion des formulaires |

---

# 🚀 Fonctionnalités Principales

## 🔐 Authentification

* Connexion utilisateur sécurisée
* Gestion des tokens JWT
* Protection des routes privées
* Gestion des rôles utilisateurs

---

## 📊 Tableau de Bord

* Vue globale des données
* Navigation rapide
* Affichage dynamique des statistiques
* Interface responsive

---

## 📁 Gestion des Données

* Création des enregistrements
* Modification des données
* Suppression sécurisée
* Recherche et filtrage
* Validation des formulaires

---

# 🔄 Flux de Communication

```text
Utilisateur
    ↓
Angular Frontend
    ↓ HTTP Request
Spring Boot REST API
    ↓
Service Layer
    ↓
Repository Layer
    ↓
Database
```

---

# 🔐 Sécurité JWT

```text
1. L'utilisateur se connecte
2. Spring Security valide les identifiants
3. Génération d'un JWT
4. Angular stocke le token
5. Chaque requête contient :
   Authorization: Bearer <token>
6. Le backend valide le JWT
7. Accès autorisé aux endpoints protégés
```

---

# 📦 API REST

```http
# Authentication
POST /api/auth/login
POST /api/auth/register

# Users
GET    /api/users
GET    /api/users/{id}
POST   /api/users
PUT    /api/users/{id}
DELETE /api/users/{id}

# Dashboard
GET /api/dashboard/stats
```

---

# 🧱 Architecture Backend

```text
Controller Layer
      ↓
Service Layer
      ↓
Repository Layer
      ↓
Database
```

---

# 📂 Organisation Frontend

```text
src/
├── app/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── models/
│   ├── guards/
│   └── interceptors/
│
├── assets/
└── environments/
```

---

# ▶️ Démarrage du Projet

## Prérequis

* Java 17+
* Maven 3+
* Node.js 20+
* Angular CLI

---

## 1️⃣ Lancer le Backend

```bash
cd backend
./mvnw spring-boot:run
```

Backend disponible sur :

```text
http://localhost:8080
```

---

## 2️⃣ Lancer le Frontend

```bash
cd frontend
npm install
ng serve
```

Frontend disponible sur :

```text
http://localhost:4200
```

# 📚 Concepts Techniques Utilisés

* Architecture REST
* Spring Dependency Injection
* Spring Security
* JWT Authentication
* Angular Services & Routing
* Reactive Forms
* HTTP Interceptors
* Layered Architecture
* DTO Mapping
* Exception Handling

---

# 🔗 Liens

| Ressource | URL                                                                      |
| --------- | ------------------------------------------------------------------------ |
| Frontend  | [http://localhost:4200](http://localhost:4200)                           |
| Backend   | [http://localhost:8080](http://localhost:8080)                           |
| Swagger   | [http://localhost:8080/swagger-ui](http://localhost:8080/swagger-ui)     |
| GitHub    | [https://github.com/Bayi-Mostapha/e-banking-platform](https://github.com/Bayi-Mostapha/e-banking-platform)) |

---

# 📖 Références

* Spring Boot Documentation
* Angular Documentation
* Spring Security Reference
* JWT Authentication Guide
* Hibernate ORM Documentation

---

<div align="center">

## Smart Management Platform

Projet Full Stack Spring Boot & Angular
Développé par **Mostapha Bayi**

</div>
