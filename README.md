# 🛍️ dsk-shop – Premium E-Commerce Platform (Lomé, Togo)

[![React](https://img.shields.io/badge/Framework-React%2018-blue?style=flat-sharp&logo=react)](https://react.dev/)
[![CSS Modules](https://img.shields.io/badge/Styles-CSS%20Modules-black?style=flat-sharp&logo=css3)](https://github.com/css-modules/css-modules)
[![Supabase](https://img.shields.io/badge/Backend-Supabase-green?style=flat-sharp&logo=supabase)](https://supabase.com/)
[![License](https://img.shields.io/badge/License-MIT-orange?style=flat-sharp)](LICENSE)

**dsk-shop** est une application web e-commerce premium à l'interface moderne (UI/UX fluide, visuels 3D, typographies audacieuses) entièrement optimisée pour le marché de **Lomé au Togo**. L'application combine les standards esthétiques internationaux et les réalités fonctionnelles de l'écosystème togolais.

---
 
## ✨ Fonctionnalités Majeures

### 💻 Interface & Expérience Utilisateur (UI/UX)
* **Design Premium Asymétrique :** Typographies haut de gamme (`Syne` pour les titres et `Plus Jakarta Sans` pour le texte courant) et palette de couleurs stricte.
* **Header Multi-Fonctions Intelligent :**
  * **Top Bar dynamique :** Masquable (via une croix) avec défilement horizontal infini (`marquee`) sur mobile.
  * **Mega Menu Grid (Desktop) :** Affichage asymétrique complet des catégories au survol.
  * **Accordéon Tactile (Mobile) :** Navigation à tiroir compacte et extensible.
* **Hero Section Responsive 3D :** Mise en page optimisée valorisant des rendus d'accessoires en lévitation tridimensionnelle.

### 🇹🇬 Localisation & Optimisations Togo
* **Gestion Monétaire :** Intégration complète des prix affichés en **Francs CFA (F CFA)**.
* **Système de Paiement Hybride :** Pré-configuration pour les paiements mobiles locaux (**T-Money**, **Flooz**) et le paiement en espèces à la livraison.
* **Logistique Urbaine :** Prise en compte de la livraison express par quartiers de Lomé (Assivito, Hédzranawoé, Agoè, Nyékonakpoé, Baguida, etc.).

---

## 🎨 Charte Graphique Strict

Le projet respecte scrupuleusement la configuration des variables CSS suivantes :

| Variable | Teinte / Rôle | Code Hexadécimal |
| :--- | :--- | :--- |
| `--color-shop-blue` | Bleu Premium (Identité) | `#10367D` |
| `--color-promo-orange` | Orange Flash (Promotions & CTAs) | `#ff5a36` |
| `--color-shop-gray` | Gris Arrière-plan (Bases) | `#f3f4f6` |
| `--color-border` | Gris Bordure Épuré | `#f3f4f6` |
| Textes Principaux | Noir Pur | `#000000` |
| Textes Alternatifs | Blanc Pur | `#ffffff` |

---

## 🏗️ Architecture du Projet

Le projet utilise une structure modulaire stricte, isolant les styles via les **CSS Modules** pour éviter toute collision globale :

```text
├── public/
│   └── assets/               # Images 3D, logos et icônes
├── src/
│   ├── components/           # Composants isolés et réutilisables
│   │   ├── Navbar/
│   │   │   ├── Navbar.tsx
│   │   │   └── Navbar.module.css
│   │   └── Hero/
│   │       ├── Hero.tsx
│   │       └── Hero.module.css
│   ├── context/              # Contextes globaux (Panier, Auth)
│   ├── styles/
│   │   └── index.css         # Variables injectées (:root) et resets globaux
│   ├── App.tsx               # Point d'entrée de l'application
│   └── main.tsx
├── package.json
└── vite.config.ts
