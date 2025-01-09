# Narthbugz.com Knowledge

## Project Overview
Marketing website for Narthbugz, a time-tracking and forecasting tool for development teams. Built with Astro.

## Key Features
- Evidence-based forecasting using Monte Carlo simulations
- Time tracking for development teams
- Integration with development tools and project management software

## Tech Stack
- Astro for static site generation
- TypeScript for type safety
- PNPM as package manager

## Development Guidelines

### Styling
- Use system font stack for better performance
- Maintain consistent color scheme:
  - Primary gradient: #3245ff to #bc52ee
  - Light mode:
    - Text primary: #111827
    - Text secondary: #4b5563
    - Background primary: rgba(255, 255, 255, 0.8)
  - Dark mode:
    - Text primary: #f3f4f6
    - Text secondary: #d1d5db (ensure all text uses CSS variables for consistent contrast)
    - Background primary: rgba(17, 24, 39, 0.85)
- Responsive breakpoint at 768px
- Use glass-morphism effects for depth (background blur + transparency)
- Support system and user dark mode preferences

### Components
- Keep components in src/components
- Use .astro files for static components
- Maintain mobile-first responsive design

### Performance
- Optimize images before adding to assets
- Use fetchpriority="high" for above-the-fold images
- Minimize JavaScript usage where possible
- Use `is:inline` script to set initial theme before page render to prevent flash of unstyled content
- Enable Astro view transitions for smooth page navigation

## Commands
```bash
# Development
pnpm dev        # Start dev server
pnpm build      # Build for production
pnpm preview    # Preview production build
pnpm a11y       # Run accessibility checks (requires dev server running)
```

## Project Structure
```
src/
├── assets/     # Static assets
├── components/ # Reusable components
├── layouts/    # Page layouts
└── pages/      # Route pages
```
