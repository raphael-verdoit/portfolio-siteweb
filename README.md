# Portfolio Statique - Jean Dupont

Une **portfolio website 100% statique** pour un étudiant BTS SIO. Aucun Node.js, npm, ou build tools requis!

## 🚀 Caractéristiques

✅ **Aucune dépendance** - Juste HTML, CSS et JavaScript vanilla  
✅ **Mode sombre** - Toggle dark/light mode avec persistance  
✅ **Responsive** - Fonctionne parfaitement sur mobile, tablette et desktop  
✅ **Rapide** - Charge instantanément, aucun build nécessaire  
✅ **Facile à personnaliser** - Modifiez le contenu directement dans le HTML  
✅ **Prêt pour Netlify** - Déployez en quelques clics  

## 📁 Structure des Fichiers

```
portfolio-static/
├── index.html          # Page principale (contenu)
├── styles.css          # Styles (design, responsive, dark mode)
├── script.js           # Interactivité (navigation, dark mode, formulaire)
├── README.md           # Ce fichier
└── .gitignore          # Fichiers à ignorer (optionnel)
```

## 🎨 Design

**Philosophie de Design:** Elegant Minimalism
- Typographie raffinée avec beaucoup d'espace blanc
- Accents terracotta chaud (#c85a54) pour les CTAs
- Esthétique professionnelle et épurée
- Support complet du mode sombre

## 📝 Comment Personnaliser

### 1. Modifier le Contenu

Ouvrez `index.html` avec un éditeur de texte et modifiez:

- **Votre nom:** Cherchez "Jean Dupont" et remplacez
- **Titre professionnel:** Modifiez le hero-title
- **Description:** Changez le hero-subtitle
- **Projets:** Éditez les portfolio-card
- **CV:** Mettez à jour la section CV
- **Contact:** Changez email, téléphone, LinkedIn, GitHub

### 2. Modifier le Design

Ouvrez `styles.css` et modifiez les variables CSS au début:

```css
:root {
    /* Couleurs */
    --accent-primary: #c85a54;      /* Couleur principale */
    --accent-secondary: #1b6b6b;    /* Couleur secondaire */
    --text-primary: #3c3c3c;        /* Texte principal */
    --bg-primary: #fefdf9;          /* Fond principal */
}
```

### 3. Ajouter des Images

1. Créez un dossier `images/` dans le même répertoire
2. Ajoutez vos images dedans
3. Référencez-les dans le HTML:
```html
<img src="images/votre-image.jpg" alt="Description">
```

## 🌐 Déployer sur Netlify

### Méthode 1: Drag & Drop (La Plus Simple)

1. Allez sur [netlify.com](https://netlify.com)
2. Créez un compte (gratuit)
3. Glissez-déposez le dossier `portfolio-static` sur la zone de Netlify
4. Votre site est en ligne! 🎉

### Méthode 2: GitHub + Netlify (Recommandé)

1. Poussez votre code sur GitHub
2. Connectez votre repo GitHub à Netlify
3. Netlify redéploie automatiquement à chaque push

### Méthode 3: Hébergement Traditionnel

1. Générez la version finale: `npm run build` (si vous avez Node.js)
2. Uploadez les fichiers via FTP sur votre hébergeur
3. C'est tout!

## 🔧 Fonctionnalités JavaScript

### Dark Mode
- Toggle automatique avec sauvegarde en localStorage
- Persiste lors du rechargement de la page

### Navigation Active
- Le lien de navigation actif se met à jour au scroll
- Smooth scroll vers les sections

### Formulaire de Contact
- Validation des champs
- Validation de l'email
- Message de succès
- Note: Pour envoyer les emails, intégrez Formspree, Netlify Forms ou EmailJS

### Animations
- Fade-in des cartes au scroll
- Parallax sur la décoration du hero
- Hover effects sur les cartes

## 📧 Activer les Emails (Optionnel)

Le formulaire de contact est actuellement une démo. Pour envoyer les emails:

### Option 1: Formspree (Recommandé)
1. Allez sur [formspree.io](https://formspree.io)
2. Créez un nouveau formulaire
3. Remplacez l'action du formulaire dans le HTML:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: Netlify Forms
1. Renommez votre form avec `netlify`:
```html
<form name="contact" method="POST" netlify>
```
2. Netlify gère automatiquement les soumissions

## 🎯 Checklist Avant Déploiement

- [ ] Remplacé "Jean Dupont" par votre nom
- [ ] Mis à jour la description personnelle
- [ ] Modifié les projets du portfolio
- [ ] Mis à jour le CV
- [ ] Changé les coordonnées de contact
- [ ] Testé le site localement
- [ ] Testé le mode sombre
- [ ] Testé la responsivité sur mobile
- [ ] Testé les liens de navigation

## 🚀 Lancer Localement

Deux façons:

### Méthode 1: Double-cliquer sur index.html
- Ouvrez `index.html` directement dans votre navigateur
- Le site fonctionne immédiatement

### Méthode 2: Serveur Local (Recommandé)
```bash
# Avec Python 3
python -m http.server 8000

# Avec Python 2
python -m SimpleHTTPServer 8000

# Avec Node.js (si vous l'avez)
npx http-server
```
Puis allez sur `http://localhost:8000`

## 🐛 Dépannage

| Problème | Solution |
|----------|----------|
| Styles ne s'appliquent pas | Vérifiez que `styles.css` est dans le même dossier que `index.html` |
| Dark mode ne fonctionne pas | Vérifiez que `script.js` est chargé correctement |
| Images manquantes | Vérifiez les chemins des images dans le HTML |
| Formulaire ne marche pas | Intégrez Formspree ou Netlify Forms |

## 📱 Responsive Design

Le site s'adapte automatiquement à:
- **Desktop:** 1200px et plus
- **Tablet:** 768px - 1199px
- **Mobile:** moins de 768px

## 🎓 Améliorations Futures

- Ajouter un blog/articles
- Intégrer un système de commentaires
- Ajouter des animations plus avancées
- Intégrer une galerie de projets
- Ajouter un système de filtrage des projets

## 📄 Licence

Libre d'utilisation et de modification.

## 💬 Questions?

Consultez la documentation ou modifiez directement le code. C'est simple et transparent!

---

**Bon courage pour votre portfolio!** 🎉
