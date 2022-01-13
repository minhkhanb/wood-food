<template>
  <div
    class="layout container max-w-full mx-auto"
    :class="{ 'sidebar-open': openSidebar }"
  >
    <header class="pt-6 border-b">
      <div class="container mx-auto">
        <div class="flex justify-between items-center mb-6">
          <div class="logo">
            <h1>
              <router-link to="#">
                <figure class="bg-gray-100 rounded-xl p-8 dark:bg-gray-800">
                  <img
                    class="w-24 h-24 rounded-full mx-auto"
                    :src="require('@/assets/images/logo.jpg')"
                    alt="CÔNG TY TNHH GỖ BẾN CÁT"
                  />
                </figure>
              </router-link>
            </h1>
          </div>
        </div>
      </div>
    </header>
    <aside>
      <div class="side-left"></div>
      <div class="nav-menu">
        <nav class="flex p-8">
          <ul class="flex">
            <li class="">
              <router-link
                class="
                  font-medium
                  px-3
                  py-2
                  text-gray-700
                  rounded-lg
                  hover:bg-gray-100 hover:text-gray-900
                  uppercase
                "
                to=""
                >trang chủ</router-link
              >
            </li>

            <li class="">
              <router-link
                class="
                  font-medium
                  px-3
                  py-2
                  text-gray-700
                  rounded-lg
                  hover:bg-gray-100 hover:text-gray-900
                  uppercase
                "
                to=""
                >giới thiệu</router-link
              >
            </li>

            <li class="">
              <router-link
                class="
                  font-medium
                  px-3
                  py-2
                  text-gray-700
                  rounded-lg
                  hover:bg-gray-100 hover:text-gray-900
                  uppercase
                "
                to=""
                >sản phẩm</router-link
              >
            </li>

            <li class="">
              <router-link
                class="
                  font-medium
                  px-3
                  py-2
                  text-gray-700
                  rounded-lg
                  hover:bg-gray-100 hover:text-gray-900
                  uppercase
                "
                to=""
                >liên hệ</router-link
              >
            </li>
          </ul>
        </nav>
      </div>
    </aside>
    <main class="main-content">
      <div>
        <div class="products max-w-screen-2xl mx-auto">
          <ul class="grid grid-cols-5 gap-4 mb-4">
            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <router-link to="#">
                    <img
                      class="rounded object-cover w-full h-full mx-auto"
                      src="http://gobencat.bizz.vn/img_products/4650/b1.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <router-link to="#">
                    <img
                      class="rounded object-cover h-full mx-auto"
                      src="http://gobencat.bizz.vn/img_products/4650/b2.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b3.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b3.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b5.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b6.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b7.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b8.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b9.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b10.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>

            <li>
              <div class="px-4 sm:px-6 py-2 sm:py-4 mx-auto bg-white shadow">
                <div class="thumbnail h-80 mb-2">
                  <img
                    class="rounded object-cover h-full mx-auto"
                    src="http://gobencat.bizz.vn/img_products/4650/b11.jpg"
                    alt=""
                  />
                </div>
                <div class="info">
                  <h3 class="font-bold text-gray-700 leading-snug">
                    <router-link to="#">Phôi cao su sẻ sấy</router-link>
                  </h3>
                  <div class="mt-2 text-sm text-gray-600">Liên hệ</div>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </main>
    <footer class="pt-6 border-t bg-gray-900">
      <div class="container mx-auto">
        <aside class="mb-8">
          <div class="flex">
            <div class="w-1/4 px-2">
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

            <div class="w-1/4 px-2">
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

            <div class="w-1/4 px-2">
              <h5 class="mb-3 text-white uppercase text-lg font-medium">
                Chính sách & quy định
              </h5>
              <div class="info text-gray-300">
                <ul>
                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Chính sách bảo mật</router-link
                    >
                  </li>

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

            <div class="w-1/4 px-2">
              <h5 class="mb-3 text-white uppercase text-lg font-medium">
                Hướng dẫn sử dụng
              </h5>
              <div class="info text-gray-300">
                <ul>
                  <li class="mb-2">
                    <router-link class="hover:text-white" to="#"
                      >Hướng dẫn sử dụng</router-link
                    >
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </aside>
      </div>
      <div class="copyright border-t border-gray-600 p-4">
        <div class="container mx-auto">
          <div class="flex text-gray-300 justify-between">
            <div class="col-left flex items-center">
              <p>Copyright © 2022 CÔNG TY TNHH GỖ BẾN CÁT.</p>
            </div>
            <div class="col-right">
              <div class="flex">
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

    <router-link to="#" class="scrollToTop">Scroll To Top</router-link>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  data() {
    return {
      openSidebar: false,
      img: require('@/assets/images/avatar.jpg'),
    };
  },
  created() {
    console.log(this.img);
  },
});
</script>

<style scoped></style>
