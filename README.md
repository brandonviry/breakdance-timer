# Breakdance Timer Plugin

![WordPress](https://img.shields.io/badge/WordPress-21759B?style=for-the-badge&logo=wordpress&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

![Version](https://img.shields.io/badge/version-0.0.1-blue.svg)
![License](https://img.shields.io/badge/license-Unlicensed-red.svg)
![WordPress](https://img.shields.io/badge/WordPress-5.0%2B-blue.svg)
![Breakdance](https://img.shields.io/badge/Breakdance-Required-orange.svg)

Un plugin WordPress personnalisé qui ajoute un élément de minuteur (countdown timer) pour Breakdance Builder.

## 🚀 Fonctionnalités

- ⏰ **Minuteur en temps réel** - Compte à rebours dynamique avec mise à jour en direct
- 🎨 **Entièrement personnalisable** - Couleurs, polices, bordures et styles configurables
- 📱 **Design responsive** - Optimisé pour tous les appareils et tailles d'écran
- 🔧 **Interface intuitive** - Sélecteur de date et heure intégré dans Breakdance
- 🛡️ **Sécurisé** - Protection XSS et validation des entrées
- ⚡ **Performance optimisée** - Code JavaScript optimisé sans manipulation DOM excessive
- 🔄 **Mise à jour en temps réel** - Changements instantanés lors de l'édition

## 📋 Prérequis

- WordPress 5.0 ou supérieur
- Breakdance Builder (plugin requis)
- PHP 7.4 ou supérieur

## 📦 Installation

1. **Téléchargement**
   ```bash
   git clone https://github.com/brandonviry/breakdance-timer.git
   ```

2. **Installation manuelle**
   - Téléchargez le plugin
   - Uploadez le dossier `breakdance-timer` dans `/wp-content/plugins/`
   - Activez le plugin dans l'administration WordPress

3. **Via l'administration WordPress**
   - Allez dans `Extensions > Ajouter`
   - Uploadez le fichier ZIP du plugin
   - Activez le plugin

## 🎯 Utilisation

### Dans Breakdance Builder

1. **Ajouter l'élément**
   - Ouvrez Breakdance Builder
   - Recherchez "Timer" dans les éléments
   - Glissez-déposez l'élément sur votre page

2. **Configuration**
   - **Date** : Sélectionnez la date cible
   - **Heure** : Définissez l'heure précise
   - **Design** : Personnalisez l'apparence

3. **Personnalisation du design**
   - **Couleurs** : Arrière-plan, cartes, texte
   - **Typographie** : Police, taille, poids
   - **Bordures** : Style, rayon, couleur
   -  ...

### Exemple de configuration

```
Date cible : 31/12/2024
Heure : 23h59
Affichage : JOURS | HEURES | MINUTES | SECONDES
```

## 🏗️ Structure du projet

```
breakdance-timer/
├── plugin.php                 # Fichier principal du plugin
├── elements/
│   └── Timer/
│       ├── element.php         # Classe PHP de l'élément
│       ├── html.twig          # Template HTML
│       ├── css.twig           # Styles CSS
│       └── default.css        # Styles par défaut
└── README.md                  # Documentation
```

## 🔧 Développement

### Architecture

- **Backend** : PHP avec classes Breakdance
- **Frontend** : JavaScript vanilla avec MutationObserver
- **Templates** : Twig pour HTML et CSS
- **Sécurité** : Validation stricte et échappement XSS

### Fonctionnalités techniques

- **Validation de date** : Format strict `dd/mm/yyyy - HHhMM`
- **Observer Pattern** : Détection automatique des changements
- **Gestion d'erreurs** : Messages d'erreur sécurisés
- **Performance** : Timers optimisés avec `setTimeout`


## 🐛 Dépannage

### Problèmes courants

**Le minuteur ne s'affiche pas**
- Vérifiez que Breakdance est activé
- Contrôlez la date/heure configurée
- Vérifiez la console pour les erreurs JavaScript

**Format de date invalide**
- Utilisez le format : `dd/mm/yyyy - HHhMM`
- Exemple : `25/12/2024 - 15h30`

**Styles non appliqués**
- Videz le cache de Breakdance
- Régénérez les CSS dans Breakdance

## 📝 Changelog

### Version 0.0.1
- ✨ Version initiale
- ⏰ Minuteur en temps réel
- 🎨 Interface de personnalisation
- 📱 Design responsive
- 🛡️ Sécurité XSS

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créez une branche (`git checkout -b feature/nouvelle-fonctionnalite`)
3. Committez vos changements (`git commit -m 'Ajout nouvelle fonctionnalité'`)
4. Push vers la branche (`git push origin feature/nouvelle-fonctionnalite`)
5. Ouvrez une Pull Request

## 👨‍💻 Auteur

**VIRY Brandon**
- GitHub: [@brandonviry](https://github.com/brandonviry)

## 📄 Licence

Ce projet n'est sous aucune licence spécifique (Unlicensed).

## 🙏 Remerciements

- Équipe Breakdance pour leur excellent builder

---

<div align="center">
  <strong>Fait avec ❤️ pour la communauté WordPress</strong>
</div>
