<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
    
      <b-carousel-slide
        text="Somente nos cinemas.."
        img-src="../assets/img/spider.jpg"
        img-height="200px"
      ></b-carousel-slide>

     <b-carousel-slide
        text="Somente nos cinemas.."
        img-src="../assets/img/end.jpg"
      ></b-carousel-slide>

       <b-carousel-slide
        text="Somente nos cinemas.."
        img-src="../assets/img/inter.jpg"
      ></b-carousel-slide>
     

    </b-carousel>
  </div>
</template>

<script>
  export default {
   
    methods: {
      onSlideStart(slide) {
        this.sliding = true
      },
      onSlideEnd(slide) {
        this.sliding = false
      }
    }
  }
</script>