<template>
  <div class="container-slider">
    <VueSlickCarousel v-bind="settings">
      <div class="slide-pics">
        <img src="~/assets/images/slide1.jpg" alt="Slide 1" width="100%" height="450">
      </div>
      <div class="slide-pics">
        <img src="~/assets/images/slide2.jpg" alt="Slide 1" width="100%" height="450">
      </div>
      <div class="slide-pics">
        <img src="~/assets/images/banner.jpg" alt="Slide 1" width="100%" height="450">
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
  import VueSlickCarousel from 'vue-slick-carousel'
  import 'vue-slick-carousel/dist/vue-slick-carousel.css'
  import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

  export default {
    name: 'HomeSlider',
    components: { VueSlickCarousel },
    data() {
      return {
        settings: {
          arrows: false,
          dots: true,
          speed: 1000,
          autoplay: true,
          autoplaySpeed: 3000,
          pauseOnDotsHover: true,
          pauseOnFocus: true,
          pauseOnHover: true
        },
      }
    },
  }
</script>

<style lang="scss">
.container-slider {
  padding: 0;
}
.slick-prev { left: -40px; }
.slick-prev:before, .slick-next:before {
  opacity: 1;
  color: black;
  font-size: 2rem;
}
.slick-dots {
  .slick-active {
    button::before {
      opacity: .75;
      font-size: 14px;
    }
  }
}

@media (max-width: 525px) {
  .container-slider {
    padding: 0;
  }
// .slick-prev:before, .slick-next:before {
//   display: none;
// }
  .slide-pics {
    img {
      height: auto;
    }
  }
}
</style>

