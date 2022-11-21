<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="app">
    <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </header>
    <main>
      <RouterView />
    </main>
    <footer>
      <p>
        SunbearDay Project Template (2022)
      </p>
    </footer>
  </div>

</template>

<style scoped>
.app {
  height: 100%;
  margin-inline: auto;
  max-width: 65ch;
  padding-inline: 1em;
}

nav {
  align-items: center;
  display: flex;
  gap: 1em;
  justify-content: center;
  min-height: 4rem;
}

/* Update active links after colors are populated. */
nav a.router-link-exact-active {
  color: var(--color-text);
}
nav a.router-link-exact-active:hover {
  background-color: transparent;
}


nav a {
  color: var(--color-black);
  text-decoration: none;
}

main {
  height: 100%;
}

footer {
  padding-block: 2em;
  text-align: center;
}

</style>