---
theme: slidev-theme-cursor
layout: cover
---

<div class="absolute inset-0">
  <img src="./assets/cover.png" class="w-full h-full object-cover" />
</div>

---
layout: cover
---

<div class="absolute inset-0">
  <img src="./assets/cover_2.png" class="w-full h-full object-cover" />
</div>


---
layout: cover
---

<div class="absolute inset-0">
  <img src="./assets/cover_3.png" class="w-full h-full object-cover" />
</div>


---
layout: default
---

# What's vibe coding, exactly?

<div class="grid grid-cols-2 gap-8 mt-16">
  <div v-click="1">
    <img src='./assets/Vibe sharing.png' class="w-full h-auto object-cover rounded-lg">
  </div>
  
  <div v-click="3">
    <img src='./assets/image1.png' class="w-full h-auto object-cover rounded-lg">
  </div>
</div>


<div class="mt-20" v-click="2">
  <h2 class="text-2xl font-medium mb-4">快速调查：Vibe coding 出来的代码是否应该 review？</h2>
</div>

---
layout: cover
---
<div class="absolute inset-0">
  <img src="./assets/cover_4.png" class="w-full h-full object-cover" />
</div>

---
layout: default
---
<div class="flex flex-col">
  <h2 class="text-2xl font-medium mb-8">为什么 Vibe Coding 最后都只在做 Landing Page?</h2>
  <div>
    <img src='./assets/image4.png' class="w-full h-180 object-cover rounded-lg shadow-lg">
  </div>
</div>

---
layout: default
---

# What went wrong? 

<div class="grid grid-cols-3 gap-8 mt-8">
  <div class="flex justify-center">
    <img src="./assets/arch_1.png" class="w-auto h-180 object-cover rounded-lg shadow-lg">
  </div>
  
  <div class="flex flex-col gap-4 col-span-2">
    <img src="./assets/arch_2.png" class="w-460 h-120 object-cover rounded-lg shadow-lg">
    <img src="./assets/arch_3.png" class="w-460 h-50 object-cover rounded-lg shadow-lg" v-click>
  </div>
</div>

---
layout: two-cols
---

# What is vibe?

<div class="flex flex-col items-center justify-center h-full">
  <img src='./assets/vibe_hangzhou_sharing.jpg' class="w-full h-130 object-cover rounded-lg mb-4" v-click="1">
  <div class="text-center text-gray-600" v-click="2">
    <p class="font-medium mb-2">Cursor Meetup Hangzhou</p>
    <p>2025 年 7 月 12 日</p>
    <p class="italic">硅星人主编 王兆洋</p>
  </div>
</div>

::right::

<div class="flex flex-col items-center justify-center h-full">
  <img src='./assets/wordcloud_final.png' class="w-full h-140 object-cover" v-click="3">
  
  <div class="text-center" v-click="4">
    <h2 class="text-3xl font-bold text-[#5A6650]">
      <span class="text-4xl">Vibe</span> is all you need.
    </h2>
  </div>
</div>

---
layout: default
---

<div>
  <div class="col-span-2 flex justify-center items-center">
    <Youtube id="8tK3IxZG80k" :width="1000" :height="640" />
  </div>
</div>

<div class="mt-12 flex justify-center" v-click>
  <h2 class="text-4xl font-medium mb-4">即使你有毕加索的技术，你就能画出毕加索的画吗？</h2>
</div>

---
layout: default
---

# Vibe coder and painter

<div class="flex">
  <!-- Left column - 1/3 width -->
  <div class="w-2/5 pr-8" v-click="1">
    <img src="./assets/paul graham.jpg" class="w-full h-180 object-cover rounded-lg shadow-lg">
  </div>

  <!-- Right column - 2/3 width -->
  <div class="w-3/5 flex flex-col gap-6">
    <div class="p-6">
      <h3 class="text-5xl font-medium mb-4" v-click="2">创作者的共同点</h3>
      <ul class="space-y-4 text-3xl text-[#333333]" v-click="3">
        <li>黑客与画家都是创作者。对于想写出漂亮程序的黑客来说，计算机只是一种工具，就像画家的画笔 —— Paul Graham</li>
        <li>Vibe Coding 让我们每个人都成为了神笔马良。</li>
      </ul>
    </div>
    <div class="p-6">
      <h3 class="text-xl font-medium mb-4" v-click="4">真正的挑战</h3>
      <ul class="space-y-2 text-3xl text-[#333333]" v-click="5">
        <li> 如何管理色彩 <span class="text-[#5A6650]">(如何管理上下文)</span></li>
        <li> 补救还是重画 <span class="text-[#5A6650]">(硬聊还是重开)</span></li>
        <li> 内心的 Image <span class="text-[#5A6650]">(Vibe)</span></li>
      </ul>
    </div>
  </div>
