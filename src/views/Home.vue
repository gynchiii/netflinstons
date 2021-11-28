<template>
<div class="mt-5 mb-4">
  <b-embed
    type="iframe"
    class="mt-4"
    allow="autoplay"
    aspect="16by9"
    src="https://www.youtube.com/embed/ae6w0-kZ3-M"
    allowfullscreen
  ></b-embed>
    <h1 style="color: white;" class="mt-4">Kids</h1>
  <MoviesCarousel class="mt-3" :movies="kids"/>
    <h1 style="color: white;" class="">Action</h1>
  <MoviesCarousel class="mt-3" :movies="action"/>
    <h1 style="color: white;" class="">Comedy</h1>
  <MoviesCarousel class="mt-3" :movies="comedy"/>
    <h1 style="color: white;" class="">Horror & Sus</h1>
  <MoviesCarousel class="mt-3" :movies="horror"/>
    <h1 style="color: white;" class="">Sports Based</h1>
  <MoviesCarousel class="mt-3" :movies="sports"/>
</div>
</template>

<script>
// @ is an alias to /src

import MoviesCarousel from '../components/MoviesCarousel'

export default {
  data () {
    return {
      kids: [
        { id: 1, title: 'Rick and Morty', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' },
        { id: 2, title: 'Cars', banner: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTqNjqaJdaz96XxluDcwsy4MjHvQT_OdxleI5ysZlpuGFPnWht95DzdhEzq73u_RgqGuQU&usqp=CAU' },
        { id: 3, title: 'Cars 2', banner: 'https://upload.wikimedia.org/wikipedia/pt/7/7e/Carros_2_P%C3%B4ster.jpg' },
        { id: 4, title: 'Toy Story', banner: 'http://assets.nflxext.com/us/boxshots/hd1080/60036637.jpg' },
        { id: 5, title: 'Toy Story 2', banner: 'https://scdn.nflximg.net/ipl/74041/706a4363ddef3f317e40c6303a375388a06b03d7.jpg' },
        { id: 6, title: 'Toy Story 3', banner: 'https://scdn.nflximg.net/ipl/43637/9a58748d488c020f2b619417bf7a4e811918d6dc.jpg' },
        { id: 7, title: 'Shrek', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' },
        { id: 8, title: 'Shrek 2', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' },
        { id: 9, title: 'Shrek 3', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' },
        { id: 10, title: 'Shrek 4', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' },
        { id: 11, title: 'Castlevania', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' },
        { id: 12, title: 'The Simpsons', banner: 'https://http2.mlstatic.com/D_NQ_NP_726734-MLB42542288039_072020-O.jpg' }
      ],
      action: [
        { id: 13, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 14, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 15, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 16, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 17, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 18, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' }
      ],
      comedy: [
        { id: 19, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 20, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 21, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 22, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 23, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 24, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' }
      ],
      horror: [
        { id: 25, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 26, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 27, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 28, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 29, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 30, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' }
      ],
      sports: [
        { id: 31, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 32, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 33, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 34, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 35, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' },
        { id: 36, banner: 'http://assets.nflxext.com/us/boxshots/hd1080/81058097.jpg' }
      ]
    }
  },
  components: {
    MoviesCarousel
  }
}
</script>
