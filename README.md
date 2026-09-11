# nuxt-app — Squelette Nuxt 3 « tout équipé »

![Nuxt](https://img.shields.io/badge/Nuxt-3-00DC82?logo=nuxt.js&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?logo=tailwindcss&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Statut](https://img.shields.io/badge/Statut-Squelette-lightgrey)

📦 **Code source** : <https://github.com/Georginio-prod/nuxt-app>

---

## 📌 Présentation

Squelette **Nuxt 3** créé en mai 2025 pour tester la nouvelle génération de modules
officiels Nuxt avec **Tailwind CSS v4**. Il contient une page d'accueil minimale et sert
de terrain d'expérimentation / base de démarrage.

## 🛠️ Modules configurés

| Module | Rôle |
|---|---|
| `@nuxt/ui` | Bibliothèque de composants |
| `@nuxt/content` | Contenu Markdown / CMS fichier |
| `@nuxt/fonts` | Chargement optimisé des polices |
| `@nuxt/icon` | Icônes (Iconify) |
| `@nuxt/image` | Images optimisées |
| `@nuxt/scripts` | Scripts tiers |
| `@nuxt/eslint` | Lint |
| `@nuxt/test-utils` | Tests |

Tailwind v4 est branché via le plugin Vite `@tailwindcss/vite` dans `nuxt.config.ts`.

## 📁 Structure

```
nuxt-app/
├── nuxt.config.ts        # Modules + plugin Tailwind
├── app.vue               # Page d'accueil
├── eslint.config.mjs
├── public/               # favicon, robots.txt
└── server/               # Dossier serveur Nitro (vide)
```

## 🚀 Utilisation

```bash
git clone https://github.com/Georginio-prod/nuxt-app.git
cd nuxt-app
npm install
npm run dev        # http://localhost:3000
```

`npm run build` / `npm run generate` / `npm run preview` sont disponibles comme sur tout projet Nuxt.

## 🌐 Déploiement

Non déployé (squelette sans contenu).

---

## 👤 Auteur

**Komla Etonam Georges EKLOU** (Georginio) — Développeur Full Stack Web & Web3

[![GitHub](https://img.shields.io/badge/GitHub-Georginio--prod-181717?logo=github)](https://github.com/Georginio-prod)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profil-0A66C2?logo=linkedin)](https://www.linkedin.com/in/komla-etonam-georges-eklou-68518b23b)
[![Portfolio](https://img.shields.io/badge/Portfolio-georginio.w3frame.com-6C63FF)](https://georginio.w3frame.com/)

> 📚 Tous mes projets sont listés et documentés sur mon [profil GitHub](https://github.com/Georginio-prod).
