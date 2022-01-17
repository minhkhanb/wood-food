<template>
  <div class="home">
    <div class="container mx-auto">
      <div class="category mb-8">
        <h3
          class="flex items-center justify-between font-medium text-xl text-green-700 uppercase mb-4"
        >
          Phôi cao su xẻ

          <router-link class="flex font-semibold items-center text-xs" to="#">
            Xem Thêm
            <ChevronDoubleRightIcon class="h-4" />
          </router-link>
        </h3>
        <Product />
      </div>

      <div class="category mb-8">
        <h3
          class="flex items-center justify-between font-medium text-xl text-green-700 uppercase mb-4"
        >
          Gỗ Cao Su

          <router-link class="flex font-semibold items-center text-xs" to="#">
            Xem Thêm
            <ChevronDoubleRightIcon class="h-4" />
          </router-link>
        </h3>
        <Product />
      </div>

      <div class="category mb-8">
        <h3
          class="flex items-center justify-between font-medium text-xl text-green-700 uppercase mb-4"
        >
          Gỗ ghép, ván ghép

          <router-link class="flex font-semibold items-center text-xs" to="#">
            Xem Thêm
            <ChevronDoubleRightIcon class="h-4" />
          </router-link>
        </h3>
        <Product />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Product from '@/sections/Product/index.vue';
import { ChevronDoubleRightIcon } from '@heroicons/vue/outline';

export default defineComponent({
  name: 'Home',
  components: { Product, ChevronDoubleRightIcon },
});
</script>
