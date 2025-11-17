# Project Initialization: blabla

**Date:** November 17, 2025

## Project Overview

This document details the setup and initialization of the `blabla` project, a Next.js 16 application with shadcn/ui components and Supabase integration, styled with an Airbnb-inspired design system.

## Tools and Versions

- **Node.js:** v22.9.0
- **Package Manager:** pnpm 10.9.0
- **Framework:** Next.js 16.0.3 (Turbopack)
- **UI Components:** shadcn/ui (54 components installed)
- **Database:** Supabase (@supabase/supabase-js 2.81.1)
- **Git:** 2.50.1
- **Vercel CLI:** 44.7.3
- **GitHub CLI:** 2.76.2

## Project Initialization

### 1. Prerequisites Verification

All prerequisites were verified and confirmed:
- ✅ Node.js installed
- ✅ pnpm installed
- ✅ Git installed and configured (Sebastien Payet, payets@haufe.com)
- ✅ Vercel CLI installed and logged in (sebastien-ai-collabs)
- ✅ GitHub CLI installed and logged in (sebyet)

### 2. Project Creation

- **Framework:** Next.js 16
- **Base Color:** Neutral
- **Project Location:** `/Users/sebastien.payet/Projects/sebastien/blabla/`
- **Initialization Method:** `pnpm dlx shadcn@latest init` with automated prompts

### 3. Configuration Files Created

- `components.json` - shadcn/ui configuration
- `next.config.ts` - Next.js configuration
- `tsconfig.json` - TypeScript configuration
- `tailwind.config.ts` - Tailwind CSS configuration (via shadcn)
- `postcss.config.mjs` - PostCSS configuration
- `eslint.config.mjs` - ESLint configuration
- `.gitignore` - Git ignore rules

### 4. Components Installed

All 54 shadcn/ui components were installed:
- Navigation: Accordion, Breadcrumb, Menubar, Navigation Menu, Sidebar, Tabs
- Forms: Button, Button Group, Checkbox, Form, Input, Input Group, Input OTP, Label, Radio Group, Select, Slider, Switch, Textarea, Toggle, Toggle Group
- Feedback: Alert, Alert Dialog, Badge, Progress, Skeleton, Sonner, Spinner
- Overlays: Dialog, Drawer, Popover, Sheet, Tooltip, Hover Card, Context Menu, Command
- Data Display: Card, Table, Avatar, Calendar, Carousel, Chart, Pagination, Empty
- Layout: Aspect Ratio, Collapsible, Resizable, Scroll Area, Separator
- Utilities: Field, Item, KBD

### 5. Dependencies

**Core Dependencies:**
- `next` - Next.js framework
- `react` & `react-dom` - React library
- `@supabase/supabase-js` - Supabase JavaScript client

**UI Dependencies:**
- `tailwindcss` - Utility-first CSS framework
- `class-variance-authority` - Component variant management
- `clsx` & `tailwind-merge` - Class name utilities
- `lucide-react` - Icon library
- `@radix-ui/*` - Headless UI primitives (installed via shadcn components)

### 6. Design System Customization

**Design Inspiration:** Airbnb

**Color Palette:**
- **Primary:** Airbnb Rausch red/coral (`oklch(0.65 0.18 12)`) - #FF5A5F equivalent
- **Background:** Clean white (`oklch(1 0 0)`)
- **Foreground:** Dark text (`oklch(0.145 0 0)`)
- **Secondary:** Light gray (`oklch(0.96 0 0)`)
- **Success:** Green (`oklch(0.65 0.15 145)`)
- **Warning:** Amber (`oklch(0.75 0.15 75)`)
- **Destructive:** Red (`oklch(0.577 0.245 27.325)`)

**Typography:**
- **Primary Font:** Inter (similar to Airbnb's Circular)
- **Monospace Font:** Geist Mono
- Font variables configured in `app/layout.tsx`

**Border Radius:**
- **Base:** 0.75rem (12px) - moderate rounding like Airbnb
- Responsive scale: sm, md, lg, xl

**Dark Mode:**
- Fully configured with adjusted colors for dark backgrounds
- Primary color slightly brighter in dark mode for visibility

### 7. Git Setup

- **Repository:** Initialized locally
- **Initial Commit:** "Initial commit: Next.js 16 project with shadcn/ui and Supabase"
- **Design System Commit:** "Customize design system: Apply Airbnb-inspired design (Rausch red primary, Inter font, rounded corners)"

### 8. GitHub Integration

- **Repository:** https://github.com/sebyet/blabla
- **Remote:** origin
- **Branch:** main
- **Status:** Connected and synced

### 9. Vercel Integration

- **Project:** sebyet/blabla
- **Status:** Linked and configured
- **Auto-deployments:** Configured (GitHub → Vercel)
- **Framework Preset:** Next.js (auto-detected)
- **Build Command:** `next build`
- **Development Command:** `next dev --port $PORT`

### 10. Project Structure

```
blabla/
├── app/
│   ├── globals.css          # Design system tokens
│   ├── layout.tsx           # Root layout with Inter font
│   └── page.tsx             # Home page
├── components/
│   └── ui/                   # 54 shadcn/ui components
├── hooks/
│   └── use-mobile.ts        # Mobile detection hook
├── lib/
│   └── utils.ts             # Utility functions (cn helper)
├── public/                   # Static assets
├── .cursor/                  # Cursor commands and rules
├── doc/                      # Documentation
└── [config files]           # Next.js, TypeScript, etc.
```

## Next Steps

1. **Start Development:**
   ```bash
   cd blabla
   pnpm dev
   ```

2. **Build for Production:**
   ```bash
   pnpm build
   ```

3. **Deploy:**
   - Automatic deployments configured via Vercel
   - Push to `main` branch triggers deployment

4. **Supabase Setup:**
   - Create a Supabase project at https://supabase.com
   - Add environment variables to Vercel:
     - `NEXT_PUBLIC_SUPABASE_URL`
     - `NEXT_PUBLIC_SUPABASE_ANON_KEY`

5. **Design System:**
   - Design tokens are in `app/globals.css`
   - All components use design system tokens
   - Airbnb-inspired color palette applied

## Design System Reference

**Primary Color (Airbnb Rausch Red):**
- Light mode: `oklch(0.65 0.18 12)`
- Dark mode: `oklch(0.7 0.2 12)`

**Usage:**
- Primary buttons and CTAs
- Links and interactive elements
- Focus rings and accents

**Font:**
- Inter (Google Fonts) - clean, modern, similar to Airbnb's Circular

**Border Radius:**
- Base: 12px (0.75rem)
- Creates friendly, approachable feel like Airbnb

## Notes

- All shadcn/ui components are installed and ready to use
- Design system is fully configured with Airbnb-inspired styling
- Project is connected to GitHub and Vercel for seamless deployment
- Cursor commands and rules are available in `.cursor/` folder

