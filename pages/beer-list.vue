<template>
  <div>
    <h1 class="text-4xl text-center py-4">
      Beer list
    </h1>
    <div>
      <ul class="flex flex-wrap">
        <li class="w-1/4" v-for="brewer in breweriesList">
          {{brewer.name}}
        </li>
      </ul>
    </div>
  </div>
</template>


<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Beer',
  head(){
    return{
      title: 'Beer list',
      meta: [
        {
          hid: "description",
          name: "description",
          content:"Beer list of random beer companies"
        },
        {
          hid: "og:description",
          name: "og:description",
          content:"Beer list of random beer companies"
        }
      ]
    }
  },
  async asyncData(context){
    const breweriesList = await context.app.$axios.$get('https://api.openbrewerydb.org/v1/breweries')
    return {breweriesList}
  }
})
</script>