<template>
  <div class="products max-w-screen-2xl mx-auto">
    <ul :class="`grid grid-cols-${numOfColumn} gap-4 mb-4`">
      <li :key="index" v-for="(product, index) in pageOfItems">
        <div class="bg-white shadow">
          <div class="thumbnail h-56 mb-2 relative overflow-hidden">
            <div
              class="thumbnail-overlay transition-all flex items-center justify-center bg-black bg-opacity-70 absolute top-0 left-0 right-0 bottom-0 z-20 opacity-0"
            >
              <router-link
                class="p-2 pl-5 pr-5 bg-transparent transition-all border border-yellow-500 text-yellow-500 text-lg hover:bg-yellow-500 hover:text-gray-100 focus:border focus:border-yellow-300"
                to="/product/1"
              >
                Xem Nhanh
              </router-link>
            </div>
            <div class="hot-label electric text-white text-xs font-medium">
              <span>Hot New</span>
            </div>
            <div
              class="img absolute top-0 left-0 right-0 bottom-0 transition-all transform hover:scale-105"
            >
              <router-link to="/product/1">
                <img
                  class="object-cover w-full h-full mx-auto"
                  :src="product.thumbnail"
                  alt=""
                />
              </router-link>
            </div>
          </div>
          <div class="info px-4 py-3">
            <h3
              class="font-semibold text-gray-700 leading-snug text-normal mb-2"
            >
              <router-link to="/product/1">{{ product.title }}</router-link>
            </h3>
            <div class="mt-2 text-sm text-gray-600 mb-2">Giá: Liên hệ</div>
            <div>
              <span>Xuất xứ: Gỗ Bến Cát</span>
            </div>
          </div>
        </div>
      </li>
    </ul>
    <div v-if="$props.paging" class="pagination pb-4 pt-4">
      <ul
        v-if="pager.pages && pager.pages.length"
        class="flex justify-center pl-0 list-none rounded my-2"
      >
        <li
          :class="{ disabled: pager.currentPage === 1 }"
          class="page-item first-item relative block leading-tight mr-px bg-white text-black hover:bg-gray-200"
        >
          <router-link
            :to="{ query: { page: 1 } }"
            class="block page-link py-4 px-6"
            >First</router-link
          >
        </li>
        <li
          :class="{ disabled: pager.currentPage === 1 }"
          class="relative block leading-tight bg-white text-black mr-px hover:bg-gray-200"
        >
          <router-link
            :to="{ query: { page: pager.currentPage - 1 } }"
            class="block page-link py-4 px-6"
            >Previous</router-link
          >
        </li>
        <li
          v-for="page in pager.pages"
          :key="page"
          :class="{ active: pager.currentPage === page }"
          class="relative block leading-tight bg-white mr-px text-black hover:bg-gray-200"
        >
          <router-link
            :to="{ query: { page: page } }"
            class="block page-link py-4 px-6"
          >
            {{ page }}
          </router-link>
        </li>
        <li
          :class="{ disabled: pager.currentPage === pager.totalPages }"
          class="relative block leading-tight bg-white mr-px text-black hover:bg-gray-200"
        >
          <router-link
            :to="{ query: { page: pager.currentPage + 1 } }"
            class="block page-link py-4 px-6"
            >Next</router-link
          >
        </li>
        <li
          :class="{ disabled: pager.currentPage === pager.totalPages }"
          class="relative block leading-tight bg-white mr-px text-black hover:bg-gray-200"
        >
          <router-link
            :to="{ query: { page: pager.totalPages } }"
            class="block page-link py-4 px-6"
            >Last</router-link
          >
        </li>
      </ul>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import paginate from 'jw-paginate';

interface Page {
  id: number;
  title: string;
  thumbnail: string;
}

interface Pager {
  totalItems: number;
  currentPage: number;
  pageSize: number;
  totalPages: number;
  startPage: number;
  endPage: number;
  startIndex: number;
  endIndex: number;
  pages: number[];
}

export default defineComponent({
  name: 'Product',
  props: {
    paging: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {
      numOfColumn: 5,
      pager: {} as Pager,
      pageOfItems: [] as Page[],
    };
  },
  methods: {
    onPageChanged() {
      console.log('onPageChanged');
    },
    getProducts(curPage: number) {
      const numOfProducts = !this.$props.paging ? 10 : 160;
      console.log(numOfProducts);
      const items = [...Array(numOfProducts).keys()].map((i) => ({
        id: i + 1,
        title: 'Phôi cao su sẻ sấy ' + (i + 1),
        thumbnail: 'http://gobencat.bizz.vn/img_products/4650/b1.jpg',
      }));

      // get page from query params or default to first page
      const page = curPage || 1;

      // get pager object for specified page
      const pageSize = 12;
      const pager = paginate(items.length, page, pageSize);

      // get page of items from items array
      const pageOfItems = items.slice(pager.startIndex, pager.endIndex + 1);

      // return pager object and current page of items
      return { pager, pageOfItems };
    },
  },
  watch: {
    '$route.query.page': {
      immediate: true,
      handler(page: number) {
        page = page || 1;
        console.log('watch page: ', page, this.pager.currentPage);
        if (page !== this.pager.currentPage) {
          const { pager, pageOfItems } = this.getProducts(page);
          console.log('pager: ', pageOfItems);
          this.pager = pager;
          this.pageOfItems = pageOfItems;
        }
      },
    },
  },
});
</script>
