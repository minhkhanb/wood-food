<template>
  <swiper
    :slides-per-view="1"
    :space-between="50"
    :centeredSlides="true"
    :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
  >
    <swiper-slide>
      <img
        class="w-full max-h-banner object-cover"
        src="http://gobencat.bizz.vn/img_slide/4650/sl1.jpg"
      />
    </swiper-slide>
    <swiper-slide>
      <img
        class="w-full max-h-banner object-cover"
        src="http://gobencat.bizz.vn/img_slide/4650/sl.jpg"
      />
    </swiper-slide>
  </swiper>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/swiper.scss';
import { SwiperEvents } from 'swiper/types';
import SwiperCore, { Autoplay } from 'swiper';

SwiperCore.use([Autoplay]);

export default defineComponent({
  name: 'SlickCarousel',
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const onSwiper = (swiper: SwiperEvents) => {
      console.log('swiper: ', swiper);
    };
    const onSlideChange = () => {
      console.log('slide change');
    };
    return {
      onSwiper,
      onSlideChange,
    };
  },
});
</script>
