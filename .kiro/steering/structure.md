# Project Structure

## Root Directory Organization

```
cursor-slidev/
├── slides.md                 # Main presentation content
├── components/               # Custom Vue components
│   ├── GlowBackground.vue   # Animated background component
│   └── Counter.vue          # Example interactive component
├── assets/                  # Static assets (images, media)
├── pages/                   # Additional slide pages
├── slidev-theme-cursor/     # Custom Cursor theme package
│   ├── layouts/            # Theme layout components
│   ├── components/         # Theme-specific components
│   ├── styles/             # Theme CSS/styling
│   └── setup/              # Theme configuration
└── snippets/               # Code snippets for presentations
```

## Key File Conventions

### Presentation Files
- **slides.md**: Primary presentation content with frontmatter
- **pages/*.md**: Additional slide collections
- **slides_ref.md**: Reference/backup slides

### Component Architecture
- **components/**: Project-specific Vue components
- **slidev-theme-cursor/components/**: Theme-level reusable components
- Use PascalCase for component names
- Prefer Composition API with `<script setup>`

### Asset Management
- **assets/**: All images, videos, and media files
- Use descriptive filenames (e.g., `wordcloud_final.png`)
- Organize by presentation or topic when needed

### Theme Structure
- **layouts/**: Slidev layout components (cover, two-cols, etc.)
- **styles/**: Global theme styles and CSS variables
- **setup/**: Theme initialization and configuration

## Naming Conventions
- Slide files: kebab-case (e.g., `imported-slides.md`)
- Components: PascalCase (e.g., `GlowBackground.vue`)
- Assets: descriptive names with underscores (e.g., `vibe_hangzhou_sharing.jpg`)
- Directories: lowercase with hyphens (e.g., `slidev-theme-cursor`)

## Configuration Files
- **package.json**: Project dependencies and scripts
- **netlify.toml**: Netlify deployment configuration
- **vercel.json**: Vercel deployment settings
- **.cursor/rules/**: Cursor AI guidance files