</div>

---
layout: two-cols
---

# How to get vibes?

<div class="mt-24">
  <ul class="space-y-6 text-lg">
    <li v-click="1" class="text-4xl">不知道自己想要什么，这很正常</li>
    <li v-click="2" class="text-4xl">Good Artist Copy, Great Artist Steal</li>
    <li v-click="3" class="text-4xl">这句话其实是毕加索说的</li>
  </ul>
</div>

::right::

<div class="flex items-center justify-center h-full"v-click="2">
  <img src="./assets/jobs.jpg" class="w-full h-auto object-cover rounded-lg shadow-lg">
</div>

---
layout: default
---

# Case: My personal website

<div class="grid grid-cols-6 gap-8 h-full">
  <div class="col-span-2 flex flex-col justify-center gap-6">
    <div class="p-6">
      <h3 class="text-3xl font-medium mb-4">背景</h3>
      <p class="text-2xl text-[#333333]">换工作比较闲，想做一下个人网站</p>
    </div>
    <div class="p-6">
      <h3 class="text-3xl font-medium mb-4">第一版<a href="https://aabdoo23.vercel.app/" class="text-[#5A6650] hover:underline">尝试</a></h3>
    </div>
  </div>

  <div class="col-span-4 flex items-center justify-center">
    <div class="w-auto h-180 bg-white rounded-lg shadow-lg overflow-hidden">
      <img src="./assets/astro_v1.png" class="w-full h-full object-cover">
    </div>
  </div>
</div>

---
layout: default
---

# Inspiration
<div class="grid grid-cols-8 gap-8 h-full">
  <div class="col-span-4 flex items-center justify-center">
    <Youtube id="Ucct_YVl1tY" :width="800" :height="400" />
  </div>
  <div class="col-span-4 flex items-center justify-center">
    <img src='./assets/beijing.jpg' class="w-auto h-180 object-cover rounded-lg shadow-lg">
  </div>
</div>


---
layout: default
---

# What if...

<img src='./assets/ryos.png' class="w-auto h-180 object-cover rounded-lg shadow-lg">

---
layout: default
---

# Creating my own OS

<div class="flex flex-col gap-8">
  <div class="text-lg">
    <p class="mb-4" v-click="1">最初尝试：Mac System 7 风格</p> <p class="text-gray-600" v-click="2">AI 很擅长，但觉得没有意思</p>
  </div>

  <div>
    <h3 class="text-xl mb-6" v-click="3">灵感：Terry A. Davis TempleOS</h3>
    <div class="grid grid-cols-2 gap-8" v-click="4">
      <img 
        src='./assets/terry_davis.jpg' 
        class="w-full h-[500px] object-cover rounded-lg shadow-lg"
        alt="Terry A. Davis"
      >
      <img 
        src='./assets/TempleOS_4.05_session.png' 
        class="w-full h-[500px] object-cover rounded-lg shadow-lg"
        alt="TempleOS Screenshot"
      >
    </div>
  </div>

  <p class="mt-4 text-lg font-light text-center italic" v-click="5">
    过去需要花一辈子的事情，现在只需要几分钟
  </p>
</div>


---
layout: default
---

# Adding more elements
用 3D 大脑来组织项目？

<div>
  <div class="col-span-2 flex justify-center items-center">
    <Youtube id="Uss7_PGaFLQ" :width="1200" :height="700" />
  </div>
</div>

---
layout: default
---

# I could create whatever I want
<div class="grid grid-cols-3 gap-16">
  <div class="flex flex-col justify-start space-y-12">
    <div class="text-3xl space-y-6" v-click="1">
      <p class="font-bold">理念的转变：</p>
      <p class="mt-8">你可以做你想到的一切</p>
      <p class="mt-8">限制你的只有想象力</p>
    </div>
    <div>
      <p class="text-2xl mb-6" v-click="2">加入那些真正喜欢的元素：</p>
      <div class="grid gap-4">
        <div class="p-4 bg-gray-50/10 rounded-lg hover:bg-gray-50/20 transition-colors duration-300" v-click="3">
          <h3 class="text-xl font-light">凌晨的海面，极光</h3>
        </div>
        <div class="p-4 bg-gray-50/10 rounded-lg hover:bg-gray-50/20 transition-colors duration-300" v-click="4">
          <h3 class="text-xl font-light">极乐迪斯科的对话框</h3>
        </div>
        <div class="p-4 bg-gray-50/10 rounded-lg hover:bg-gray-50/20 transition-colors duration-300" v-click="5">
          <h3 class="text-xl font-light">The Ape of Naples的封面</h3>
        </div>
      </div>
    </div>
  </div>

  <div class="grid grid-cols-2 gap-6 h-[500px] col-span-2" v-click="4">
    <img 
      src='./assets/disco_elysium.jpg' 
      class="w-300 h-full object-cover rounded-xl shadow-xl hover:scale-105 transition-transform duration-300"
      alt="Disco Elysium dialogue interface"
    >
    <div class="flex flex-col gap-6" v-click="6">
      <img 
        src='./assets/apeofnaples.webp'
        class="w-full h-1/2 object-cover rounded-xl shadow-xl hover:scale-105 transition-transform duration-300"
        alt="The Ape of Naples album cover"
      >
      <img 
        src='./assets/ape3d.png'
        class="w-full h-1/2 object-cover rounded-xl shadow-xl hover:scale-105 transition-transform duration-300"
        alt="3D visualization"
      >
    </div>
  </div>
