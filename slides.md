---
title: YouWare x Adventure X Presentation
info: |
  A minimalist presentation using YouWare design system
theme: slidev-theme-cursor
class: text-center
mdc: true
layout: default
---

# Vibe is All You Need —— 从感觉到表达

<div class="flex justify-center items-center h-full">
  <img src="./assets/wordcloud_final.png" class="h-[100%] w-auto" />
</div>

---
layout: two-cols
---

# Self Introduction

<div class="mt-16">

## Marvin (马进)

<ul class="text-base space-y-2">
  <li>算法工程师 @YouWare，之前在豆瓣和 AfterShip 做推荐系统</li>
  <li>Cursor 的 Ambassador，线下 Meetup & Hackathon 的主办方</li>
  <li>做过一些 Vibe Coding 开源工具，Github 1k+ star</li>
  <li>头像来自于大卫林奇的 Twin Peaks + 辛普森风格迁移</li>
</ul>

</div>

::right::

<div class="flex flex-row gap-6 items-center justify-center h-full">
  <YouWareCard :hoverable="true" class="w-55 h-55">
    <img src='./assets/marvin.jpg' class="w-full h-full object-cover rounded-lg" />
  </YouWareCard>
  
  <YouWareCard :hoverable="true" class="w-55 h-55">
    <img src='./assets/man+from+another+place.jpg' class="w-full h-full object-cover rounded-lg" />
  </YouWareCard>
</div>


---
layout: two-cols
---

# Cursor Meetup Hangzhou

<div class="flex justify-left">
  <img src='./assets/hangzhou.jpg' class="w-100 h-100 object-cover rounded-lg shadow-lg">
</div>

::right::

# Cursor Hackathon Shenzhen

<div class="flex justify-left">
  <img src='./assets/hackathon.jpg' class="w-100 h-100 object-cover rounded-lg shadow-lg">
</div>

---
layout: default
---

# What's vibe coding, exactly?

<div class="grid grid-cols-2 gap-8 mt-16">
  <YouWareCard :hoverable="true">
    <img src='./assets/Vibe sharing.png' class="w-full h-auto object-cover rounded-lg">
  </YouWareCard>
  
  <YouWareCard :hoverable="true">
    <img src='./assets/image1.png' class="w-full h-auto object-cover rounded-lg">
  </YouWareCard>
</div>


<div class="mt-20">
  <h2 class="text-2xl font-medium mb-4">快速调查：Vibe coding 出来的代码是否应该 review？</h2>
</div>

---
layout: default
---

# Vibe coding is cool, but...

<div class="flex items-center gap-8">
  <img src='./assets/image4.png' class="w-140 h-auto object-cover rounded-lg shadow-lg">
  <div class="text-2xl font-bold">
    <p>掌控了可控核聚变</p>
    <p>却拿来给手机充电</p>
  </div>
</div>
<div class="mt-12">
  <h2 class="text-2xl font-medium mb-4">为什么大家 Vibe Coding 最后都只在做 Landing Page?</h2>
</div>

---
layout: default
---

# What went wrong? 

<div class="grid grid-cols-3 gap-8 mt-8">
  <div class="flex justify-center">
    <img src="./assets/arch_1.png" class="w-auto h-100 object-cover rounded-lg shadow-lg">
  </div>
  
  <div class="flex flex-col gap-4 col-span-2">
    <img src="./assets/arch_2.png" class="w-160 h-72 object-cover rounded-lg shadow-lg">
    <img src="./assets/arch_3.png" class="w-160 h-32 object-cover rounded-lg shadow-lg">
  </div>
</div>

---
layout: two-cols
---

# What is vibe?

<div class="flex flex-col gap-6">
  <YouWareCard :hoverable="true" class="p-6">
    <img src='./assets/vibe_hangzhou_sharing.jpg' class="w-full h-64 object-cover rounded-lg mb-4">
    <div class="text-sm text-gray-600">
      <p class="font-medium mb-2">Cursor Meetup Hangzhou</p>
      <p>2025 年 7 月 12 日</p>
      <p class="italic">硅星人主编 王兆洋</p>
    </div>
  </YouWareCard>
</div>

::right::

<div class="flex flex-col items-center justify-center h-full">
  <img src='./assets/wordcloud_final.png' class="w-full h-96 object-cover ">
  
  <div class="text-center">
    <h2 class="text-3xl font-bold text-[#5A6650]">
      <span class="text-4xl">Vibe</span> is all you need.
    </h2>
  </div>
</div>

---
layout: default
---

# Vibe coder and painter

<div>
  <div class="col-span-2 flex justify-center items-center">
    <Youtube id="8tK3IxZG80k" width="500" height="360" />
  </div>
</div>

