<template>
  <div>
      <Carousel
        autoplayHoverPause
        speed="800"
        spacePadding="2"
        paginationSize="0"
        autoplay
        :per-page="6"
      >

        <slide v-for="movie in movies" :key="movie.id">
          <b-card
            :img-src="movie.banner"
            img-top
            tag="article"
            style="max-width: 15rem; max-height: 21rem;"
            class="mb-1"
          >
        </b-card>
        </slide>
      </Carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel'

export default {
  components: {
    Carousel,
    Slide
  },
  props: {
    movies: {
      type: Array
    }
  }
}
</script>
