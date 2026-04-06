<script setup>
import { onMounted } from "vue";
import HelloWorld from './components/HelloWorld.vue'

onMounted(() => {
  fetch("http://localhost:3000/api/hello")
    .then(res => res.json())
    .then(data => console.log(data));
});
</script>

<template>
  <HelloWorld />
</template>
