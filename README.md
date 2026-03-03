# Portfolio - Fatoumata Sall

Portfolio personnel développé avec Astro et déployé sur Vercel.

## 🚀 À propos

Ce portfolio présente mon parcours en tant qu'étudiante en 1ère année de Licence en Informatique à l'ESISA. Il contient mes informations personnelles, mes compétences, mes projets et mes coordonnées de contact.

## 📋 Structure du site

- **Accueil** : Présentation générale et appel à l'action
- **À propos** : Parcours, formation, compétences et objectifs
- **Projets** : Liste des projets réalisés et à venir
- **Contact** : Formulaire de contact et liens sociaux

## 🛠️ Technologies utilisées

- **Astro** : Framework web moderne et performant
- **HTML/CSS** : Structure et design responsive
- **JavaScript** : Interactivité du formulaire de contact
- **Vercel** : Plateforme de déploiement automatique

## 💻 Installation et développement local

### Prérequis

- Node.js (version 18 ou supérieure)
- npm ou yarn

### Installation

```bash
# Cloner le dépôt
git clone https://github.com/sallfatou/portfolio.git
cd portfolio

# Installer les dépendances
npm install

# Lancer le serveur de développement
npm run dev
```

Le site sera accessible à l'adresse : `http://localhost:4321`

### Commandes disponibles

| Commande                   | Action                                           |
| :------------------------- | :----------------------------------------------- |
| `npm install`              | Installe les dépendances                         |
| `npm run dev`              | Lance le serveur de développement                |
| `npm run build`            | Génère le site pour la production (`./dist/`)   |
| `npm run preview`          | Prévisualise le build en local                   |
| `npm run astro ...`        | Exécute une commande Astro spécifique           |

## ✏️ Comment mettre à jour le contenu

### Informations personnelles

Les informations personnelles sont directement intégrées dans les pages. Pour les modifier :

1. **Page d'accueil** : Éditez `src/pages/index.astro`
2. **Page À propos** : Éditez `src/pages/about.astro`
3. **Page Contact** : Éditez `src/pages/contact.astro`

### Ajouter un projet

Pour ajouter un nouveau projet, éditez le fichier `src/pages/projects.astro` :

```javascript
const upcomingProjects = [
	{
		title: "Nom du projet",
		description: "Description détaillée du projet",
		status: "À venir", // ou "En cours" ou "Terminé"
		category: "Catégorie",
		skills: ["Compétence1", "Compétence2"]
	},
	// ... autres projets
];
```

Pour un projet terminé avec lien GitHub :

```javascript
const completedProjects = [
	{
		title: "Nom du projet",
		description: "Description du projet",
		status: "Terminé",
		category: "Catégorie",
		skills: ["Compétence1", "Compétence2"],
		github: "https://github.com/sallfatou/nom-du-projet",
		demo: "https://demo-url.com" // optionnel
	}
];
```

### Modifier les couleurs et le style

Les variables CSS globales sont définies dans `src/layouts/Layout.astro` :

```css
:root {
	--color-primary: #3b82f6;
	--color-primary-dark: #2563eb;
	--color-text: #1f2937;
	--color-text-light: #6b7280;
	--color-bg: #ffffff;
	--color-bg-alt: #f9fafb;
	--color-border: #e5e7eb;
}
```

## 🚀 Déploiement sur Vercel

### Déploiement automatique

Le site est configuré pour un déploiement automatique depuis GitHub vers Vercel :

1. **Push sur GitHub** : Chaque push sur la branche `main` déclenche un déploiement
2. **Build automatique** : Vercel exécute `npm run build` automatiquement
3. **Publication** : Le site mis à jour est disponible en quelques secondes

### Configuration manuelle

Si vous souhaitez déployer manuellement :

1. Créez un compte sur [Vercel](https://vercel.com)
2. Connectez votre dépôt GitHub
3. Sélectionnez le framework "Astro"
4. Cliquez sur "Deploy"

### Variables d'environnement (optionnel)

Aucune variable d'environnement n'est requise pour ce projet de base.

## 📁 Structure des fichiers

```
portfolio/
├── public/              # Fichiers statiques (images, favicon, etc.)
├── src/
│   ├── layouts/
│   │   └── Layout.astro # Layout principal avec navigation et footer
│   ├── pages/
│   │   ├── index.astro  # Page d'accueil
│   │   ├── about.astro  # Page À propos
│   │   ├── projects.astro # Page Projets
│   │   └── contact.astro  # Page Contact
├── astro.config.mjs     # Configuration Astro
├── tsconfig.json        # Configuration TypeScript
├── package.json         # Dépendances du projet
├── vercel.json          # Configuration Vercel
└── README.md            # Ce fichier
```

## 🎨 Fonctionnalités

- ✅ Design responsive (mobile, tablette, desktop)
- ✅ Navigation sticky avec liens actifs
- ✅ Animations et transitions fluides
- ✅ Formulaire de contact fonctionnel
- ✅ Code commenté et réutilisable
- ✅ Optimisé pour les performances
- ✅ Respect des bonnes pratiques d'accessibilité

## 📝 Accessibilité

Ce portfolio respecte les bonnes pratiques d'accessibilité :

- Navigation au clavier
- Attributs ARIA appropriés
- Contrastes de couleurs suffisants
- Textes alternatifs pour les éléments visuels
- Structure sémantique HTML

## 📧 Contact

- **Email** : f.sall@esisa.ac.ma
- **GitHub** : [@sallfatou](https://github.com/sallfatou)
- **Portfolio** : [Lien à venir après déploiement]

## 📄 Licence

Ce projet est un portfolio personnel. Vous êtes libre de vous en inspirer pour créer le vôtre.

---

**Développé avec ❤️ par Fatoumata Sall**

*Dernière mise à jour : Mars 2026*
