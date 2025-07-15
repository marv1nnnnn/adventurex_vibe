# Technology Stack

## Core Framework
- **Slidev**: Vue-based presentation framework
- **Vue 3**: Component framework with Composition API
- **TypeScript**: Type-safe JavaScript (in components)
- **Vite**: Build tool and dev server

## Package Management
- **pnpm**: Primary package manager (v10.7.0+)
- **Node.js**: Runtime (v18.0.0+ required)

## Themes & Styling
- **slidev-theme-cursor**: Custom Cursor-branded theme
- **Tailwind CSS**: Utility-first CSS framework (via Slidev)
- **Custom Components**: Vue SFC components in `/components`

## Deployment Platforms
- **GitHub Pages**: Automated via GitHub Actions
- **Vercel**: SPA deployment with rewrites
- **Netlify**: Static site hosting

## Common Commands

### Development
```bash
pnpm install          # Install dependencies
pnpm dev             # Start dev server (localhost:3030)
```

### Build & Export
```bash
pnpm build           # Build for production
pnpm export          # Export slides as PDF/images
```

### Theme Development
```bash
# In slidev-theme-cursor directory
pnpm dev             # Test theme with example.md
pnpm screenshot      # Generate theme screenshots
```

## File Structure Conventions
- Slides content: `slides.md` (main presentation)
- Components: `/components/*.vue`
- Assets: `/assets/*` (images, media)
- Theme: `/slidev-theme-cursor/` (linked package)