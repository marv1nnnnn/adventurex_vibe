# YouWare Theme Guide for Slidev

This guide explains how to use the YouWare-branded Slidev theme in your presentation files.

## Theme Overview

The YouWare theme transforms the default Cursor theme into a light, minimalist design that matches YouWare's branding:
- **Background**: Light cream (#F5F0E8)
- **Typography**: Courier Prime (English), PingFang SC (Chinese)
- **Accent Color**: Forest green (#5A6650)
- **Style**: Clean, vintage tech aesthetic

## Basic Setup

In your `slides.md` frontmatter, ensure you're using the theme:

```yaml
---
theme: slidev-theme-cursor
mdc: true  # Enable MDC for enhanced components
---
```

## Available Layouts

### 1. Cover Layout
Perfect for title slides with centered content:

```markdown
---
layout: cover
---

# Your Title Here
## Subtitle in Chinese or English

<p class="text-xl mt-4">
  Additional description text
</p>
```

### 2. Intro Layout
For introduction slides with more content:

```markdown
---
layout: intro
---

# Introduction Title

Your introductory content here with automatic spacing and styling.
```

### 3. Default Layout
Standard slide layout with full flexibility:

```markdown
---
layout: default
---

# Slide Title

Your content here...
```

### 4. Two Columns Layout
For side-by-side content:

```markdown
---
layout: two-cols
---

# Left Column Title

Content for the left side...

::right::

# Right Column Title

Content for the right side...
```

### 5. Section Layout
For section dividers:

```markdown
---
layout: section
---

# New Section Title

Brief description or tagline
```

### 6. Quote Layout
For testimonials or quotes:

```markdown
---
layout: quote
---

<blockquote>
  "Your quote text here..."
</blockquote>

<cite>— Author Name, Title</cite>
```

## YouWare Components

### YouWareButton
A styled button component with YouWare's green accent:

```vue
<YouWareButton>
  Click Me
</YouWareButton>

<!-- With size variants -->
<YouWareButton size="small">Small Button</YouWareButton>
<YouWareButton size="medium">Medium Button</YouWareButton>
<YouWareButton size="large">Large Button</YouWareButton>

<!-- Full width -->
<YouWareButton :full-width="true">
  Full Width Button
</YouWareButton>
```

### YouWareCard
A clean card component for organized content:

```vue
<YouWareCard>
  <h3>Card Title</h3>
  <p>Card content goes here...</p>
</YouWareCard>

<!-- With hover effect -->
<YouWareCard :hoverable="true">
  <h3>Hoverable Card</h3>
  <p>This card lifts on hover</p>
</YouWareCard>
```

## Styling Classes

### Text Colors
- `text-[#333333]` - Body text (default)
- `text-[#1A1A1A]` - Heading text
- `text-[#5A6650]` - Green accent text

### Backgrounds
- `bg-[#F5F0E8]` - Primary background
- `bg-white` - Card background
- `bg-[#FAFAF8]` - Code block background

### Custom Tags
For the YouWare tag style seen in the trending projects:

```css
<style>
.yw-tag {
  @apply px-4 py-2 bg-[#5A6650] text-white rounded-full text-sm font-medium;
  @apply hover:bg-[#4A5640] transition-colors cursor-pointer;
}
</style>
```

## Typography Guidelines

### Headings
- **H1**: 3rem (48px), font-weight: 600
- **H2**: 2rem (32px), font-weight: 600
- **H3/H4**: 1.5rem (24px), font-weight: 500

### Body Text
- Regular text uses Courier Prime at 400 weight
- Line height: 1.6 for better readability
- Chinese text automatically uses PingFang SC

### Code Blocks
Code blocks automatically use Courier Prime with the light background theme:

```javascript
// Your code here
const message = "Hello, YouWare!"
console.log(message)
```

## Best Practices

1. **Keep It Minimal**: YouWare's aesthetic is clean and uncluttered
2. **Use White Space**: Don't overcrowd slides; let content breathe
3. **Consistent Spacing**: Use the built-in spacing utilities
4. **Green Accents**: Use the forest green color sparingly for emphasis
5. **Mix Languages**: The theme supports seamless Chinese/English mixing

## Example Slide Patterns

### Hero Slide
```markdown
---
layout: cover
---

# Not YouTube, it's YouWare.

<p class="text-xl mt-4 opacity-70">
  Finally, your computer speaks your language.
</p>

<div class="mt-8">
  <YouWareButton size="large">
    Get Started
  </YouWareButton>
</div>
```

### Feature Grid
```markdown
---
layout: default
---

# Features

<div class="grid grid-cols-3 gap-6 mt-8">
  <YouWareCard :hoverable="true">
    <h3>Create</h3>
    <p>Build custom apps</p>
  </YouWareCard>
  
  <YouWareCard :hoverable="true">
    <h3>Upload</h3>
    <p>Share with others</p>
  </YouWareCard>
  
  <YouWareCard :hoverable="true">
    <h3>Connect</h3>
    <p>Join the community</p>
  </YouWareCard>
</div>
```

### Mixed Language Content
```markdown
---
layout: default
---

# Vibe is All You Need
## 从感觉到表达

The theme automatically handles font switching between Courier Prime and PingFang SC.

你可以自由地混合使用中英文内容。
```

## Troubleshooting

1. **Fonts Not Loading**: Ensure Courier Prime is available or will be loaded via web fonts
2. **Chinese Text Issues**: PingFang SC should fallback to system Chinese fonts if not available
3. **Dark Mode**: The theme is designed for light mode only (`colorSchema: "light"`)

## Additional Resources

- Original Slidev documentation: https://sli.dev
- YouWare brand guidelines: (internal document)
- Component examples: See `slides.md` for live examples