</div>

---
layout: default
---

# Toolkit

<div class="grid grid-cols-2 gap-24 mt-8 h-full">
  <!-- Left: Tools Used -->
  <div class="flex flex-col justify-start pt-16 gap-16" v-click="1">
    <h3 class="text-6xl font-bold mb-8 text-[#1A1A1A]">🛠️ 我使用的工具</h3>
    <ul class="space-y-12">
      <li class="flex items-center gap-6">
        <div class="i-carbon:code text-4xl text-[#5A6650]" />
        <span class="text-4xl">Cursor + Roo code + Claude code</span>
      </li>
      <li class="flex items-center gap-6">
        <div class="i-carbon:earth text-4xl text-[#5A6650]" />
        <span class="text-4xl">除了联网搜索没有别的 MCP</span>
      </li>
    </ul>
  </div>
  <!-- Right: Overlooked Steps -->
  <div class="flex flex-col justify-start pt-16 gap-16" v-click="2">
    <h3 class="text-6xl font-bold mb-8 text-[#1A1A1A]">✨ 杀手锏</h3>
    <ul class="space-y-12">
      <li class="flex items-center gap-6">
        <div class="i-carbon:idea text-4xl text-[#5A6650]" />
        <span class="text-4xl">通过 Roo Code 进行 AI 头脑风暴</span>
      </li>
      <li class="flex items-center gap-6">
        <div class="i-carbon:checkbox text-4xl text-[#5A6650]" />
        <span class="text-4xl">做选择题而不是写作文</span>
      </li>
    </ul>
  </div>
</div>

---
layout: default
---

# Thoughts

<div class="flex flex-col justify-center h-full gap-12 mt-16">
  <div class="p-8" v-click="1">
    <div class="flex items-center gap-6">
      <div class="i-carbon:idea text-4xl text-[#5A6650]"></div>
      <span class="text-3xl">强迫自己不去改代码，锻炼自己的 prompt 能力</span>
    </div>
  </div>

  <div class="p-8" v-click="2">
    <div class="flex items-center gap-6">
      <div class="i-carbon:face-satisfied text-4xl text-[#5A6650]"></div>
      <span class="text-3xl">你可以不喜欢它，但你要了解它</span>
    </div>
  </div>

  <div class="p-8" v-click="3">
    <div class="flex items-center gap-6">
      <div class="i-carbon:shuffle text-4xl text-[#5A6650]"></div>
      <span class="text-3xl">拥抱不确定性，随机是创意的源泉</span>
    </div>
  </div>

  <div class="p-8" v-click="4">
    <div class="flex items-center gap-6">
      <div class="i-carbon:code text-4xl text-[#5A6650]"></div>
      <span class="text-3xl">使用 code-based 方案，而不是 UI-based 方案 (e.g. SuperCollider vs Ableton)</span>
    </div>
  </div>

  <div class="p-8" v-click="5">
    <div class="flex items-center gap-6">
      <div class="i-carbon:group text-4xl text-[#5A6650]"></div>
      <span class="text-3xl">多看别人的项目，从中获得启发</span>
    </div>
  </div>
</div>

---
layout: default
---

# Youware: Vibe coder's community

<div class="grid grid-cols-3 gap-24 h-full items-center mt-8">
  <!-- Left: Text (1/3) -->
  <div class="flex col-span-1 flex-col justify-center py-12">
    <div class="text-3xl font-medium leading-relaxed">
      <span class="mb-2 block" v-click="1">大部分人都是先看见再相信</span>
      <span class="text-[#5A6650]" v-click="2">所以要先让他们看见</span>
    </div>
  </div>
  
  <!-- Right: Image (2/3) -->
  <div class="col-span-2 flex items-center justify-center" v-click="2">
    <img src="./assets/youware.png" class="w-auto h-170 object-contain">
  </div>
</div>

---
layout: default
---

# Support us
<div class="flex items-center justify-center">
  <img src="./assets/producthunt.jpg" class="w-auto h-170 object-contain">
</div>