<div class="mt-12 flex justify-center">
  <h2 class="text-2xl font-medium mb-4">即使你有毕加索的技术，你就能画出毕加索的画吗？</h2>
</div>

---
layout: default
---

# Vibe coder and painter

<div class="flex">
  <!-- Left column - 1/3 width -->
  <div class="w-1/3 pr-8">
    <img src="./assets/paul graham.jpg" class="w-full h-100 object-cover rounded-lg shadow-lg">
  </div>

  <!-- Right column - 2/3 width -->
  <div class="w-2/3 flex flex-col gap-6">
    <YouWareCard class="p-6">
      <h3 class="text-xl font-medium mb-4">创作者的共同点</h3>
      <ul class="space-y-4 text-[#333333]">
        <li>黑客与画家都是创作者。对于想写出漂亮程序的黑客来说，计算机只是一种工具，就像画家的画笔 —— Paul Graham</li>
        <li>Vibe Coding 让我们每个人都成为了神笔马良。</li>
      </ul>
    </YouWareCard>
    <YouWareCard class="p-6">
      <h3 class="text-xl font-medium mb-4">真正的挑战</h3>
      <ul class="space-y-2 text-[#333333]">
        <li> 如何管理色彩 <span class="text-[#5A6650]">(如何管理上下文)</span></li>
        <li> 补救还是重画 <span class="text-[#5A6650]">(硬聊还是重开)</span></li>
        <li> 内心的 Image <span class="text-[#5A6650]">(Vibe)</span></li>
      </ul>
    </YouWareCard>
  </div>
</div>

---
layout: two-cols
---

# How to get vibes?

<div class="mt-24">
  <ul class="space-y-6 text-lg">
    <li>不知道自己想要什么，这很正常</li>
    <li>Good Artist Copy, Great Artist Steal</li>
    <li>这句话其实是毕加索说的</li>
  </ul>
</div>

::right::

<div class="flex items-center justify-center h-full">
  <img src="./assets/jobs.jpg" class="w-full h-auto object-cover rounded-lg shadow-lg">
</div>

---
layout: default
---

# Case: My personal website

<div class="grid grid-cols-6 gap-8 h-full">
  <div class="col-span-2 flex flex-col justify-center gap-6">
    <YouWareCard class="p-6">
      <h3 class="text-xl font-medium mb-4">背景</h3>
      <p class="text-[#333333]">换工作阶段比较闲，想做一下个人网站</p>
    </YouWareCard>
    <YouWareCard class="p-6">
      <h3 class="text-xl font-medium mb-4">第一版<a href="https://aabdoo23.vercel.app/" class="text-[#5A6650] hover:underline">尝试</a></h3>
    </YouWareCard>
  </div>

  <div class="col-span-4 flex items-center justify-center">
    <div class="w-auto h-100 bg-white rounded-lg shadow-lg overflow-hidden">
      <img src="./assets/astro_v1.png" class="w-full h-full object-cover">
    </div>
  </div>
</div>

---
layout: default
---

# What if...
<div class="grid grid-cols-8 gap-8 h-full">
  <div class="col-span-4 flex items-center justify-center">
    <Youtube id="Ucct_YVl1tY" width="500" height="320" />
  </div>
  <div class="col-span-4 flex items-center justify-center">
    <img src='./assets/beijing.jpg' class="w-auto h-100 object-cover rounded-lg shadow-lg">
  </div>
</div>


---
layout: default
---

# What if...

<img src='./assets/ryos.png' class="w-auto h-110 object-cover rounded-lg shadow-lg">

---
layout: default
---

# Creating my own OS

最初尝试：Mac System 7 风格
AI 很擅长，但觉得没有意思

灵感：Terry A. Davis TempleOS
<img src='./assets/terry_davis.jpg' class="w-auto h-60 object-cover rounded-lg shadow-lg">
<img src='./assets/TempleOS_4.05_session.png' class="w-auto h-60 object-cover rounded-lg shadow-lg">

过去需要花一辈子的事情，现在只需要几分钟


---
layout: default
---

# Adding more elements


Psychonauts

---
layout: default
---

# I could create what I want

最重要的是这个理念的转变

Disco Elysium

Ape of Naples

Near Death Experience

---
layout: default
---

# I could create what I want

最重要的是这个理念的转变

Near Death Experience

Disco Elysium

Ape of Naples

---
layout: default
---

# My Toolkit

AI 头脑风暴模式

---
layout: default
---

# My Suggestions

1. 强迫自己不去改代码，锻炼自己的 prompt 能力
2. 使用 code-based 方案，而不是 UI-based 方案 (e.g. SuperCollider vs Ableton)
3. 多看别人的项目，从中获得启发

---
layout: default
---

# Youware: Vibe coder's community


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