<script setup>
import logoUrl from './assets/oxocode-logo.svg'
</script>

<template>
  <main class="hero">
    <img :src="logoUrl" alt="OxoCode logo" class="logo" />
    <h1>Coming soon</h1>
    <p>We are crafting something amazing. Stay tuned!</p>
    <a class="github" href="http://github.com/oxo-code" target="_blank" rel="noopener">
      GitHub
    </a>
  </main>
</template>

<style scoped>
.hero {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 1.5rem;
  text-align: center;
  color: #f7f7f7;
}

.logo {
  width: min(320px, 60vw);
}

h1 {
  font-size: clamp(2.5rem, 6vw, 3.5rem);
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

p {
  max-width: 34rem;
  font-size: 1.125rem;
  color: #d0d0d0;
}

.github {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 0.75rem 1.75rem;
  border-radius: 999px;
  background: linear-gradient(135deg, #f78b2d, #ffb057);
  color: #101010;
  font-weight: 600;
  text-decoration: none;
  transition: transform 150ms ease, box-shadow 150ms ease;
}

.github:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 25px rgba(247, 139, 45, 0.35);
}

.github:focus-visible {
  outline: 2px solid #f78b2d;
  outline-offset: 4px;
}
</style>
