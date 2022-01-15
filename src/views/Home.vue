<template>
  <div class="home">
    <div class="products max-w-screen-2xl mx-auto">
      <ul class="grid grid-cols-5 gap-4 mb-4">
        <li :key="index" v-for="(product, index) in products">
          <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
            <div class="thumbnail h-64 mb-2">
              <router-link to="#">
                <img
                  class="rounded object-cover w-full h-full mx-auto"
                  :src="product.thumbnail"
                  alt=""
                />
              </router-link>
            </div>
            <div class="info">
              <h3 class="font-bold text-gray-700 leading-snug text-xl">
                <router-link to="#">{{ product.title }}</router-link>
              </h3>
              <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  data() {
    return {
      products: [
        {
          id: 1,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 2,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 3,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 4,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 5,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 6,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 7,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 8,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 9,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 10,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 11,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 12,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 13,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 14,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 15,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 16,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 17,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 18,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 19,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 20,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 21,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 22,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 23,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 24,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 25,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 26,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 27,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 28,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 29,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 30,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 31,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 32,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 33,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 34,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 35,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 36,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 37,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 38,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 39,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 40,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 41,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 42,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 43,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 44,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 45,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 46,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 47,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 48,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 49,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 50,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 51,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 52,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 53,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 54,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 55,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 56,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 57,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 58,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 59,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
        {
          id: 60,
          thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
          title: 'Phôi cao su sẻ sấy',
        },
      ],
    };
  },
});
</script>
