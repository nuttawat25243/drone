<template>
  <div>
    <Package></Package>
    <Gallery></Gallery>
    <Team></Team>
    <Contact></Contact>
    <Navigator></Navigator>
  </div>
</template>

<script>
import Gallery from '@/components/Gallery.vue';
import Team from '@/components/Team.vue';
import Contact from '@/components/Contact.vue';
import Navigator from '@/components/Navigator.vue';
import Package from '@/components/Package.vue';

export default {
  name: 'IndexPage',

  components: {
    Gallery,Team,Contact,Navigator,Package,
  },
}
</script>

<style scoped>
</style>
