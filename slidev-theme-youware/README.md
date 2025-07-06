# Slidev Theme YouWare

A minimalist Slidev theme inspired by YouWare's design system, featuring a warm color palette, Courier Prime typography, and clean components.

## Installation

Add the theme to your Slidev project:

```json
{
  "dependencies": {
    "slidev-theme-youware": "link:slidev-theme-youware"
  }
}
```

Then set it in your slides frontmatter:

```yaml
---
theme: slidev-theme-youware
---
```

## Components

### YouWareButton

A versatile button component with primary and secondary variants.

#### Props
- `href` (string, optional): Makes the button a link
- `to` (string, optional): Makes the button a router link
- `variant` (string, optional): 'primary' | 'secondary' (default: 'primary')

#### Usage

```vue
<!-- Primary button -->
<YouWareButton>
  Click Me
</YouWareButton>

<!-- Secondary button -->
<YouWareButton variant="secondary">
  Learn More
</YouWareButton>

<!-- Button as link -->
<YouWareButton href="https://youware.com">
  Visit Website
</YouWareButton>
```

#### Styling
- Primary: Green background (#4A6741) with white text
- Secondary: Transparent with green border
- Hover effects with subtle elevation
- Rounded corners (8px radius)

### YouWareCard

A clean card component for organizing content.

#### Props
- `title` (string, optional): Card header title

#### Usage

```vue
<!-- Card with title -->
<YouWareCard title="Feature Name">
  Description of the feature goes here
</YouWareCard>

<!-- Card without title -->
<YouWareCard>
  Simple content in a card
</YouWareCard>
```

#### Styling
- White background with subtle border
- 12px border radius
- Soft shadow that elevates on hover
- 2rem padding

## Layouts

### cover

The hero/title slide layout with centered content.

#### Features
- Logo support (top-left position)
- Event/date tags in footer
- Centered content alignment
- Maximum content width of 900px

#### Frontmatter Options
```yaml
---
layout: cover
logo: ./path/to/logo.png
event: Conference Name
date: July 2025
---
```

### default

Standard content layout with comfortable padding.

#### Features
- 4rem padding on all sides
- Full typography support
- No special positioning

#### Usage
```yaml
---
layout: default
---
```

### two-cols

Split-screen layout for side-by-side content.

#### Features
- Equal column widths by default
- Right column content via `::right::` slot
- Gap of 3rem between columns
- Responsive grid layout

#### Usage
```markdown
---
layout: two-cols
---

# Left Column
Content for the left side

::right::

# Right Column
Content for the right side
```

### center

Centered content layout for impactful statements.

#### Features
- Vertically and horizontally centered
- Maximum content width of 800px
- Perfect for single statements or CTAs

#### Usage
```yaml
---
layout: center
---
```

### section

Full-color section divider slides.

#### Features
- Green background (#4A6741)
- White text override
- Centered content
- Full viewport height

#### Usage
```yaml
---
layout: section
---
```

### quote

Beautiful quote layout with citation support.

#### Features
- Large quote text (2rem)
- Centered alignment
- Citation styling with `<cite>` tag
- No quote borders (clean look)

#### Usage
```markdown
---
layout: quote
---

<blockquote>
  "Your inspiring quote here"
</blockquote>

<cite>— Author Name, Title</cite>
```

## Utility Classes

### .yw-button
Standalone button styling (same as YouWareButton component)

### .yw-tag
Pill-shaped tags for categories or labels

```html
<span class="yw-tag">Category</span>
```

Features:
- Rounded pill shape
- Light beige background
- Small text (0.875rem)
- Inline-block display

### .yw-card
Standalone card styling (same as YouWareCard component)

## Color Palette

The theme uses CSS custom properties for consistent theming:

```css
--yw-bg-primary: #F5F0E8;      /* Light beige background */
--yw-bg-white: #FFFFFF;        /* Pure white */
--yw-text-primary: #2D2D2D;    /* Dark text */
--yw-text-secondary: #6B6B6B;  /* Secondary text */
--yw-text-muted: #A5A5A5;      /* Muted text */
--yw-accent-green: #4A6741;    /* Primary green */
--yw-accent-green-hover: #3A5331; /* Darker green */
--yw-border: #E5E0D8;          /* Border color */
--yw-tag-bg: #F0EBE3;          /* Tag background */
```

## Typography

- **Font Family**: Courier Prime (monospace)
- **Headings**: Bold with tight letter-spacing
- **Body Text**: Regular weight with comfortable line-height
- **Code**: Courier Prime in both inline and blocks

### Font Sizes
- H1: 3.5rem
- H2: 2.5rem
- H3: 1.875rem
- H4: 1.5rem
- Body: 1.125rem
- Code: 0.875rem

## Theme Configuration

In your `slides.md`:

```yaml
---
theme: slidev-theme-youware
colorSchema: light
fonts:
  sans: Courier Prime
  mono: Courier Prime
---
```

## Example Slides

### Hero Slide
```markdown
---
layout: cover
event: Tech Conference
date: July 2025
---

# Your Title Here

Your subtitle or tagline

<YouWareButton>
  Get Started
</YouWareButton>
```

### Feature Grid
```markdown
---
layout: default
---

# Features

<div class="grid grid-cols-3 gap-4">
  <YouWareCard title="Fast">
    Lightning quick performance
  </YouWareCard>
  
  <YouWareCard title="Simple">
    Clean and intuitive
  </YouWareCard>
  
  <YouWareCard title="Powerful">
    Feature-rich platform
  </YouWareCard>
</div>
```

### Quote Slide
```markdown
---
layout: quote
---

<blockquote>
  "The best way to predict the future is to invent it."
</blockquote>

<cite>— Alan Kay</cite>
```

## Best Practices

1. **Use Courier Prime** - The theme is optimized for this monospace font
2. **Embrace whitespace** - The design philosophy emphasizes breathing room
3. **Keep it minimal** - Less is more with this theme
4. **Use the color palette** - Stick to the provided colors for consistency
5. **Leverage components** - Use YouWareButton and YouWareCard for cohesive design

## License

MIT