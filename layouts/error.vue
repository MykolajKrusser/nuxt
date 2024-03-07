<template>
  <div class="text-center h-full px-3 py-10">
    <strong>Error - {{error.message}}</strong>
  </div>
</template>

<script lang="ts">
export default {
  props:{
    error: {
      type: Object,
      default: null
    }
  }
}
</script>