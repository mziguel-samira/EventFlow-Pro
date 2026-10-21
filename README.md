# EventFlow Pro 🗓️

Une application web complète et responsive de gestion d'événements, conçue pour offrir une expérience utilisateur fluide et un déploiement cloud hautement disponible.

## 📖 À propos du projet
**EventFlow Pro** est une Single Page Application (SPA) permettant à chaque utilisateur de gérer son agenda personnel de manière centralisée. L'application intègre la création d'événements, un calendrier interactif, un système d'authentification sécurisé et l'envoi de rappels automatiques par email.

L'objectif technique de ce projet était de concevoir une application front-end performante et de la déployer en environnement de production sur **Microsoft Azure**, en appliquant les bonnes pratiques de sécurité, de monitoring et d'optimisation des coûts.

## 🚀 Fonctionnalités principales
- **Tableau de bord** : Vue globale avec statistiques (événements à venir, terminés, rappels actifs).
- **Gestion d'événements** : Création, édition et suppression avec catégorisation (Anniversaire, Fête, Conférence, Match, Autre).
- **Calendrier interactif** : Vue mensuelle dynamique avec indicateurs visuels.
- **Rappels Gmail** : Notifications automatiques paramétrables (J-7, J-3, J-1) via l'API.
- **Authentification** : Inscription et connexion sécurisées (hachage SHA-256) avec option SSO Google.
- **Interface personnalisable** : Mode sombre / mode clair, gestion du profil et des préférences utilisateur.

## ☁️ Architecture Cloud & Services Azure
L'application a été déployée sur **Microsoft Azure App Service** en utilisant les services suivants :
- **Azure App Service** : Hébergement de l'application web (Plan F1).
- **Kudu (SCM)** : Déploiement manuel et gestion des fichiers dans le répertoire `/wwwroot`.
- **Sécurité** : HTTPS natif avec TLS 1.3 activé par défaut, aucun secret exposé dans le code.
- **Monitoring** : Application Insights et Azure Monitor pour le suivi des performances (Uptime > 99,9%).

## 🛠️ Stack technologique
- **Frontend** : HTML5, CSS3, JavaScript (Vanilla).
- **Stockage** : `localStorage` (côté client) pour la persistance des données.
- **Services Cloud** : Microsoft Azure, API Gmail.
- **Outils** : Git, GitHub, Kudu.

## 💻 Lancement en local
Puisqu'il s'agit d'une Single Page Application tout-en-un, aucune installation complexe n'est requise :
1. Clonez ce dépôt.
2. Ouvrez le fichier `index.html` dans n'importe quel navigateur web moderne.

## 🔗 Application en Production
L'application est déployée et accessible à l'URL suivante :
`https://evenement-bpg8cr6htejcgve.germanywestcentral-01.azurewebsites.net`