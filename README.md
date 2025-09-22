# Programme Minceur LR Pro

Application web professionnelle pour le suivi de programmes minceur avec gestion multi-utilisateurs, base de données sécurisée et déploiement en ligne.

## 🚀 Fonctionnalités

### Pour les Clients
- **Profil personnel** avec informations complètes
- **Mesures corporelles** avec historique et graphiques
- **Routine quotidienne** personnalisée par le partenaire
- **Suivi quotidien** avec graphiques d'évolution
- **Upload de photos et vidéos** pour le suivi

### Pour les Partenaires LR
- **Gestion des clients** avec création et suivi
- **Diagnostic personnalisé** avec recommandations de produits
- **Catalogue de produits LR** complet
- **Suivi des progrès** de tous leurs clients
- **Routines personnalisées** pour chaque client

### Pour les Administrateurs
- **Gestion complète** de tous les utilisateurs
- **Statistiques globales** de l'application
- **Administration** des produits et diagnostics

## 🛠️ Technologies

- **Frontend** : HTML5, CSS3, JavaScript (ES6+)
- **Base de données** : Supabase (PostgreSQL)
- **Authentification** : Supabase Auth
- **Graphiques** : Chart.js
- **Déploiement** : Netlify
- **Sécurité** : Row Level Security (RLS)

## 📦 Installation

### 1. Cloner le projet
```bash
git clone <repository-url>
cd programme-minceur-lr-pro
```

### 2. Configurer Supabase

1. Créer un projet sur [Supabase](https://supabase.com)
2. Exécuter le script SQL `supabase-schema.sql` dans l'éditeur SQL
3. Récupérer l'URL et la clé anonyme du projet

### 3. Configurer l'application

1. Ouvrir `app.js`
2. Remplacer les variables de configuration :
```javascript
const SUPABASE_URL = 'YOUR_SUPABASE_URL';
const SUPABASE_ANON_KEY = 'YOUR_SUPABASE_ANON_KEY';
```

### 4. Déployer sur Netlify

1. Connecter le repository à Netlify
2. Configurer les variables d'environnement si nécessaire
3. Déployer automatiquement

## 🗄️ Structure de la base de données

### Tables principales
- **profiles** : Informations des utilisateurs
- **measurements** : Mesures corporelles
- **tracking_entries** : Suivi quotidien
- **routines** : Routines personnalisées
- **selected_products** : Produits sélectionnés
- **diagnostics** : Diagnostics et recommandations
- **media_files** : Photos et vidéos
- **goals** : Objectifs de perte de poids
- **follow_up_notes** : Notes de suivi

### Sécurité
- **Row Level Security (RLS)** activé sur toutes les tables
- **Politiques de sécurité** pour isoler les données par utilisateur
- **Authentification** via Supabase Auth
- **Autorisations** basées sur le type d'utilisateur

## 🔐 Types d'utilisateurs

### Client
- Accès à son propre profil, mesures, routine et suivi
- Peut ajouter des mesures et des entrées de suivi
- Peut uploader des photos et vidéos
- Accès en lecture seule à sa routine

### Partenaire LR
- Gestion de ses clients
- Création de routines personnalisées
- Diagnostic et recommandations de produits
- Suivi des progrès de tous ses clients

### Administrateur
- Accès complet à toutes les fonctionnalités
- Gestion de tous les utilisateurs
- Administration de l'application

## 📱 Interface utilisateur

### Design responsive
- **Mobile-first** avec adaptation desktop
- **Couleurs LR** : Vert principal (#809478), beige secondaire (#f2e1c3)
- **Composants** : Cards, modals, formulaires stylisés
- **Navigation** : Onglets adaptatifs selon le type d'utilisateur

### Fonctionnalités clés
- **Graphiques interactifs** pour le suivi des progrès
- **Upload de fichiers** avec aperçu
- **Modals** pour les actions importantes
- **Validation** des formulaires en temps réel

## 🚀 Déploiement

### Netlify
1. Connecter le repository GitHub
2. Configurer le build (pas de build step nécessaire)
3. Déployer automatiquement

### Variables d'environnement
```bash
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_supabase_anon_key
```

## 🔧 Développement

### Structure des fichiers
```
├── index.html          # Page principale
├── styles.css          # Styles CSS
├── app.js             # Logique JavaScript
├── supabase-schema.sql # Schéma de base de données
├── netlify.toml       # Configuration Netlify
└── README.md          # Documentation
```

### Fonctionnalités à développer
- [ ] Système de notifications
- [ ] Export PDF des rapports
- [ ] API REST pour intégrations
- [ ] Application mobile (React Native)
- [ ] Système de paiement
- [ ] Intégration avec les APIs LR

## 📊 Sécurité et conformité

### RGPD
- **Consentement** explicite pour le traitement des données
- **Droit à l'effacement** des données personnelles
- **Portabilité** des données
- **Transparence** sur l'utilisation des données

### Sécurité des données
- **Chiffrement** des données sensibles
- **Authentification** forte
- **Audit** des accès et modifications
- **Sauvegarde** automatique des données

## 🤝 Contribution

1. Fork le projet
2. Créer une branche feature
3. Commiter les changements
4. Pousser vers la branche
5. Ouvrir une Pull Request

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

## 📞 Support

Pour toute question ou problème :
- **Email** : contact.teamdanlr@gmail.com
- **Téléphone** : 06 20 49 37 76
- **Facebook** : [@LR Health & Beauty](https://www.facebook.com/profile.php?id=61580422450746)

---

**Réalisé par : Daniaux Christophe**  
**Partenaire : LR Health & Beauty**
