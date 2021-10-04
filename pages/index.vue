<template>
  <section>
    <Navigation />
    <Gallery />
  </section>
</template>

<script>
import Gallery from '~/components/Gallery.vue'
import Navigation from '~/components/Navigation.vue'
export default {
  components: { Navigation, Gallery },
}
</script>

<style lang="scss">
@import '@/assets/styles/base.scss';
</style>
