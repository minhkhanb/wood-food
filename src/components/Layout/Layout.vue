﻿<template>
  <div
    class="layout container max-w-full mx-auto"
    :class="{ 'sidebar-open': openSidebar }"
  >
    <header class="pt-6 overflow-hidden px-4">
      <div class="container mx-auto">
        <div
          class="flex flex-col lg:flex-row sm:text-left flex-auto justify-between items-center mb-6"
        >
          <div class="logo flex-stretch mb-4">
            <h1>
              <router-link to="/">
                <figure
                  class="w-24 h-24 overflow-hidden bg-white rounded-xl mr-0 sm:mr-6"
                >
                  <img
                    class="w-full h-full object-contain"
                    :src="require('@/assets/images/logo.jpg')"
                    alt="CÔNG TY TNHH GỖ BẾN CÁT"
                  />
                </figure>
              </router-link>
            </h1>
          </div>

          <div
            class="flex flex-auto w-full px-4 py-2 search border border-gray-700 rounded-3xl overflow-hidden mb-4"
          >
            <input
              type="text"
              placeholder="Tìm kiếm sản phẩm..."
              class="border-0 focus:outline-none bg-transparent w-full"
            />
            <button class="w-6 ml-2">
              <SearchIcon />
            </button>
          </div>

          <div
            class="top-bar flex flex-col sm:flex-row items-center flex-auto ml-0 sm:ml-8"
          >
            <div class="contact flex flex-col sm:flex-row items-center mb-4">
              <PhoneIcon class="text-yellow-500 w-12" />
              <p
                class="text-yellow-500 sm:ml-2 font-bold w-32 text-center sm:text-left"
              >
                Tư vấn hỗ trợ <br />0986 625 525
              </p>
            </div>

            <div class="work-open flex flex-col sm:flex-row items-center mb-4">
              <ClockIcon class="text-green-500 w-12" />
              <p
                class="text-green-500 ml-2 font-bold w-56 text-center sm:text-left"
              >
                Thời gian làm việc <br />
                <span class="font-medium">Thứ 2 - Thứ 7 | 8:00 - 17:00</span>
              </p>
            </div>

            <div class="shipping flex flex-col sm:flex-row items-center mb-4">
              <TruckIcon class="text-green-500 w-12" />
              <p
                class="text-green-500 ml-2 font-bold w-56 text-center sm:text-left"
              >
                Miễn phí vận chuyển <br />
                <span class="font-medium">Đơn hàng > 1.000.000 VNĐ</span>
              </p>
            </div>
          </div>
        </div>
      </div>
    </header>
    <aside>
      <div class="nav-menu hidden md:block my-0 px-4">
        <div class="container mx-auto">
          <nav class="flex px-0 py-5">
            <ul class="flex">
              <li class="">
                <router-link
                  class="w-16 px-2 py-4 border block overflow-hidden"
                  to="/"
                >
                  <HomeIcon class="w-6 mx-auto" />
                </router-link>
              </li>

              <li class="">
                <router-link
                  class="block text-black font-medium px-8 py-4 text-base hover:bg-white hover:text-gray-500 border uppercase"
                  to=""
                  >giới thiệu</router-link
                >
              </li>

              <li class="menu-item relative">
                <router-link
                  class="block text-black font-medium px-8 py-4 text-base hover:bg-white hover:text-gray-500 border uppercase"
                  to=""
                >
                  sản phẩm
                </router-link>

                <ul class="sub-menu">
                  <li class="">
                    <router-link
                      class="block text-black font-medium px-8 py-4 hover:bg-white text-base hover:text-gray-500 border uppercase"
                      to="/product"
                      >Phôi Cao Su Xẻ Sấy</router-link
                    >
                  </li>

                  <li class="">
                    <router-link
                      class="block text-black font-medium px-8 py-4 hover:bg-white text-base hover:text-gray-500 border uppercase"
                      to="/product"
                      >Gỗ Ghép, Ván Ghép</router-link
                    >
                  </li>

                  <li class="">
                    <router-link
                      class="block text-black font-medium px-8 py-4 hover:bg-white text-base hover:text-gray-500 border uppercase"
                      to="/product"
                      >Gỗ Cao Su</router-link
                    >
                  </li>
                </ul>
              </li>

              <li class="">
                <router-link
                  class="block text-black font-medium px-8 py-4 text-base hover:bg-white hover:text-gray-500 border uppercase"
                  to=""
                  >dịch vụ</router-link
                >
              </li>

              <li class="">
                <router-link
                  class="block text-black font-medium px-8 py-4 text-base hover:bg-white hover:text-gray-500 border uppercase"
                  to=""
                  >liên hệ</router-link
                >
              </li>
            </ul>
          </nav>
        </div>
      </div>

      <div class="side-left">
        <div class="">
          <SlickCarousel />
        </div>
      </div>
    </aside>
    <main class="main-content px-4">
      <div class="breacrum container mx-auto">
        <nav class="flex px-0 py-5">
          <ul class="flex">
            <li class="">
              <router-link class="px-2 py-4 block hover:text-gray-500" to="/">
                Home
              </router-link>
            </li>

            <li class="">
              <span class="px-2 py-4 block" to=""> / </span>
            </li>

            <li class="">
              <router-link
                class="px-2 py-4 block hover:text-gray-500"
                to="/product"
              >
                Product
              </router-link>
            </li>
          </ul>
        </nav>
      </div>
      <div class="max-w-screen-xl mx-auto">
        <slot />
      </div>
    </main>
    <footer class="pt-6 border-t bg-gray-900">
      <div class="container mx-auto px-8">
        <aside class="flex flex-col sm:flex-row mb-8">
          <div class="block w-full sm:w-9/12 sm:flex text-center sm:text-left">
            <div class="w-full sm:w-1/4 px-2 mb-6">
              <h5 class="mb-3 text-white uppercase text-lg font-medium">
                THÔNG TIN LIÊN HỆ
              </h5>
              <div class="info text-gray-300 leading-8">
                CÔNG TY TNHH GỖ BẾN CÁT<br />
                164 QL 22B, Ấp Thanh Phước, Xã Thanh Điền, Huyện Châu Thành, Tây
                Ninh
                <br />
                Hotline:<a href="tel:0901027070">0901 027 070</a>,
                <a href="tel:0986625525">0986 625 525</a><br />
                Email:
                <a href="mailto:gobencat@gmail.com">gobencat@gmail.com</a>
              </div>
            </div>

            <div class="w-full sm:w-1/4 px-2 mb-6">
              <h5 class="mb-3 text-white uppercase text-lg font-medium">
                GIỚI THIỆU
              </h5>
              <div class="info text-gray-300">
                <ul>
                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Giới thiệu về chúng tôi</router-link
                    >
                  </li>

                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Tuyển dụng</router-link
                    >
                  </li>

                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Ưu đãi - khuyến mại</router-link
                    >
                  </li>
                </ul>
              </div>
            </div>

            <div class="w-full sm:w-1/4 px-2 mb-6">
              <h5 class="mb-3 text-white uppercase text-lg font-medium">
                Chính sách & quy định
              </h5>
              <div class="info text-gray-300">
                <ul>
                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Chính sách vận chuyển</router-link
                    >
                  </li>
                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Quy định thanh toán</router-link
                    >
                  </li>
                </ul>
              </div>
            </div>

            <div class="w-full sm:w-1/4 px-2 mb-6">
              <h5 class="mb-3 text-white uppercase text-lg font-medium">
                Hướng dẫn sử dụng
              </h5>
              <div class="info text-gray-300">
                <ul>
                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Hướng dẫn mua hàng</router-link
                    >
                  </li>
                </ul>
              </div>
            </div>
          </div>

          <div class="social-box w-full sm:w-3/12 mx-auto sm:ml-0">
            <div class="mb-2">
              <div class="social">
                <div
                  class="fb-page"
                  data-href="https://www.facebook.com/facebook"
                  data-tabs="events"
                  data-width="320"
                  data-height=""
                  data-small-header="false"
                  data-adapt-container-width="true"
                  data-hide-cover="false"
                  data-show-facepile="true"
                >
                  <blockquote
                    cite="https://www.facebook.com/facebook"
                    class="fb-xfbml-parse-ignore"
                  >
                    <a href="https://www.facebook.com/facebook">Meta</a>
                  </blockquote>
                </div>
              </div>
              <div class="map">
                <GoogleMap
                  api-key="AIzaSyBbPdgwcEOZZLYhU3yR-9ozwntTDili30w"
                  :center="center"
                  :zoom="15"
                  style="width: 100%; max-width: 320px; height: 180px"
                >
                  <Marker :options="{ position: center }" />
                </GoogleMap>
              </div>
            </div>
          </div>
        </aside>
      </div>
      <div class="copyright border-t border-gray-600 p-4">
        <div class="container mx-auto">
          <div class="block sm:flex text-center text-gray-300 justify-between">
            <div class="col-left flex items-center mb-2">
              <p>Copyright © 2022 CÔNG TY TNHH GỖ BẾN CÁT.</p>
            </div>
            <div class="col-right mb-2">
              <div class="flex justify-center">
                <router-link class="px-1" to="#">
                  <img
                    :src="require('@/assets/images/icon-facebook.png')"
                    alt=""
                  />
                </router-link>

                <router-link class="px-1" to="#">
                  <img
                    :src="require('@/assets/images/icon-youtube.png')"
                    alt=""
                  />
                </router-link>

                <router-link class="px-1" to="#">
                  <img :src="require('@/assets/images/icon-lin.png')" alt="" />
                </router-link>

                <router-link class="px-1" to="#">
                  <img
                    :src="require('@/assets/images/icon-pinset.png')"
                    alt=""
                  />
                </router-link>
              </div>
            </div>
          </div>
        </div>
      </div>
    </footer>

    <!-- <router-link to="#" class="scrollToTop">Scroll To Top</router-link> -->
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { GoogleMap, Marker } from 'vue3-google-map';
import {
  TruckIcon,
  PhoneIcon,
  SearchIcon,
  ClockIcon,
  HomeIcon,
} from '@heroicons/vue/outline';
import SlickCarousel from '@/components/SlickCarousel.vue';

export default defineComponent({
  components: {
    TruckIcon,
    PhoneIcon,
    SearchIcon,
    ClockIcon,
    SlickCarousel,
    HomeIcon,
    GoogleMap,
    Marker,
  },
  data() {
    return {
      openSidebar: false,
      img: require('@/assets/images/avatar.jpg'),
    };
  },
  setup() {
    const center = { lat: 11.0950583, lng: 106.2611953 };

    return { center };
  },
  created() {
    console.log(this.img);
  },
});
</script>

<style scoped></style>
