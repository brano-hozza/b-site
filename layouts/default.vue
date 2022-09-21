<template>
  <div>
    <header class="w-full h-10 flex justify-start bg-slate-300">
      <nav class="flex flex-row items-center">
        <h3 class="mx-2"><b>B</b>-Site</h3>
        <ul class="flex items-center justify-start">
          <li class="h-4/5 inline mr-2 px-2 text-white" :class="[route.path === '/dashboard' ? 'bg-slate-400' : 'bg-slate-500']">
            <a href="/dashboard">Dashboard</a>
          </li>
          <li class="h-4/5 inline mr-2 px-2 text-white" :class="[route.path === '/about' ? 'bg-slate-400' : 'bg-slate-500']">
            <a href="/about">About</a>
          </li>
          <li class="h-4/5 inline mr-2 px-2 text-white" :class="[route.path === '/contact' ? 'bg-slate-400' : 'bg-slate-500']">
            <a href="/contact">Contact</a>
          </li>
        </ul>
      </nav>
    </header>
    <section class="min-h-screen">
      <slot />
    </section>
    <aside></aside>
    <footer class="w-full bg-slate-600 h-10 justify-center align-middle flex">
      <p class="text-white">Copyright 2022 Branislav Hozza</p>
    </footer>
  </div>
</template>
<script setup lang="ts">
const route = useActiveRoute();
</script>
<style lang="scss"></style>
