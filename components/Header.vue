<template>
<header class="shadow flex items-center justify-between h-16 px-8 text-gray-500">

<!-- Left logo -->
<div>
  <nuxt-link to="/">
    <NuxtLogo class="w-6 h-6"/>
  </nuxt-link>
</div>

<!-- Search -->
<div>
  <input type="search" placeholder="Type search.." class="px-5 py-2 rounded bg-gray-50 w-64 border-none">
</div>

<!-- right side -->
<div>
    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9" />
  </svg>
</div>

</header>
</template>

<script>
import NuxtLogo from './NuxtLogo.vue'
export default {
  components: { NuxtLogo },

}
</script>

<style>

</style>