Gemutly

Discover and order homemade meals from talented local chefs — or become a chef and share your culinary passion!

Gemutly is an Uber-style marketplace for food, connecting diners with local home chefs. It features a modern, responsive design, multilingual support, and full authentication powered by the Base44 platform. Built to be investor-ready and user-friendly, Gemutly is a production-grade React + Tailwind app.

Features

• Hero Section – Full-screen video background with call-to-action buttons.

• Diner Features Carousel – Interactive cards highlighting app benefits.

• Chef Marketplace – Explore local chefs, view profiles, and order meals.

• Chef Profile Pages – Dynamic, SEO-friendly profiles with menu items.

• Become a Chef – Onboarding page to register as a home chef.

• Authentication – Built-in Base44 login/register system.

• Internationalization – Supports 10 languages, including RTL for Arabic.

• Responsive Design – Mobile-first layout optimized for all devices.

• Dark/Light Mode – Smooth theme switching using next-themes.

Tech Stack

• React + Base44 – Frontend framework and platform for authentication.

• Tailwind CSS v4 – Styling and responsive layouts.

• TypeScript – Type-safe development.

• Base44 Auth – Email/password login, session management, and user accounts.

• Next-Themes – Dark/light mode support.

• Geist Font – Clean and modern typography.

• Stripe Connect (Scaffolded) – Platform-ready payment flow between chefs and diners.

Project Structure
src/
├── app/
│   ├── layout.tsx          # Root layout
│   ├── page.tsx            # Home page
│   ├── explore/page.tsx    # Diner marketplace
│   ├── become-chef/page.tsx # Chef onboarding
│   └── [chef]/[slug]/page.tsx # Dynamic chef profiles
├── components/
│   ├── Navbar.tsx
│   ├── Footer.tsx
│   ├── HeroVideo.tsx
│   ├── DinerFeatureCarousel.tsx
│   ├── ChefCard.tsx
│   ├── MenuItemCard.tsx
├── lib/
│   ├── stripe.ts
│   └── data.ts              # Mock chef/menu data
├── messages/
│   ├── en.json
│   ├── es.json
│   └── ...                  # Other language JSONs
└── globals.css
Getting Started

Clone the repository:

git clone https://github.com/yourusername/gemutly-app.git
cd gemutly-app

Install dependencies:

npm install

Run the development server:

npm run dev

Open http://localhost:3000
 in your browser.

Customization

• Hero Video: Update HeroVideo.tsx src attribute to change the video.

• Colors: Tailwind CSS color palette uses:

  • Primary: Orange (orange-500, orange-600)

  • Accents: Green (#22c55e) and Orange (#f97316)

  • Text: Slate (slate-100, slate-700)

• Content: Edit text in page.tsx, DinerFeatureCarousel.tsx, and chef pages.

• Languages: Add translations in messages/*.json.

Deployment

• Deploy as a static React app on any platform supporting Base44 apps.

• Recommended: Base44 hosting, Vercel, or Netlify.

License

This project is for demonstration purposes and is licensed under the MIT License.
