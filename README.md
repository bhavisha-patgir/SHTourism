# SHTourism
<p align="center">
  <img src="public/icon.svg" alt="Heritage Explorer Logo" width="80" height="80" />
</p>

<h1 align="center">🏛️ Heritage Explorer — Smart Heritage Tourism Platform</h1>

<p align="center">
  <em>Discover, explore, and experience India's rich cultural heritage through immersive virtual tours, interactive maps, smart trip planning, and AI-powered insights.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-16-black?logo=next.js" alt="Next.js" />
  <img src="https://img.shields.io/badge/React-19-61dafb?logo=react" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-5.7-3178c6?logo=typescript" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-4-06b6d4?logo=tailwindcss" alt="Tailwind" />
  <img src="https://img.shields.io/badge/Three.js-r183-black?logo=three.js" alt="Three.js" />
  <img src="https://img.shields.io/badge/License-MIT-green" alt="License" />
</p>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [Pages & Modules](#-pages--modules)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Backend (Laravel API Snippets)](#-backend-laravel-api-snippets)
- [Deployment](#-deployment)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌍 Overview

**Heritage Explorer** is a modern, full-featured heritage tourism web application focused on **Gujarat and Rajasthan's** cultural landmarks. It combines cutting-edge web technologies — including a **3D interactive globe**, **360° virtual tours**, **AI chatbot**, and **crowd prediction analytics** — to deliver a premium digital tourism experience.

The platform helps tourists and heritage enthusiasts:
- **Discover** heritage sites, monuments, temples, and palaces
- **Explore** sites virtually through 360° panoramic viewers
- **Plan** optimized multi-stop trips with interactive route maps
- **Predict** crowd levels to find the best visiting times
- **Attend** cultural events, festivals, and heritage walks

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🌐 **3D Interactive Globe** | Explore heritage sites on a rotating 3D globe with fly-to animations, built with Three.js & react-globe.gl |
| 🗺️ **Dual Map Views** | Switch between a 3D globe and a detailed 2D Leaflet/Google Maps view with markers and popups |
| 🔄 **360° Virtual Tours** | Immersive panoramic tours using Photo Sphere Viewer with auto-rotate and gallery plugins |
| 🤖 **AI Heritage Chatbot** | Floating chatbot assistant to answer questions about heritage places, tickets, and directions |
| 📊 **Crowd Prediction** | Hourly/daily crowd level predictions with interactive Recharts visualizations |
| 🧳 **Smart Trip Planner** | Select multiple heritage sites, get optimized routes, explore in 360°, and view Google Maps directions |
| 🎭 **Events & Festivals** | Browse upcoming cultural events filtered by state (Gujarat/Rajasthan) and month, with calendar views |
| 🖼️ **Heritage Gallery** | Curated image gallery of heritage sites with detailed historical information |
| 🌙 **Dark/Light Theme** | Full theme support via next-themes |
| 📱 **Fully Responsive** | Optimized for mobile, tablet, and desktop viewports |
| ⚡ **Vercel Analytics** | Built-in performance and visitor analytics |

---

## 📄 Pages & Modules

### 🏠 Home Page (`/`)
- **Hero Section** — Animated hero banner with call-to-action
- **Featured Places** — Showcase of top heritage destinations
- **Upcoming Events** — Preview of upcoming festivals and heritage walks
- **CTA Section** — Engagement section to explore virtual tours

### 🏛️ Heritage Sites (`/heritage/[id]`)
- Dynamic heritage site detail pages
- Site history, architecture details, visiting information
- Image galleries and crowd prediction charts per site

### 🗺️ Interactive Map (`/map`)
- **Globe View** — 3D globe with heritage markers and fly-to animations
- **Map View** — 2D interactive Leaflet map with detailed markers and popups
- Sidebar with site list, search and filtering
- Seamless toggle between globe and map modes

### 🔄 Virtual Tours (`/virtual-tour`)
- Heritage image gallery with category filtering
- 360° panoramic viewer for immersive site exploration
- Auto-rotate and gallery plugin support

### 🧳 Trip Planner (`/trip-planner`)
- Multi-stop trip builder with place selection
- AI-optimized route suggestions
- 360° exploration for each stop
- Interactive route map powered by Google Maps/Leaflet
- Smart feature pills: Route Optimization, 360° Exploration, Google Maps, Smart Suggestions

### 📊 Crowd Prediction (`/crowd-prediction`)
- Site-by-site crowd level dashboard
- Hourly and daily predictions with time-series charts
- Recommendation engine for best visiting hours
- Built with Recharts for smooth, interactive data visualization

### 🎭 Events (`/events` & `/events/[id]`)
- Cultural events listing — festivals, heritage walks, light & sound shows
- Filter by state (Gujarat / Rajasthan) and month
- Calendar view component
- Individual event detail pages

### 🖼️ Gallery (`/gallery/[id]`)
- Heritage site photo galleries with historical context

### 🤖 AI Chatbot (Global)
- Floating chat widget on every page
- Answers heritage-related queries (places, tickets, directions, visit tips)
- Typing animation with message timestamps

### 🔌 API Routes (`/api`)
- `GET /api/places` — Heritage sites data
- `GET /api/events` — Cultural events data with filtering support

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| [Next.js 16](https://nextjs.org/) | React framework with App Router, SSR, and API routes |
| [React 19](https://react.dev/) | UI library with latest features |
| [TypeScript 5.7](https://www.typescriptlang.org/) | Type-safe development |
| [Tailwind CSS 4](https://tailwindcss.com/) | Utility-first CSS framework |
| [Radix UI](https://www.radix-ui.com/) | Accessible, unstyled UI primitives |
| [Lucide React](https://lucide.dev/) | Modern icon library |

### Maps & 3D
| Technology | Purpose |
|---|---|
| [Three.js](https://threejs.org/) | 3D rendering engine for the globe |
| [react-globe.gl](https://github.com/vasturiano/react-globe.gl) | React wrapper for 3D globe visualization |
| [Leaflet](https://leafletjs.com/) + [React Leaflet](https://react-leaflet.js.org/) | Open-source interactive 2D maps |
| [Google Maps API](https://developers.google.com/maps) | Route directions & additional mapping |

### Virtual Tours
| Technology | Purpose |
|---|---|
| [Photo Sphere Viewer](https://photo-sphere-viewer.js.org/) | 360° panoramic image viewer |
| Auto-rotate Plugin | Automatic panorama rotation |
| Gallery Plugin | Multi-image panorama galleries |

### Data & Analytics
| Technology | Purpose |
|---|---|
| [Recharts](https://recharts.org/) | Crowd prediction charts and analytics |
| [Vercel Analytics](https://vercel.com/analytics) | Visitor and performance tracking |

### Forms & Validation
| Technology | Purpose |
|---|---|
| [React Hook Form](https://react-hook-form.com/) | Performant form handling |
| [Zod](https://zod.dev/) | Schema validation |

### Backend (Snippets)
| Technology | Purpose |
|---|---|
| [Laravel](https://laravel.com/) | PHP backend framework (snippets included) |
| Event Model + Seeder | Gujarat/Rajasthan events (March–June 2026) |
| EventController | `GET /api/events` with filtering and sorting |

---

## 📁 Project Structure

```
smart-heritage-UI/
├── app/                          # Next.js App Router pages
│   ├── page.tsx                  # Home page
│   ├── layout.tsx                # Root layout (Navbar, Footer, Chatbot)
│   ├── globals.css               # Global styles & Tailwind config
│   ├── api/                      # API routes
│   │   ├── events/               # Events endpoint
│   │   └── places/               # Places endpoint
│   ├── heritage/[id]/            # Dynamic heritage site pages
│   ├── map/                      # Interactive map page
│   ├── virtual-tour/             # Virtual tour gallery
│   ├── trip-planner/             # Smart trip planner
│   ├── crowd-prediction/         # Crowd predictions dashboard
│   ├── events/                   # Events listing & detail
│   │   └── [id]/                 # Individual event page
│   └── gallery/[id]/             # Gallery detail pages
│
├── components/                   # Reusable React components
│   ├── navbar.tsx                # Navigation bar
│   ├── footer.tsx                # Site footer
│   ├── chatbot.tsx               # AI chatbot widget
│   ├── theme-provider.tsx        # Dark/Light theme provider
│   ├── home/                     # Home page sections
│   │   ├── hero-section.tsx
│   │   ├── featured-places.tsx
│   │   ├── upcoming-events.tsx
│   │   └── cta-section.tsx
│   ├── map/                      # Map components
│   │   ├── interactive-map.tsx
│   │   ├── globe-map-content.tsx
│   │   └── leaflet-map-content.tsx
│   ├── heritage/                 # Heritage site components
│   │   ├── crowd-prediction-chart.tsx
│   │   └── image-gallery.tsx
│   ├── virtual-tour/             # Virtual tour components
│   │   ├── image-gallery.tsx
│   │   ├── panoramic-viewer.tsx
│   │   ├── virtual-tour-viewer.tsx
│   │   ├── tour-gallery.tsx
│   │   └── pano-viewer-trigger.tsx
│   ├── trip-planner/             # Trip planner components
│   │   ├── trip-planner.tsx
│   │   ├── place-card.tsx
│   │   ├── route-map.tsx
│   │   ├── panorama-viewer.tsx
│   │   ├── viewer-360-modal.tsx
│   │   ├── leaflet-route-map-content.tsx
│   │   └── photo-sphere-viewer.tsx
│   ├── crowd/                    # Crowd prediction components
│   │   └── crowd-dashboard.tsx
│   ├── events/                   # Events components
│   │   ├── upcoming-events.tsx
│   │   └── events-calendar.tsx
│   └── ui/                       # Radix UI primitives (shadcn/ui)
│
├── hooks/                        # Custom React hooks
├── lib/                          # Utility functions
├── public/                       # Static assets & icons
│   └── images/                   # Heritage site images
├── images/                       # Additional image assets
├── styles/                       # Additional stylesheets
├── laravel-backend-snippets/     # Laravel API backend snippets
│   ├── app/                      # Models & Controllers
│   ├── database/                 # Migrations & Seeders
│   └── routes/                   # API route definitions
│
├── next.config.mjs               # Next.js configuration
├── tsconfig.json                 # TypeScript configuration
├── package.json                  # Dependencies & scripts
├── postcss.config.mjs            # PostCSS configuration
└── components.json               # shadcn/ui configuration
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** ≥ 18.x
- **npm** or **pnpm**

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/smart-heritage-UI.git
   cd smart-heritage-UI
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   pnpm install
   ```

3. **Set up environment variables** (see [Environment Variables](#-environment-variables))

4. **Start the development server**
   ```bash
   npm run dev
   ```

5. **Open in browser**
   ```
   http://localhost:3000
   ```

### Build for Production

```bash
npm run build
npm start
```

---

## 🔐 Environment Variables

Create a `.env.local` file in the project root:

```env
# Google Maps API Key (for trip planner route maps)
NEXT_PUBLIC_GOOGLE_MAPS_API_KEY=your_google_maps_api_key

# Google Gemini AI Key (for chatbot - optional)
NEXT_PUBLIC_GEMINI_API_KEY=your_gemini_api_key
```

> **Note:** The application will work without these keys, but the Google Maps route functionality and AI chatbot will be limited.

---

## 🔧 Backend (Laravel API Snippets)

The `laravel-backend-snippets/` directory contains copy-paste ready Laravel files for an events API:

| Component | Description |
|---|---|
| **Event Model** | Eloquent model with migration |
| **EventSeeder** | Pre-populated with Gujarat & Rajasthan events (March–June 2026) |
| **EventController** | `GET /api/events` endpoint |

### Supported Query Parameters

| Parameter | Values | Description |
|---|---|---|
| `state` | `Gujarat` \| `Rajasthan` | Filter by state |
| `month` | `1`–`12` | Filter by month |
| `upcoming` | `0` \| `1` (default: `1`) | Show only upcoming events |
| `sort` | `nearest` (default) \| `startDate` | Sort order |
| `id` | Event ID | Fetch a specific event |

---

## 🌐 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Import the repository on [Vercel](https://vercel.com)
3. Add environment variables in the Vercel dashboard
4. Deploy — Vercel will auto-detect Next.js settings

### Other Platforms

The app can be deployed on any platform that supports Next.js:
- **Netlify** — with the Next.js adapter
- **AWS Amplify** — with SSR support
- **Docker** — using the official Next.js Docker example
- **Self-hosted** — `npm run build && npm start`

---

## 📸 Screenshots

> _Add screenshots of your application here after deployment:_

| Page | Preview |
|---|---|
| Home | _screenshot_ |
| Interactive Globe | _screenshot_ |
| Heritage Detail | _screenshot_ |
| Virtual Tour 360° | _screenshot_ |
| Trip Planner | _screenshot_ |
| Crowd Prediction | _screenshot_ |
| Events Calendar | _screenshot_ |

---

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. **Fork** the repository
2. **Create** a feature branch: `git checkout -b feature/amazing-feature`
3. **Commit** your changes: `git commit -m "Add amazing feature"`
4. **Push** to the branch: `git push origin feature/amazing-feature`
5. **Open** a Pull Request

### Development Guidelines
- Follow the existing code style and component patterns
- Use TypeScript for all new files
- Use Radix UI primitives for new UI components
- Write semantic, accessible HTML
- Ensure responsive design across all viewports

---

## 📝 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<p align="center">
  Made with ❤️ for preserving and promoting cultural heritage
</p>
