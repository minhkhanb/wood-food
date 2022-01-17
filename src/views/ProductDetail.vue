<template>
  <Layout>
    <div class="product-detail">
      <div class="container mx-auto">
        <div class="product flex flex-col sm:flex-row mb-8">
          <div
            class="thumbnail product-detail w-full sm:w-1/2 h-96 sm:h-product mb-2 relative overflow-hidden"
          >
            <div
              class="img absolute top-0 left-0 right-0 bottom-0 transition-all transform"
            >
              <div>
                <img
                  class="object-cover w-full h-full mx-auto"
                  :src="product.thumbnail"
                  alt=""
                />
              </div>
            </div>
          </div>

          <div class="info px-4 py-3 w-full sm:w-1/2">
            <h3
              class="font-semibold text-gray-700 text-xl uppercase leading-snug text-normal mb-2"
            >
              <router-link to="/product/1">{{ product.title }}</router-link>
            </h3>
            <div class="mt-2 text-sm text-gray-600 mb-2">Giá: Liên hệ</div>
            <div class="mb-2">
              <span>Xuất Xứ: Gỗ Bến Cát</span>
            </div>

            <div>
              <p>Thông Tin Sản Phẩm:<br /></p>
              <ul>
                <li>
                  - Lorem Ipsum is simply dummy text of the printing and
                  typesetting industry
                </li>
                <li>
                  - It is a long established fact that a reader will be
                  distracted by the readable content of a page when looking at
                  its layout.
                </li>
                <li>
                  - There are many variations of passages of Lorem Ipsum
                  available, but the majority have suffered alteration
                </li>
                <li>
                  - Contrary to popular belief, Lorem Ipsum is not simply random
                  text
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="product-relation">
          <h3
            class="flex items-center justify-between font-medium text-xl text-green-700 uppercase mb-4"
          >
            Sản phẩm liên quan
          </h3>
          <Product />
        </div>
      </div>
    </div>
  </Layout>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import Product from '@/sections/Product/index.vue';
import Layout from '@/components/Layout/Layout.vue';

export default defineComponent({
  name: 'Product Detail Home',
  components: { Product, Layout },
  data() {
    return {
      product: {
        id: 1,
        title: 'Phôi cao su sẻ sấy 1',
        thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
      },
    };
  },
});
</script>
