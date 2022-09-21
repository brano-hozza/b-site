<template>
  <header>
    <nav>
      <ul>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
      </ul>
    </nav>
  </header>
  <section>
    <slot />
  </section>
  <aside></aside>
  <footer>
    <p>Copyright 2022 Branislav Hozza</p>
  </footer>
</template>

<script setup lang="ts"></script>

<style scoped></style>
