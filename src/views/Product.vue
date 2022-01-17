<template>
  <Layout>
    <div class="product">
      <Product :paging="true" />
    </div>
  </Layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Product from '@/sections/Product/index.vue';
import Layout from '@/components/Layout/Layout.vue';

export default defineComponent({
  name: 'Product Home',
  components: { Product, Layout },
});
</script>
