# Suivi de Caisse - Application de Gestion Financière

Une application moderne de suivi de caisse multi-utilisateurs avec base de données décentralisée.

## 🚀 Fonctionnalités

- **Gestion des transactions** : Entrées, sorties, transferts et opérations bancaires
- **Multi-utilisateurs** : Gestion des rôles admin/utilisateur
- **Gestion clients** : Suivi des clients et recouvrements
- **Comptes bancaires** : Gestion multi-comptes et multi-devises
- **Commandes clients** : Suivi des commandes et livraisons
- **Tableaux de bord** : Statistiques et analyses en temps réel
- **Base de données décentralisée** : Synchronisation en ligne avec Supabase
- **Application mobile** : Support Android avec Capacitor

## 🛠️ Technologies

- **Frontend** : React 18 + TypeScript + Tailwind CSS
- **Base de données** : Supabase (PostgreSQL)
- **Mobile** : Capacitor pour Android
- **Déploiement** : Netlify
- **Icons** : Lucide React

## 📱 Installation et Configuration

### 1. Installation des dépendances
```bash
npm install
```

### 2. Configuration Supabase

1. Créez un compte sur [Supabase](https://supabase.com)
2. Créez un nouveau projet
3. Copiez `.env.example` vers `.env` et ajoutez vos clés :

```env
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

### 3. Configuration de la base de données

1. Dans votre projet Supabase, allez dans l'éditeur SQL
2. Exécutez les migrations dans l'ordre :
   - `supabase/migrations/create_tables.sql`
   - `supabase/migrations/insert_initial_data.sql`

### 4. Lancement de l'application

```bash
# Mode développement
npm run dev

# Build pour production
npm run build

# Aperçu de production
npm run preview
```

## 📱 Application Mobile Android

### Configuration
```bash
# Synchroniser avec Capacitor
npm run capacitor:sync

# Lancer sur Android
npm run android

# Build et lancer
npm run android:build
```

## 🗄️ Structure de la Base de Données

### Tables principales :
- **users** : Utilisateurs de l'application
- **transactions** : Toutes les transactions financières
- **categories** : Catégories et sous-catégories
- **clients** : Informations clients
- **bank_accounts** : Comptes bancaires
- **client_orders** : Commandes des clients

### Sécurité :
- Row Level Security (RLS) activé sur toutes les tables
- Authentification requise pour toutes les opérations
- Politiques de sécurité configurées

## 🔧 Fonctionnalités Avancées

### Synchronisation Hors Ligne
- Stockage local avec localStorage comme fallback
- Synchronisation automatique avec Supabase quand disponible
- Indicateur de statut de connexion

### Gestion des Données
- Import/Export des données en JSON
- Sauvegarde automatique
- Réinitialisation des données

### Interface Responsive
- Design mobile-first
- Navigation adaptative
- Optimisé pour tous les écrans

## 🚀 Déploiement

L'application est automatiquement déployée sur Netlify. Pour déployer manuellement :

```bash
npm run build
# Puis déployez le dossier 'dist' sur votre hébergeur
```

## 📊 Utilisation

### 1. Tableau de Bord
- Vue d'ensemble des finances
- Statistiques en temps réel
- Aperçu des utilisateurs et clients

### 2. Transactions
- Ajout de nouvelles transactions
- Filtrage et recherche avancés
- Modification et suppression

### 3. Gestion Clients
- Ajout et modification de clients
- Suivi des commandes
- Analyse du recouvrement

### 4. Paramètres
- Gestion des utilisateurs
- Configuration des catégories
- Comptes bancaires
- Import/Export des données

## 🔒 Sécurité

- Authentification Supabase
- Chiffrement des données en transit
- Politiques de sécurité au niveau base de données
- Validation côté client et serveur

## 🤝 Contribution

1. Fork le projet
2. Créez une branche feature (`git checkout -b feature/AmazingFeature`)
3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrez une Pull Request

## 📝 Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## 📞 Support

Pour toute question ou support, contactez l'équipe de développement.

---

**Suivi de Caisse** - Une solution complète pour la gestion financière d'entreprise 🏢💰