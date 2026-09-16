<script setup lang="ts">
import { useIsSlideActive } from '@slidev/client'

// Omarchy's own wordmark, as shipped in ~/.local/share/omarchy/logo.txt
const logo = `                 ▄▄▄
 ▄█████▄    ▄███████████▄    ▄███████   ▄███████   ▄███████   ▄█   █▄    ▄█   █▄
███   ███  ███   ███   ███  ███   ███  ███   ███  ███   ███  ███   ███  ███   ███
███   ███  ███   ███   ███  ███   ███  ███   ███  ███   █▀   ███   ███  ███   ███
███   ███  ███   ███   ███ ▄███▄▄▄███ ▄███▄▄▄██▀  ███       ▄███▄▄▄███▄ ███▄▄▄███
███   ███  ███   ███   ███ ▀███▀▀▀███ ▀███▀▀▀▀    ███      ▀▀███▀▀▀███  ▀▀▀▀▀▀███
███   ███  ███   ███   ███  ███   ███ ██████████  ███   █▄   ███   ███  ▄██   ███
███   ███  ███   ███   ███  ███   ███  ███   ███  ███   ███  ███   ███  ███   ███
 ▀█████▀    ▀█   ███   █▀   ███   █▀   ███   ███  ███████▀   ███   █▀    ▀█████▀
                                       ███   █▀`

const active = useIsSlideActive()
</script>

<template>
  <div class="omarchy-logo">
    <!-- keyed on slide activation so the draw-in replays every time you arrive -->
    <pre v-if="active" :key="String(active)" class="art">{{ logo }}</pre>
    <pre v-else class="art art--idle">{{ logo }}</pre>
  </div>
</template>

<style scoped>
.omarchy-logo {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}

.art {
  margin: 0;
  padding: 0;
  background-color: transparent;
  font-family: 'JetBrains Mono', 'Fira Code', ui-monospace, monospace;
  font-size: 15px;
  line-height: 1;
  white-space: pre;
  overflow: visible;

  /* a bright band sweeps across the letters */
  color: transparent;
  background-image: linear-gradient(
    100deg,
    #5eead4 0%,
    #60a5fa 35%,
    #ffffff 50%,
    #60a5fa 65%,
    #5eead4 100%
  );
  background-size: 250% 100%;
  -webkit-background-clip: text;
  background-clip: text;

  animation:
    draw-in 1.6s steps(81, end) both,
    shimmer 3.5s linear 1.6s infinite;
}

.art--idle {
  animation: none;
  clip-path: inset(0 100% 0 0);
}

@keyframes draw-in {
  from { clip-path: inset(0 100% 0 0); }
  to   { clip-path: inset(0 0 0 0); }
}

@keyframes shimmer {
  from { background-position: 100% 0; }
  to   { background-position: -150% 0; }
}

@media (prefers-reduced-motion: reduce) {
  .art { animation: none; clip-path: none; }
}
</style>
