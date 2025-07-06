---
title: YouWare x Adventure X Presentation
info: |
  A minimalist presentation using YouWare design system
theme: slidev-theme-youware
class: text-center
mdc: true
layout: default
---

# Vibe is All You Need
## 从感觉到表达

<ProfileCard 
  name="Marvin Ma"
  title="Machine Learning Engineer @ YouWare"
  :items="[
    { icon: '🌟', text: 'Building open source vibe coding tools' },
    { icon: '🚀', text: 'Cursor Ambassador & Hackathon Host' }
  ]"
/>
---
layout: default
---

# Welcome to YouWare

Building the future of personalized computing experiences.

<div class="mt-8 grid grid-cols-3 gap-4">
  <YouWareCard title="Create">
    Build custom applications tailored to your workflow
  </YouWareCard>
  
  <YouWareCard title="Upload">
    Share your creations with the community
  </YouWareCard>
  
  <YouWareCard title="Paste Code">
    Quick prototyping with instant preview
  </YouWareCard>
</div>

---
layout: two-cols
---

# Features

Our platform offers:

- 🚀 **Lightning Fast** - Built for speed
- 🎨 **Beautiful Design** - Minimalist and clean
- 🔧 **Developer Friendly** - Great DX
- 🌍 **Community Driven** - Open ecosystem

::right::

```javascript
// Example code
function createProject(name) {
  return {
    id: generateId(),
    name: name,
    created: new Date(),
    status: 'active'
  }
}

const myProject = createProject('YouWare Demo')
console.log(myProject)
```

---
layout: section
---

# Build Something Amazing

Join thousands of developers creating the future

---
layout: center
---

# Trending Projects

<div class="flex flex-wrap justify-center gap-2 mt-8">
  <span class="yw-tag">All</span>
  <span class="yw-tag">Game</span>
  <span class="yw-tag">Productivity tool</span>
  <span class="yw-tag">Education</span>
  <span class="yw-tag">Presentation</span>
  <span class="yw-tag">Landing page</span>
  <span class="yw-tag">Dashboard</span>
  <span class="yw-tag">Portfolio</span>
</div>

---
layout: quote
---

<blockquote>
  "YouWare has completely transformed how I build and share my projects. The minimalist design and powerful features make it a joy to use."
</blockquote>

<cite>— Alex Chen, Full Stack Developer</cite>

---
layout: default
---

# Getting Started

1. **Sign up** for a free account
2. **Create** your first project
3. **Share** with the community

<div class="mt-8">
  <YouWareButton variant="primary">
    Start Building
  </YouWareButton>
  
  <YouWareButton variant="secondary" class="ml-4">
    View Documentation
  </YouWareButton>
</div>

---
layout: cover
---

# Thank You

<p class="text-xl mt-4">
  Ready to build something amazing?
</p>

<div class="mt-8 flex gap-4 justify-center">
  <span class="yw-tag">@youware</span>
  <span class="yw-tag">youware.com</span>
</div>