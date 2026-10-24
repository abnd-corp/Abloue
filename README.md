# Abloue

Application web de visualisation et gestion de données géographiques par département français.

**Exemple d'utilisation :** Cette application est actuellement configurée pour afficher des loueurs de matériel, mais elle peut être facilement adaptée pour tout type de données nécessitant une visualisation géographique par département (commerces, services, professionnels, événements, etc.).

## 🌐 Démo en ligne

[https://abnd-corp.github.io/Abloue/abloue.html](https://abnd-corp.github.io/Abloue/abloue.html)

## 📄 Licences

Ce projet utilise deux licences différentes pour des composants distincts :

- **Code de l'application** (JavaScript, CSS, structure HTML) : [MIT License](LICENSE) © 2025 Hugo Lagouardat & Rudy Alves
- **Carte SVG de France** (incluse dans `abloue.html`) : [Creative Commons Attribution 4.0 International (CC BY 4.0)](http://creativecommons.org/licenses/by/4.0/) © Régis Enguehard

Ces deux licences sont compatibles et permettent une utilisation libre du projet. Voir le fichier [LICENSE](LICENSE) pour les détails complets de la licence MIT.

## ✨ Caractéristiques principales

- **Fonctionnement autonome** : L'application peut fonctionner **sans serveur web** - il suffit d'ouvrir le fichier `abloue.html` directement dans un navigateur (compatible également avec un serveur web si nécessaire)
- **Client-side uniquement** : Toutes les données et la logique sont côté client (HTML, CSS, JavaScript)
- **Personnalisable** : Structure modulaire facile à adapter pour vos propres données

## 🎯 Fonctionnalités

- **Carte interactive de France** avec départements cliquables
- **Système de filtrage** par nom et département
- **Affichage en cartes** avec informations détaillées
- **Interface responsive** avec visualisation claire des données
- **Données personnalisables** : adaptez facilement le contenu à vos besoins (actuellement configuré pour des loueurs de matériel en exemple)

## 🚀 Installation et utilisation

**Aucune installation requise !** L'application fonctionne sans serveur web, mais peut aussi être hébergée sur un serveur.

### Utilisation locale (sans serveur)

1. Clonez le dépôt :
```bash
git clone https://github.com/hugolagouardat/Abloue.git
cd Abloue
```

2. Ouvrez simplement `abloue.html` dans votre navigateur web (double-clic sur le fichier ou clic droit > Ouvrir avec > Navigateur)

### Utilisation avec serveur web (optionnel)

L'application est également compatible avec tout serveur web (Apache, Nginx, serveur de développement, etc.). Il suffit de placer les fichiers dans le répertoire du serveur.

Aucune dépendance backend n'est nécessaire - l'application fonctionne entièrement côté client.

## 📁 Structure du projet

```
Abloue/
├── abloue.html          # Page principale
├── css/                 # Styles CSS
│   ├── abloue.css
│   ├── card.css
│   ├── carte.css
│   ├── filtre.css
│   ├── formulaire.css
│   └── modal.css
├── js/                  # Scripts JavaScript
│   ├── abloue.js        # Logique principale
│   ├── card.js          # Gestion des cartes
│   ├── filtre.js        # Système de filtrage
│   ├── modal.js
│   └── jquery.js
└── data/                # Données
    ├── departements.js  # Mapping départements
    └── loueurs.js       # Base de données loueurs
```

## 🗺️ À propos de la carte

La carte interactive de France utilisée dans cette application est **Abcarte**, une modification de la [carte-france-svg](https://github.com/regisenguehard/carte-france-svg) de Régis Enguehard avec ajout des numéros de département.

- **Carte originale** : [carte-france-svg](https://github.com/regisenguehard/carte-france-svg) © Régis Enguehard
- **Licence** : [Creative Commons Attribution 4.0 International (CC BY 4.0)](http://creativecommons.org/licenses/by/4.0/)
- **Modifications** : Ajout des numéros de département pour créer Abcarte

Dépôt Abcarte : [github.com/abnd-corp/Abcarte](https://github.com/abnd-corp/Abcarte)

## 🛠️ Technologies utilisées

- HTML5
- CSS3
- JavaScript (ES6+)
- jQuery 3.x
- SVG pour la carte interactive

## 👤 Auteur

**Rudy Alves** - [@Rxdy](https://github.com/Rxdy)
**Hugo Lagouardat** - [@hugolagouardat](https://github.com/hugolagouardat)

## 🙏 Remerciements

- [abnd-corp](https://github.com/abnd-corp) pour Abcarte
- [Régis Enguehard](https://github.com/regisenguehard) pour la carte SVG de France
