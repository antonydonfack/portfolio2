# CV Professionnel - Antonie Donfack Wamba

Portfolio et CV en ligne moderne, responsive et optimisé pour les performances.

## 🚀 Déploiement sur Netlify

### Méthode 1 : Déploiement direct (Recommandée)

1. **Préparer les fichiers**
   ```
   cv-professionnel/
   ├── index.html          # Fichier principal
   ├── netlify.toml        # Configuration Netlify
   ├── package.json        # Métadonnées du projet
   ├── README.md          # Documentation
   ├── cv-antonie-donfack.pdf  # CV en PDF
   └── assets/            # Ressources (si nécessaire)
       ├── images/
       └── documents/
   ```

2. **Déploiement via interface Netlify**
   - Aller sur [netlify.com](https://netlify.com)
   - Créer un compte gratuit
   - Cliquer sur "Add new site" → "Deploy manually"
   - Glisser-déposer le dossier complet
   - Le site sera automatiquement déployé

3. **Configuration du domaine personnalisé**
   - Dans les paramètres du site : Site settings → Domain management
   - Changer le nom : `antonie-cv.netlify.app` ou votre domaine personnalisé

### Méthode 2 : Déploiement via Git (Pour les mises à jour automatiques)

1. **Créer un repository GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit - CV professionnel"
   git branch -M main
   git remote add origin https://github.com/votre-username/cv-professionnel.git
   git push -u origin main
   ```

2. **Connecter à Netlify**
   - Sur Netlify : "Add new site" → "Import from Git"
   - Connecter GitHub et sélectionner le repository
   - Configuration de build :
     - Build command : `echo 'Build complete'`
     - Publish directory : `.` (racine)
   - Cliquer sur "Deploy site"

### Méthode 3 : Netlify CLI

1. **Installer Netlify CLI**
   ```bash
   npm install -g netlify-cli
   ```

2. **Déployer**
   ```bash
   netlify login
   netlify init
   netlify deploy --prod
   ```

## 📁 Structure des fichiers

### Fichiers requis
- `index.html` : Page principale du CV
- `netlify.toml` : Configuration Netlify (headers, redirections, optimisations)
- `package.json` : Métadonnées du projet

### Fichiers optionnels
- `cv-antonie-donfack.pdf` : Version PDF du CV
- `_redirects` : Redirections supplémentaires (si pas de netlify.toml)
- `robots.txt` : Instructions pour les moteurs de recherche
- `sitemap.xml` : Plan du site pour le SEO

## ⚡ Optimisations incluses

### Performance
- CSS et JS inline pour réduire les requêtes HTTP
- Images optimisées et lazy loading
- Mise en cache aggressive des ressources statiques
- Compression gzip automatique

### SEO
- Balises meta optimisées
- Structure HTML sémantique
- Schema.org markup pour les données structurées
- URLs propres et lisibles

### Sécurité
- Headers de sécurité (CSP, XSS Protection, etc.)
- Prévention du clickjacking
- Protection contre les attaques MIME

### Accessibilité
- Navigation au clavier
- Contraste des couleurs conforme WCAG
- Labels et descriptions pour les lecteurs d'écran
- Structure hiérarchique claire

## 🔧 Personnalisation

### Modifier les informations
1. Ouvrir `index.html`
2. Remplacer les sections :
   - Informations personnelles (nom, email, téléphone)
   - Compétences et pourcentages
   - Expériences professionnelles
   - Formation
   - Projets

### Modifier le design
1. Les styles sont dans la balise `<style>` du fichier HTML
2. Modifier les variables CSS :
   ```css
   :root {
     --primary-color: #2563eb;
     --secondary-color: #7c3aed;
     --accent-color: #fbbf24;
   }
   ```

### Ajouter des fonctionnalités
- Formulaire de contact avec Netlify Forms
- Intégration Google Analytics
- Mode sombre/clair
- Multilingue

## 📱 Test en local

1. **Serveur Python**
   ```bash
   python -m http.server 8000
   ```
   Puis ouvrir `http://localhost:8000`

2. **Serveur PHP**
   ```bash
   php -S localhost:8000
   ```

3. **Node.js http-server**
   ```bash
   npx http-server
   ```

## 🌍 Domaine personnalisé

### Avec Netlify (gratuit)
- Sous-domaine : `votre-nom.netlify.app`
- Configuration dans Site settings → Domain management

### Domaine custom
1. Acheter un domaine (.com, .dev, .tech, etc.)
2. Dans Netlify : Site settings → Domain management → Add custom domain
3. Configurer les DNS selon les instructions Netlify

## 📊 Analytics et monitoring

### Google Analytics
Ajouter dans `<head>` :
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Netlify Analytics
Activer dans Site settings → Analytics (payant mais très précis)

## 🔄 Mises à jour

### Déploiement manuel
1. Modifier les fichiers
2. Glisser-déposer le nouveau dossier sur Netlify

### Déploiement automatique (avec Git)
1. Modifier les fichiers
2. `git add . && git commit -m "Mise à jour CV" && git push`
3. Netlify redéploie automatiquement

## 🐛 Dépannage

### Site ne se charge pas
- Vérifier que `index.html` est à la racine
- Vérifier les erreurs dans la console développeur

### Styles cassés
- Vérifier que les liens CSS externes sont accessibles
- Tester en mode navigation privée

### Performance lente
- Optimiser les images
- Minimiser le CSS/JS
- Utiliser les suggestions de Lighthouse

## 📞 Support

En cas de problème :
1. Vérifier les logs de déploiement sur Netlify
2. Tester le site en local
3. Consulter la documentation Netlify
4. Contacter le support Netlify (communauté très active)

## 📝 License

Ce projet est sous licence MIT. Vous êtes libre de l'utiliser et le modifier selon vos besoins.

---

**Développé avec ❤️ par Antonie Donfack Wamba**  
📧 antonydonfack@icloud.com  
📱 +237 695 61 99 08