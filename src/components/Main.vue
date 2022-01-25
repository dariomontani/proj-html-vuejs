<template>
  <main>
    <Cards />
    <Cit />
    <Specials />
    <BuildPizza />
    <People />
    <Clients />
    <BestPizza />
    <TypeOfPizza />
    <DelishPizza />
    <Booking />
  </main>
</template>

<script>
import Cards from './Cards.vue';
import Cit from './Cit.vue';
import Specials from './Specials.vue';
import BuildPizza from './BuildPizza.vue';
import People from './People.vue';
import Clients from './Clients.vue';
import BestPizza from './BestPizza.vue';
import TypeOfPizza from './TypeOfPizza.vue';
import DelishPizza from './DelishPizza.vue';
import Booking from './Booking.vue';

export default {
    name: "Main",
    components: {
    Cards,
    Cit,
    Specials,
    BuildPizza,
    People,
    Clients,
    BestPizza,
    TypeOfPizza,
    DelishPizza,
    Booking,
  },
}
</script>

<style lang="scss" scope>

</style>