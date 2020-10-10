<template>
  <div>
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="4000"
      controls
      indicators
      background="#ababab"
      img-width="1024"
      img-height="280"
      style="text-shadow: 1px 1px 2px #333;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
    
      <b-carousel-slide
        caption="First slide"
        text="Somente nos cinemas.."
        img-src="../assets/img/spider.jpg"
      ></b-carousel-slide>

    
      <b-carousel-slide img-src="../assets/img/end.jpg">
      </b-carousel-slide>

      
      <b-carousel-slide img-src="../assets/img/inter.jpg"></b-carousel-slide>

      <b-carousel-slide>
        <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            width="1024"
            height="280"
            src="../assets/img/end.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

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