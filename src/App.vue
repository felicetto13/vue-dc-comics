<template>
<div id="app">
  <TheHeader></TheHeader>
  <main>
    <div class="main-content">
      Aggiungi contenuto qui
    </div>
  </main>
  <TheFooter></TheFooter>
</div>
</template>

<script>

import TheHeader from "./components/TheHeader.vue"
import TheFooter from "./components/TheFooter.vue"


export default {
  name: 'App',
  components: {
    TheHeader, TheFooter
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.main-content {
  background-color: black;
  color: white;
  font-size: 30px;
  text-align: center;
  padding: 5rem 0;
}
</style>
