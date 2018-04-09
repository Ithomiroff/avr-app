<template>
  <section class="slider-wrap">
    <div class="slider__head">
      <div class="title">Наши партнеры</div>
    </div>
    <carousel
      :autoplay="true"
      :autoplayHoverPause="true"
      :paginationEnabled="false"
      :navigationEnabled="true"
      :easing="'ease-in'"
      :perPageCustom="[[4608, 2],[768, 3], [1024, 4]]"
    >
      <slide v-for="(partner, index) in this.partners" :key="index">
        <img v-bind:src="partner.img" alt="">
      </slide>
    </carousel>
  </section>
</template>

<script>
    import { Carousel, Slide } from 'vue-carousel';
    export default {
        name: "slider-partners",
        component: {
          Carousel,
          Slide
        },
        data() {
            return {
                partners: [
                {
                    img:'/images/partners/1 (1).png',
                    link: 'google.com'
                },
                {
                    img:'/images/partners/1 (9).png',
                    link: 'google.com'
                },
                {
                  img:'/images/partners/1 (9).png',
                  link: 'google.com'
                },
                {
                  img:'/images/partners/1 (9).png',
                  link: 'google.com'
                },
                {
                  img:'/images/partners/1 (9).png',
                  link: 'google.com'
                },
                {
                  img:'/images/partners/1 (9).png',
                  link: 'google.com'
                },
          ]
        }
      }
    }
</script>

<style lang="scss">
  .slider-wrap {
    img {
      max-width: 100px;
      width: 100%;
    }
  }
</style>
