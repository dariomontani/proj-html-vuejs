<template>
  <header>
      <Navbar />
      <Jumbo />
  </header>
</template>

<script>
import Navbar from './Navbar.vue';
import Jumbo from './Jumbo.vue';


export default {
  name: "Header",
  components: {
    Navbar,
    Jumbo,
  },
}
</script>

<style lang="scss" scope>

</style>