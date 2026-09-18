---
theme: default
title: "Omarchy: DHH's take on Linux"
info: |
  A presentation about Omarchy, DHH's Linux distribution.
transition: slide-left
mdc: true
---

<h1 class="!text-8xl !font-bold !mb-6">Omarchy</h1>

<p class="!text-4xl opacity-80">DHH's take on Linux</p>

---

<div class="h-full grid grid-cols-2 gap-10 items-center">
  <h1 class="!text-6xl !font-bold !leading-tight">First, the basics, in case you've been living under a rock</h1>
  <img src="/under-a-rock.svg" alt="A confused creature peeking out from under a rock, asking Who's DHH?" class="w-full" />
</div>

---

<div class="flex items-center gap-6">
  <img src="/dhh.jpg" alt="David Heinemeier Hansson" class="w-32 h-32 rounded-full object-cover flex-none shadow-lg" />
  <div>
    <h1 class="!mb-0">Who is DHH?</h1>
    <p class="opacity-60 !mt-1">David Heinemeier Hansson</p>
  </div>
</div>

<div class="grid grid-cols-2 gap-x-10 gap-y-3 pt-8">

<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">💎</span>
    <span class="font-bold text-lg">Ruby on Rails</span>
  </span>
  <span class="opacity-60 text-sm">2004 &middot; still project lead today</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">🏢</span>
    <span class="font-bold text-lg">37signals</span>
  </span>
  <span class="opacity-60 text-sm">co-founder &amp; CTO &middot; Basecamp, HEY, ONCE</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">📚</span>
    <span class="font-bold text-lg">REWORK</span>
  </span>
  <span class="opacity-60 text-sm">NYT bestseller &middot; four books with Jason Fried</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">🏆</span>
    <span class="font-bold text-lg">Best Hacker 2005</span>
  </span>
  <span class="opacity-60 text-sm">Google &amp; O&rsquo;Reilly award, for Rails</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">🏁</span>
    <span class="font-bold text-lg">Le Mans</span>
  </span>
  <span class="opacity-60 text-sm">class win, LMGTE Am &middot; 2014</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">☁️</span>
    <span class="font-bold text-lg">Leaving the cloud</span>
  </span>
  <span class="opacity-60 text-sm">off AWS &middot; ~$2M/year saved, numbers published</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">🍎</span>
    <span class="font-bold text-lg">Beating Apple</span>
  </span>
  <span class="opacity-60 text-sm">HEY vs the App Store &middot; 2020 &middot; Apple blinked</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">🐧</span>
    <span class="font-bold text-lg">Omakub &rarr; Omarchy</span>
  </span>
  <span class="opacity-60 text-sm">2024 &middot; started at Le Mans, between sessions</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">🤖</span>
    <span class="font-bold text-lg">Omarchy Quattro</span>
  </span>
  <span class="opacity-60 text-sm">1,000+ PRs merged in three months</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-64 flex-none flex items-baseline gap-1.5">
    <span class="text-lg">✍️</span>
    <span class="font-bold text-lg">The manifestos</span>
  </span>
  <span class="opacity-60 text-sm">Omakase &middot; Rails Doctrine &middot; TDD is Dead</span>
</div>

</div>

<!--
The achievements, in rough order of how much they built his name.

Ruby on Rails (2004) - the headline. Extracted from the Basecamp codebase rather
than designed in the abstract. Popularised convention over configuration and made
Ruby mainstream almost single-handedly. GitHub, Shopify, Airbnb, Square, Zendesk,
Coinbase and early Twitter all built on it. Twenty years on, still project lead.

37signals - co-founder and CTO with Jason Fried. Basecamp, HEY (email, 2020),
ONCE (software you buy once and host yourself instead of renting forever).
Deliberately small, profitable, no venture capital.

Books - REWORK hit the NYT bestseller list. Also Getting Real, REMOTE, and
It Doesn't Have to Be Crazy at Work. These reached people who will never write
a line of code, and did as much for his profile as Rails did.

Best Hacker of the Year 2005 - awarded by Google and O'Reilly for Rails.

Le Mans - a serious second career, not a hobby. Raced the 24 Hours multiple times
and took a class win in LMGTE Am in 2014.

Leaving the cloud (2022-23) - moved 37signals off AWS back onto own hardware and
published the numbers, around $2M/year saved. Open-sourced the tooling (Kamal).
Ran straight against industry consensus and forced a real debate.

Beating Apple (2020) - Apple threatened to pull HEY from the App Store over
in-app purchase rules. He took it public, loudly. Apple backed down and adjusted
its rules; it fed into the wider regulatory pressure on app store economics.

