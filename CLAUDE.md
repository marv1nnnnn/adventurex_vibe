# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Slidev presentation kit built for Cursor Ambassadors and Team members. It uses the custom `slidev-theme-cursor` theme that follows Cursor's monochrome branding guidelines.

## Development Commands

```bash
# Install dependencies
pnpm install

# Start development server with hot reload
pnpm dev

# Build static presentation for deployment
pnpm build

# Export presentation to various formats
pnpm export
```

## Architecture & Structure

### Core Technology Stack
- **Framework**: Slidev (Vue.js-based presentation framework)
- **Package Manager**: pnpm
- **Styling**: Tailwind CSS with UnoCSS utilities
- **Theme**: Custom `slidev-theme-cursor` (local dependency)

### Key Directories
- `slides.md` - Main presentation content using Markdown
- `components/` - Vue components (e.g., GlowBackground.vue for animated effects)
- `assets/` - Static assets (images, QR codes, logos)
- `slidev-theme-cursor/` - Custom theme implementation
- `.cursor/rules/` - AI assistant guidelines for slide creation and branding

### Deployment Configuration
- **Netlify**: Configured via `netlify.toml` with SPA redirects
- **Vercel**: Configured via `vercel.json` with SPA rewrites
- **GitHub Pages**: Workflow available at `.github/workflows/deploy.yml`

## Creating and Editing Slides

### Basic Slide Structure
- Use `---` with newlines to separate slides
- Enable MDC syntax with `mdc: true` in frontmatter for enhanced Markdown components
- Wrap content with `<GlowBackground>` for animated background effects

### Common Slide Patterns
```markdown
---
layout: cover
class: bg-[#0F0F0F] text-white text-center
---

<GlowBackground>
  <h1 class="text-6xl font-bold">Title</h1>
</GlowBackground>
```

### Cursor Brand Guidelines
Follow these color values for consistency:
- Primary background: `#0F0F0F`
- Card background: `#171717`
- Border/divider: `#252525`
- Body text: `rgba(255, 255, 255, 0.8)`
- Headlines: `#FFFFFF`
- Accent grey: `#6E6E6E`

Typography:
- Font: Inter
- H1/H2: Weight 900, tracking -2%
- Body: Weight 400-500

## Important Conventions

1. **Component Usage**: Always check existing components before creating new ones
2. **Styling**: Use Tailwind/UnoCSS classes inline, avoid separate CSS files
3. **Images**: Store in `assets/` directory with descriptive names
4. **Custom Components**: Follow Vue 3 Composition API with `<script setup>`

## AI Assistant Rules

Two MDC rule files provide comprehensive guidance:
- `create-slidev-slides.mdc` - Detailed Slidev syntax and features guide
- `cursor-brand-guidelines.mdc` - Complete Cursor monochrome branding specifications

Reference these when creating slides or modifying theme components to ensure consistency with Cursor's design system.