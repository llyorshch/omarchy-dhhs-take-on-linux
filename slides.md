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
    <p class="!text-3xl !leading-snug opacity-70 !mt-6">Isn't it just another Linux distro that will soon be forgotten?</p>
  </div>
  <img src="/why.svg" alt="A woman with her hand on her chin, wondering: Why?" class="w-full" />
</div>


---

# DHH's and Omarchy's uniqueness
- DHH is disruptive and does not sacrifice his vision for the sake of consensus
- Now, DHH is focused in Linux. Macs are no longer good. 
- DHH is a developer with strong developer opinions
- DHH has traction between developers --> [GH contributions](https://github.com/omacom/omarchy/graphs/contributors?from=9%2F19%2F2024&to=1%2F1%2F2026) 
- DHH can raise a lot of funding --> [Omacon Patrons](https://omarchy.org/patrons/)
- Omarchy was born during the explosion of agentic development

---
layout: center
class: text-center
---

# Thank you!

Questions?
