# Easy-Telkie-connect-app
A web app that helps Telkom customers visualize network coverage, detect roaming, view recommended data bundles, and manage mobile plans. Features include location detection, real-time coverage strength alerts, bundle purchase actions, and a mobile-first interface with navigation.

FILE STRUCTURE
telkom-coverage-app/
├─ public/                  # Static files (logo, icons, images, favicon)
│   ├─ telkom-logo.png
│   └─ icons/
│       ├─ home.svg
│       ├─ bell.svg
│       └─ plans.svg
│
├─ src/
│   ├─ app/                 # App Router (routes & layouts)
│   │   ├─ layout.tsx       # Global layout (header, nav, etc.)
│   │   ├─ page.tsx         # Homepage
│   │   ├─ bundles/
│   │   │   └─ page.tsx     # Bundles page
│   │   ├─ notifications/
│   │   │   └─ page.tsx     # Notifications page
│   │   ├─ plans/
│   │   │   └─ page.tsx     # Plans page
│   │   └─ api/             # Next.js API routes
│   │       ├─ coverage/
│   │       │   └─ route.ts # Example API for coverage data
│   │       └─ bundles/
│   │           └─ route.ts # Example API for bundles
│   │
│   ├─ components/          # Reusable UI components
│   │   ├─ ui/              # Base UI elements (buttons, cards, etc.)
│   │   │   ├─ Button.tsx
│   │   │   ├─ Card.tsx
│   │   │   └─ Navbar.tsx
│   │   ├─ layout/          # Layout components (header, footer, nav)
│   │   │   ├─ Header.tsx
│   │   │   ├─ BottomNav.tsx
│   │   │   └─ Sidebar.tsx
│   │   └─ features/        # Feature-based components
│   │       ├─ LocationBanner.tsx
│   │       ├─ CoverageBanner.tsx
│   │       └─ BundleCard.tsx
│   │
│   ├─ context/             # Global state (React Context API)
│   │   └─ LocationContext.tsx
│   │
│   ├─ hooks/               # Custom hooks
│   │   ├─ useCoverage.ts
│   │   ├─ useLocation.ts
│   │   └─ useBundles.ts
│   │
│   ├─ lib/                 # API + utilities
│   │   ├─ api/             # API service helpers
│   │   │   ├─ coverage.ts
│   │   │   └─ bundles.ts
│   │   └─ utils.ts         # Helper functions
│   │
│   ├─ styles/              # SCSS styles
│   │   ├─ globals.scss     # Global styles
│   │   ├─ variables.scss   # Color palette, fonts, etc.
│   │   └─ components/      # Component-specific styles
│   │       ├─ navbar.scss
│   │       └─ bundle-card.scss
│   │
│   └─ types/               # TypeScript types
│       ├─ coverage.ts
│       └─ bundles.ts
│
├─ .eslintrc.json           # ESLint rules
├─ tsconfig.json            # TS config with path aliases
├─ package.json
└─ README.md