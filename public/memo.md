# Mémoire d'Éco-conception Web

**Étudiant :** SAUVAL Nyl  
**Formation :** BUT 3 Informatique (Parcours APP)  
**Année :** 2025-2026  
**Institution :** IUT de Lens

---

## 1. L'Intérêt de Next.js pour un site éco-responsable

Dans une **démarche scientifique** (mesure et documentation de mes choix techniques) visant la **sobriété dimensionnelle et d'usage**, le choix de Next.js se justifie par les aspects suivants :

1.  **Génération de Sites Statiques (SSG) / Export statique :** En utilisant `output: 'export'`, j'ai configuré le projet pour que les pages soient pré-rendues à la compilation. Cela réduit drastiquement la consommation des serveurs (pas de calcul côté serveur à chaque requête), favorisant une **efficacité de gestion** via une infrastructure minimale.
2.  **Minification et Code Splitting par défaut :** Next.js divise intelligemment le code JavaScript pour ne charger que ce qui est strictement nécessaire à la page affichée. J'applique ainsi le principe de **sobriété d'usage** : une utilisation limitée aux besoins réels pour réduire le volume de données transféré.
3.  **Hébergement en périphérie (Edge / CDN comme GitHub Pages) :** Ce site statique s'héberge facilement sur des CDN. Cela rapproche la donnée de l'utilisateur final et réduit le nombre de rebonds réseaux, diminuant de facto l'empreinte carbone liée à la transmission.
4.  **Optimisation native (Google Fonts & Scripts) :** J'utilise les capacités du framework pour supprimer les requêtes réseau superflues, ce qui libère au plus vite les ressources de l'utilisateur (**Efficacité d'usage**).

---

## 2. Bonnes pratiques mises en œuvre dans le cadre de ce site CV

En adoptant une **approche holistique** de l'IT éco-responsable pour minimiser mon impact environnemental, j'ai implémenté les pratiques suivantes :

* **Sobriété d'adaptation avec Tailwind CSS :** Bien que j'utilise Tailwind pour un design moderne, j'ai configuré PostCSS pour purger drastiquement le CSS. Mon application finale ne charge que les classes strictement utilisées, évitant le téléchargement de code inutile.
* **Design UI Minimaliste & Accessibilité :** J'ai choisi un thème vert sauge avec de forts contrastes pour lutter contre l'**illectronisme**. J'ai également développé mon propre **Mode Sombre** (Dark Mode) en React, sans librairie externe lourde, afin de réduire la consommation énergétique sur les écrans OLED.
* **Polices Systèmes Uniquement :** Au lieu de solliciter Google Fonts (impactant la **vie privée**), j'exploite les polices `system-ui, -apple-system, sans-serif`. Cela m'évite de faire télécharger plusieurs centaines de kilo-octets de polices à mes visiteurs.
* **Hébergement sans base de données (Efficacité de Conception) :** En adoptant une architecture "Serverless", je limite l'exposition aux défaillances et réduis le nombre de serveurs tournant en permanence pour mon site.
* **DOM Sémantique Allégé :** J'utilise rigoureusement les balises sémantiques HTML5 (`<main>`, `<header>`, `<article>`, `<section>`). Mon interface est ainsi rapide à parser pour le navigateur et parfaitement accessible aux lecteurs d'écrans, garantissant un accès universel sans contrainte d'**équipement** récent.
