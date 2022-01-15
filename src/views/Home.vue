<template>
  <div class="home">
    <Product />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Product from '@/sections/Product/index.vue';

export default defineComponent({
  name: 'Home',
  components: { Product },
});
</script>
