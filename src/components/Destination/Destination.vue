<template>
<section class="destination destination__wrapper">
  <div class="container destination__container">
    <div class="destination__content">
      <h3 class="destination__subtitle subtitle">Choice Of</h3>
      <h2 class="destination__title title">Destinations</h2>
      <h4 class="destination__description description">explore the beauty of god's earth in a beautiful forest and have fun</h4>
      <ActionButton class="action-btn--medium">Explore Now</ActionButton>
    </div>
    <div class="destination__slider-wrapper destination-slider">
      <Swiper
          class="destination-slider__wrapper"
          :modules="modules"
          :slides-per-view="3"
          :centeredSlides="true"
          :grabCursor="true"
          :space-between="30"
          :pagination="{
            clickable: true
          }"
          :initial-slide="1"
          :navigation="{
            enabled: true,
          }"
          @slideChange="onSlideChange"
      >
        <SwiperSlide class="destination-slider__slide" v-for="destinationSlide in destinationSlides">
          <DestinationSlide  :image-path="destinationSlide" />
        </SwiperSlide>
      </Swiper>
    </div>
  </div>
</section>
</template>

<script setup lang="ts">
import ActionButton from "@/components/Buttons/ActionButton.vue";
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Navigation, Pagination, Scrollbar, A11y } from 'swiper/modules';
import 'swiper/scss';
import 'swiper/scss/navigation';
import 'swiper/scss/pagination';
import 'swiper/scss/scrollbar';
import DestinationSlide from "@/components/Destination/DestinationSlide.vue";

const destinationSlides = ['../../assets/images/destinations/destination_1.png', '../../assets/images/destinations/destination_2.png', '../../assets/images/destinations/destination_1.png']
const modules = [
  Navigation, Pagination, Scrollbar, A11y
]

function onSlideChange (): void {
  console.log('slide')
}
</script>

<style lang="scss">
@import "@/assets/styles/destination";
</style>