Omakub then Omarchy - Omakub came first, on Ubuntu. Omarchy went "seven layers
deeper down the stack", onto Arch and Hyprland. He started it in summer 2024
between sessions at the 24 Hours of Le Mans, after watching too many Linux
ricing videos.

Omarchy Quattro - the current version, according to him built essentially
entirely by AI agents under his direction. 1,000+ pull requests merged in three
months, many from contributors who are not traditional programmers.

The manifestos - Rails is Omakase, The Rails Doctrine, TDD is Dead. Each one
started a fight that consumed the industry for months. He writes as well as he
codes, and that is the underrated half of the story.

Not on the slide, but say it if asked: the controversies are real and
inseparable from the fame. The 2021 Basecamp ban on political discussion at work
cost roughly a third of the staff.
-->

---

<div class="flex items-center gap-6">
  <img src="/dhh.jpg" alt="David Heinemeier Hansson" class="w-32 h-32 rounded-full object-cover flex-none shadow-lg" />
  <div>
    <h1 class="!mb-0">What is DHH like?</h1>
    <p class="opacity-60 !mt-1">David Heinemeier Hansson</p>
  </div>
</div>

<div class="grid grid-cols-2 gap-x-10 gap-y-3 pt-8">

<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🗣️</span>
    <span class="font-bold text-xl">Persuasive</span>
  </span>
  <span class="opacity-60 text-sm">doesn't argue, converts</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🔥</span>
    <span class="font-bold text-xl">Vehement</span>
  </span>
  <span class="opacity-60 text-sm">no lukewarm register</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🍣</span>
    <span class="font-bold text-xl">Opinionated</span>
  </span>
  <span class="opacity-60 text-sm">chooses for you, by design</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🔄</span>
    <span class="font-bold text-xl">Reversible</span>
  </span>
  <span class="opacity-60 text-sm">changes his mind in public</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">📦</span>
    <span class="font-bold text-xl">Prolific</span>
  </span>
  <span class="opacity-60 text-sm">the output is real</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🎨</span>
    <span class="font-bold text-xl">Aesthetic</span>
  </span>
  <span class="opacity-60 text-sm">taste over technique</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🙃</span>
    <span class="font-bold text-xl">Contrarian</span>
  </span>
  <span class="opacity-60 text-sm">allergic to consensus</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🌶️</span>
    <span class="font-bold text-xl">Provocative</span>
  </span>
  <span class="opacity-60 text-sm">seeks the friction</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🌹</span>
    <span class="font-bold text-xl">Romantic</span>
  </span>
  <span class="opacity-60 text-sm">thinks in epics, not metrics</span>
</div>
<div v-click class="flex items-baseline gap-3">
  <span class="w-52 flex-none flex items-baseline gap-1.5">
    <span class="text-xl">🪞</span>
    <span class="font-bold text-xl">Self-indulgent</span>
  </span>
  <span class="opacity-60 text-sm">the flip side of all of it</span>
</div>

</div>

