# 🍽️ Gemutly

Discover and order homemade meals from talented local chefs — or become a chef and share your culinary passion.

Gemutly is an Uber-style marketplace for food, connecting diners with local home chefs. It features a modern, responsive design, multilingual support, and full authentication powered by the Base44 platform. Built to be investor-ready and user-friendly, Gemutly is a production-grade React + Tailwind application.

🔗 **Live Demo:** [gemutly.base44.app](https://gemutly.base44.app/)
📂 **Repository:** [github.com/rkazumovi/gemutly-app](https://github.com/rkazumovi/gemutly-app)

![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS%20v4-38B2AC?logo=tailwindcss&logoColor=white)
![Base44](https://img.shields.io/badge/Platform-Base44-orange)

---

## Overview

Gemutly connects diners with local home chefs through a marketplace experience: browsing chef profiles and menus, ordering meals, and — for chefs — an onboarding flow to register and start selling. The app is built with internationalization and RTL support in mind from the ground up, and includes a scaffolded payments layer via Stripe Connect for future chef payouts.

## ✨ Features

- 🎬 Hero section with a full-screen video background and call-to-action buttons
- 🍜 Diner features carousel — interactive cards highlighting app benefits
- 👨‍🍳 Chef marketplace — explore local chefs, view profiles, and order meals
- 📄 Dynamic, SEO-friendly chef profile pages with menu items
- 📝 "Become a Chef" onboarding flow for registering as a home chef
- 🔐 Built-in authentication (login/register) via Base44 Auth
- 🌍 Internationalization — 10 supported languages, including RTL support for Arabic
- 📱 Mobile-first responsive layout optimized for all devices
- 🌓 Dark/light mode theme switching

## 🛠️ Built With

**Languages**
- TypeScript — type-safe application and component logic
- CSS — styling via Tailwind CSS

**Frameworks / Platform**
- [React](https://react.dev/) — UI library
- [Base44](https://base44.com/) — application platform providing authentication, hosting, and backend infrastructure
- [Tailwind CSS v4](https://tailwindcss.com/) — utility-first styling and responsive layouts
- [next-themes](https://github.com/pacocoursey/next-themes) — dark/light mode theme management

**Payments**
- [Stripe Connect](https://stripe.com/connect) (scaffolded) — platform-ready payment flow between chefs and diners

**Typography**
- [Geist](https://vercel.com/font) — primary font family

## 📁 Project Structure

```
src/
├── app/
│   ├── layout.tsx              # Root layout
│   ├── page.tsx                # Home page
│   ├── explore/page.tsx        # Diner marketplace
│   ├── become-chef/page.tsx    # Chef onboarding
│   └── [chef]/[slug]/page.tsx  # Dynamic chef profiles
├── components/
│   ├── Navbar.tsx
│   ├── Footer.tsx
│   ├── HeroVideo.tsx
│   ├── DinerFeatureCarousel.tsx
│   ├── ChefCard.tsx
│   └── MenuItemCard.tsx
├── lib/
│   ├── stripe.ts
│   └── data.ts                 # Mock chef/menu data
├── messages/
│   ├── en.json
│   ├── es.json
│   └── ...                     # Additional language JSONs
└── globals.css
```

## 🚀 Getting Started

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/rkazumovi/gemutly-app.git
   cd gemutly-app
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Run the development server
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

## 🎨 Customization

- **Hero Video** — update the `src` attribute in `HeroVideo.tsx` to change the background video
- **Colors** — Tailwind color palette:
  - Primary: Orange (`orange-500`, `orange-600`)
  - Accents: Green (`#22c55e`) and Orange (`#f97316`)
  - Text: Slate (`slate-100`, `slate-700`)
- **Content** — edit text in `page.tsx`, `DinerFeatureCarousel.tsx`, and the chef profile pages
- **Languages** — add or edit translations in `messages/*.json`

## 📦 Deployment

Gemutly is deployed as a static React app on the **Base44** platform and is live at:
👉 [gemutly.base44.app](https://gemutly.base44.app/)

It can also be deployed to any platform that supports Base44-built apps, with Vercel or Netlify recommended as alternatives.

## 📄 License

This project is for demonstration purposes and is licensed under the MIT License.
