<template>
  <main>
    <Cards />
    <Cit />
    <Specials />
  </main>
</template>

<script>
import Cards from './Cards.vue';
import Cit from './Cit.vue';
import Specials from './Specials.vue';


export default {
    name: "Main",
    components: {
    Cards,
    Cit,
    Specials,
  },
}
</script>

<style lang="scss" scope>

</style>