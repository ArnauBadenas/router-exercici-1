<script setup lang="ts">
import { ref, watch, type Ref, watchEffect } from 'vue';

const input = ref(null)

</script>
  
<template>
  <main>
    <h1>Search</h1>
    <input type="search" name="search" id="search" v-model="input">
    <RouterLink :to="{path:'/results', query: { input } }">Search</RouterLink>
  </main>
</template>
