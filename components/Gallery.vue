<template>
  <div class="gallery--container">
    <div class="masonry">
      <nuxt-img
        v-for="(image, imageIndex) in images"
        :key="`image-${imageIndex}`"
        class="brick"
        format="webp"
        :src="image"
      />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        'images/starry-night/thumbnail.jpg',
        'images/the-storm-on-the-sea-of-galilee/thumbnail.jpg',
        'images/lady-with-an-ermine/thumbnail.jpg',
        'images/the-boy-in-the-red-vest/thumbnail.jpg',
        'images/girl-with-pearl-earring/thumbnail.jpg',
        'images/the-great-wave-off-kanagawa/thumbnail.jpg',
        'images/the-night-cafe/thumbnail.jpg',
        'images/arnolfini-portrait/thumbnail.jpg',
        'images/guernica/thumbnail.jpg',
        'images/van-gogh-self-portrait/thumbnail.jpg',
        'images/mona-lisa/thumbnail.jpg',
        'images/penitent-magdalene/thumbnail.jpg',
        'images/the-sleeping-gypsy/thumbnail.jpg',
        'images/the-basket-of-apples/thumbnail.jpg',
        'images/the-swing/thumbnail.jpg',
      ],
    }
  },
}
</script>

//
<style lang="scss" scoped>
@import '@/assets/styles/gallery.scss';
</style>