<!--
My read on David, based on the Lex Fridman interview (#501) and his public track record.

1. **Persuasive** — he doesn't argue, he converts. He's mastered the "I brought the pudding" rhetoric: no abstract debate, just a product downloaded by tens of thousands of people put on the table.

2. **Vehement** — he has no lukewarm register. Everything comes out in superlatives ("freaking amazing", "delirious", "the perfect computer").

3. **Opinionated** — literally his design trademark. Rails, Omarchy and his way of speaking share the same principle: I choose for you, and if you don't like it, there are other options.

4. **Reversible** — the most interesting thing about him. He went from declared AI skeptic to evangelist in months, and he admits it out loud ("nine months ago I would have used the label AI psychosis myself"). Plenty of people with his public ego don't do that.

5. **Prolific** — 1,000+ PRs in three months, an operating system barely a year old, a framework holding up half the web. The output is real, not rhetorical.

6. **Aesthetic** — his primary criterion isn't technical, it's taste. Omarchy wasn't born from a functional need; it was born from watching Linux ricing videos and wanting something beautiful.

7. **Contrarian** — he systematically positions himself against consensus: leaving the cloud, against VC, against DEI statements, and now pro-AI while his tribe (open source) is largely hostile.

8. **Provocative** — he actively seeks friction; his Overton window theory is transparently a justification of his own public fighting style.

9. **Romantic** — in the nineteenth-century sense: race cars, amor fati, stoicism, the Commodore 64, fatherhood as the peak human experience. He thinks in images and epics, not metrics.

10. **Self-indulgent** — the flip side of all the above. His defense of Linus and Elon ("who am I to judge?", harshness justified by the size of the mission) is transparently a defense of himself, and his extrapolation from "I built a distro with agents" to "this is how all software will be" skips quite a few steps.

In one sentence: a genuine builder with exceptional instincts for taste and a rare ability to change his mind in public, wrapped in a rhetoric of absolutes worth discounting by about 30% — but discounting it entirely would be the mistake, because historically he's been right about the direction even when he overstates the magnitude.

Bridge to the next slide: Omarchy doesn't make sense as a technical decision, it makes sense as a decision about TASTE.
-->

---

<div class="h-full flex flex-col">

# What is Omarchy?

<p class="text-2xl leading-relaxed !mt-6 opacity-90">
A beautiful, opinionated Linux desktop by DHH, built on Arch and Hyprland and fully set up out of the box.
</p>

<div class="flex-1 min-h-0">
  <OmarchyLogo />
</div>

</div>

---

<div class="h-full grid grid-cols-2 gap-10 items-center">
  <div>
    <h1 class="!text-5xl !font-bold !leading-tight">OK, but why are we even talking about DHH and Omarchy?</h1>
  </div>
  <img src="/why.svg" alt="A woman with her hand on her chin, wondering: Why?" class="w-full" />
</div>


---

# DHH's and Omarchy's uniqueness 💎

<v-clicks>

- He is disruptive, and never trades his vision for consensus
- His focus is now Linux &mdash; in his view, the Mac has stopped being good
- He is a developer, with strong developer opinions
- He has real traction among developers &mdash; [GitHub contributors](https://github.com/omacom/omarchy/graphs/contributors?from=9%2F19%2F2024&to=1%2F1%2F2026)
- He can raise serious money &mdash; [Omarchy patrons](https://omarchy.org/patrons/)
- And Omarchy was born right as agentic development exploded

</v-clicks>

<div v-click class="pt-8">
  <p class="!text-4xl !font-bold !leading-tight text-teal-600">
    Will DHH and Omarchy win the Linux desktop, as they claim?
  </p>
</div>

<!--
Six reasons this is not just another distro. The last one is the argument that
ties the talk together: the timing is what makes it different.

Traction: 41,700+ stars on omacom/omarchy, and DHH says 1,000+ pull requests
merged in three months, many from people who are not traditional programmers.

On the Mac: his complaint is that a locked-down, curated platform is a hostile
place for agents and development work. In the interview: "the Mac is just a
hostile place to be. It just has walls all over the place." The irony he enjoys
is that Linux's supposed flaws - arcane config files, cryptic errors - are
exactly what agents handle well.
-->
---

# Omarchy timeline

<div class="h-full flex items-center">
<div class="relative w-full">

  <div class="absolute left-0 right-0 top-1/2 -translate-y-1/2 h-1 bg-gray-200 rounded"></div>

  <div class="relative grid grid-cols-7 gap-1">
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"><div class="text-xs font-bold text-teal-600">May 2024</div><div class="font-bold text-sm leading-tight">Omakub</div><div class="text-xs opacity-50 leading-tight">the first attempt, on Ubuntu</div></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"></div>
  </div>
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"><div class="text-xs font-bold text-teal-600">Jun 2025</div><div class="font-bold text-sm leading-tight">Omarchy</div><div class="text-xs opacity-50 leading-tight">restarted on Arch + Hyprland</div></div>
  </div>
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"><div class="text-xs font-bold text-teal-600">Jul 2025</div><div class="font-bold text-sm leading-tight">v1.0</div><div class="text-xs opacity-50 leading-tight">first public releases</div></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"></div>
  </div>
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"><div class="text-xs font-bold text-teal-600">Aug 2025</div><div class="font-bold text-sm leading-tight">v2.0</div></div>
  </div>
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"><div class="text-xs font-bold text-teal-600">Sep 2025</div><div class="font-bold text-sm leading-tight">v3.0</div></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"></div>
  </div>
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"><div class="text-xs font-bold text-teal-600">Aug 2026</div><div class="font-bold text-sm leading-tight">v4.0 Quattro</div><div class="text-xs opacity-50 leading-tight">built by agents, start to finish</div></div>
  </div>
  <div v-click class="flex flex-col items-center">
    <div class="h-28 w-full flex flex-col justify-end items-center text-center pb-3"><div class="text-xs font-bold text-teal-600">Today</div><div class="font-bold text-sm leading-tight">v4.0.4</div><div class="text-xs opacity-50 leading-tight">41,700+ stars</div></div>
    <div class="w-4 h-4 rounded-full bg-teal-500 ring-4 ring-white flex-none"></div>
    <div class="h-28 w-full flex flex-col justify-start items-center text-center pt-3"></div>
  </div>
  </div>

</div>
</div>

<!--
Dates come from the GitHub repos, not from memory.

May 2024 - omacom/omakub created. The Ubuntu-based first attempt, now retired;
DHH calls it "fine", but he was building on someone else's foundation.

June 2025 - omacom/omarchy created. Restarted "seven layers deeper down the
stack" on Arch and Hyprland, begun between sessions at the 24 Hours of Le Mans.

July to September 2025 - v1, v2 and v3 in roughly a month each. Note the pace:
three major versions in three months, still largely hand-written at the start.

August 2026 - v4.0, Quattro. The version DHH says was written essentially
entirely by agents under his direction. This is the point of the whole talk.

Today - v4.0.4, 41,700+ stars. Omakub has about 8,000 by comparison.

If asked why v3 to v4 took eleven months while v1 to v3 took three: the earlier
numbers were small increments, and Quattro was a much larger rebuild.
-->

---
class: text-white
---

<img src="/quattro.jpg" alt="" class="absolute inset-0 w-full h-full object-cover" />
<div class="absolute inset-0 bg-black/60"></div>

<div class="relative">

# Omarchy Quattro

<v-clicks>

- Full Quickshell-based desktop shell
- [Omarchy plugins](https://plugins.omarchy.org/)
- Dual boot
- Setup for a different owner and factory reset
- ISO under 6GB
- Sub-minute installs are possible

</v-clicks>

</div>


---


# Omarchy's Quirks and Features 🛠️
<v-clicks>

- Arch + Hyprland + Quickshell
- Arch packages + AUR + mise
- The Omarchy Menu
- The top bar
- Themes
- Backgrounds
- Terminal
- Neovim
- GUIs and TUIs 
</v-clicks>
---

# Omarchy and AI 🍑
<v-clicks>


- All major coding agents pre-wired in the launcher and managed by mise
- "Default agent" integrated
- The Omarchy skill (and all desktop shell and tools AI-friendly)
- Top bar AI bot icon
- Dictation
- Caffeine
</v-clicks>


<img v-click src="/face-rub.jpg" alt="An overwhelmed man rubbing his face with both hands" class="absolute right-10 bottom-10 w-52 drop-shadow-xl" />

---

# Omarchy - The Gripes 🫤
<v-clicks>


- Bloatware: 1Password, Basecamp, Hey, Spotify, X. (even with keyboard shortcuts!)
- Learning curve, specially to keep your hand away from the mouse
- You can't just hand your computer to anyone
- The fanboys. (Mostly ex-Apple fanboys? 🤔)
- If you don't like DHH, you need to accept to separate the artist from his work
</v-clicks>

---

# Omarchy - The Joys 🚀
<v-clicks>

- Once you get used to it, it's addictive.
- It's fast! Even in old Intel Macbooks.
- Nice backgrounds, nice fonts, nice retro-style aesthetic.
- Claude fixed Display configuration, Soundcard performance, Bluetooth, Wifi and keyboard backlight. AWESOME.
- Gaming! Steam, Retroarch, Minecraft...
</v-clicks>


---
layout: center
class: text-center
---

<h1 class="!text-6xl !font-bold !leading-tight">Will DHH and Omarchy win the Linux desktop?</h1>

---
layout: center
class: text-center
---

<p class="!text-[16rem] !font-black !leading-none !my-0">No.</p>

---
layout: center
class: text-center
---

<p class="!text-3xl !my-0">but</p>

---

<div class="h-full flex items-center">
<div class="text-2xl leading-relaxed space-y-6">

<p>Every contribution to open source software adds up. <strong>Hyprland</strong>, <strong>Mise</strong> and others will get funding that other distributions will benefit from.</p>

<p>Omarchy is setting the foundation for other distributions, especially in the way AI is integrated as a first-class citizen.</p>

<p>Future Linux distributions &mdash; not driven by DHH, AI-first, and aimed beyond developers &mdash; will be built on top of Omarchy's ideas.</p>

</div>
</div>

<!--
The turn of the talk. "No" is the honest answer on market share: the desktop
Linux numbers are not going to flip, and claiming otherwise would cost you the
room. But that is the wrong scoreboard.

The argument: Omarchy's contribution is upstream and conceptual, not measured in
installs. Funding flows to Hyprland, Mise and the rest of the stack, and every
other distribution inherits that work. The AI-as-first-class-citizen design is
the part that gets copied.

Land it plainly: whoever eventually does win the Linux desktop will be standing
on ideas that Omarchy proved first.
-->

---
layout: center
class: text-center
---

# Thank you!

Questions?
