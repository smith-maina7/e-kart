<template>
  <header>
    <nav>
      <Nav />
    </nav>
  </header>
  <router-view />
</template>
<script setup>
import Nav from "@/components/Nav-bar.vue";
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@300&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  background-color: rgb(243, 241, 241);
}
header {
  position: sticky;
  top: 0;
  width: 100%;
  z-index: 99;
}
</style>
