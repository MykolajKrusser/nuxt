<template>
  <nav class="flex mx-auto">
    <ul class="flex gap-4">
      <li><nuxt-link to="/">Home</nuxt-link></li>
      <li><nuxt-link to="/beer-list">Beer list</nuxt-link></li>
    </ul>
  </nav>
</template>

<script lang="ts">
export default {
  name: 'MainNavigation'
}
</script>

<style>
  .nuxt-link-exact-active{
    text-decoration: underline;
  }
</style>