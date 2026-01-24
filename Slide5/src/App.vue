<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Slide5 from './components/Slide5.vue';

</script>

<template>
  <!-- <HelloWorld msg="tran quang binh" /> -->
  <Slide5 msg2="Binh"/>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
