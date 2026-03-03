# Guide de déploiement sur Vercel

Ce guide explique comment déployer votre portfolio Astro sur Vercel.

## 📋 Prérequis

- Compte GitHub (déjà configuré avec le dépôt https://github.com/sallfatou/portfolio.git)
- Compte Vercel (gratuit) : https://vercel.com

## 🚀 Étapes de déploiement

### 1. Créer un compte Vercel

1. Allez sur https://vercel.com
2. Cliquez sur **"Sign Up"**
3. Choisissez **"Continue with GitHub"**
4. Autorisez Vercel à accéder à votre compte GitHub

### 2. Importer le projet

1. Une fois connecté, cliquez sur **"Add New..."** puis **"Project"**
2. Vous verrez la liste de vos dépôts GitHub
3. Trouvez **"portfolio"** dans la liste
4. Cliquez sur **"Import"** à côté du dépôt

### 3. Configurer le projet

Vercel détectera automatiquement qu'il s'agit d'un projet Astro :

- **Framework Preset** : Astro (détecté automatiquement)
- **Build Command** : `npm run build` (pré-rempli)
- **Output Directory** : `dist` (pré-rempli)
- **Install Command** : `npm install` (pré-rempli)

**Ne modifiez rien**, les paramètres par défaut sont corrects !

### 4. Déployer

1. Cliquez sur le bouton **"Deploy"**
2. Attendez 1-2 minutes pendant le déploiement
3. Une fois terminé, vous verrez un écran de succès avec confettis 🎉

## 🌐 Récupérer l'URL de votre portfolio

L'URL de votre portfolio sera de la forme :
```
https://portfolio-[random-string].vercel.app
```

Exemple : `https://portfolio-abc123xyz.vercel.app`

### Personnaliser le domaine (optionnel)

Pour un domaine personnalisé gratuit :

1. Dans le dashboard Vercel, allez dans **Settings** > **Domains**
2. Vous pouvez renommer votre projet pour obtenir une URL comme :
   ```
   https://fatoumata-sall.vercel.app
   ```

## 🔄 Déploiements automatiques

Désormais, **chaque fois que vous faites un `git push` vers GitHub**, Vercel redéploiera automatiquement votre site !

### Workflow de mise à jour

```bash
# Modifier vos fichiers localement
# Par exemple : src/pages/projects.astro

# Ajouter les modifications
git add .

# Créer un commit
git commit -m "Ajout d'un nouveau projet"

# Pousser vers GitHub
git push

# Vercel déploie automatiquement ! ✨
```

## 📊 Vérifier le statut du déploiement

1. Allez sur votre dashboard Vercel : https://vercel.com/dashboard
2. Cliquez sur votre projet **"portfolio"**
3. Vous verrez :
   - L'URL de production
   - L'historique des déploiements
   - Les logs de build
   - Les statistiques de performance

## 🎯 Ajouter l'URL à votre profil LinkedIn

Une fois le portfolio déployé :

1. Copiez l'URL de votre portfolio
2. Allez sur votre profil LinkedIn
3. Cliquez sur **"Ajouter une section de profil"** > **"Contact"**
4. Ajoutez l'URL dans la section **"Site web"**
5. Choix du type : **"Portfolio"**

## 🔧 En cas de problème

### Build échoue sur Vercel

1. Vérifiez les logs dans le dashboard Vercel
2. Testez localement avec `npm run build`
3. Vérifiez que toutes les dépendances sont dans `package.json`

### Le site ne s'affiche pas correctement

1. Videz le cache du navigateur (Ctrl + F5)
2. Vérifiez dans l'onglet "Deployments" que le dernier déploiement est réussi
3. Vérifiez les erreurs dans la console du navigateur (F12)

### Besoin de redéployer manuellement

1. Allez dans **Deployments**
2. Cliquez sur les **"..." ** à côté d'un déploiement
3. Choisissez **"Redeploy"**

## 📱 Tester sur mobile

Une fois déployé, vous pouvez tester votre portfolio sur mobile :

1. Ouvrez l'URL sur votre téléphone
2. Le site est responsive et s'adapte automatiquement !

## ✅ Checklist finale

- [ ] Portfolio déployé sur Vercel
- [ ] URL fonctionnelle et accessible
- [ ] Test sur ordinateur
- [ ] Test sur mobile/tablette
- [ ] URL ajoutée au profil LinkedIn
- [ ] URL partagée avec d'autres (optionnel)

## 🎓 Ressources utiles

- Documentation Astro : https://docs.astro.build
- Documentation Vercel : https://vercel.com/docs
- Dashboard Vercel : https://vercel.com/dashboard
- Support Vercel : https://vercel.com/support

---

**Félicitations ! Votre portfolio est maintenant en ligne ! 🎉**

Si vous avez des questions, n'hésitez pas à consulter la documentation ou à demander de l'aide.
