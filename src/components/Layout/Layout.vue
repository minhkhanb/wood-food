<template>
  <div
    class="layout container max-w-full mx-auto border"
    :class="{ 'sidebar-open': openSidebar }"
  >
    <header class="pt-6 border-b">
      <div class="container mx-auto">
        <div class="flex justify-between items-center mb-6">
          <div class="logo">
            <h1>
              <router-link to="#">
                <img
                  :src="require('@/assets/images/logo.jpg')"
                  alt="CÔNG TY TNHH GỖ BẾN CÁT"
                />
              </router-link>
            </h1>
          </div>
        </div>
      </div>
    </header>
    <aside>
      <div class="side-left"></div>
      <div class="nav-menu">
        <nav>
          <ul>
            <li>
              <router-link to="">trang chủ</router-link>
            </li>

            <li>
              <router-link to="">giới thiệu</router-link>
            </li>

            <li>
              <router-link to="">sản phẩm</router-link>
            </li>

            <li>
              <router-link to="">liên hệ</router-link>
            </li>
          </ul>
        </nav>
      </div>
    </aside>
    <main class="main-content">
      <div class="border border-pink-600">
        <div class="products">
          <ul>
            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b1.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b2.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b3.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b3.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b5.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b6.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b7.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b8.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b9.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b10.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>

            <li>
              <div>
                <div class="thumbnail">
                  <router-link to="#">
                    <img
                      src="http://gobencat.bizz.vn/img_products/4650/b11.jpg"
                      alt=""
                    />
                  </router-link>
                </div>
                <div class="info">
                  <h3></h3>
                </div>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </main>
    <footer class="pt-6 border-t">
      <div class="container mx-auto">
        <aside>
          <div>
            <div>
              <h5>THÔNG TIN LIÊN HỆ</h5>
              <div class="info">
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

            <div>
              <h5>GIỚI THIỆU</h5>
              <div class="info">
                <ul>
                  <li>
                    <router-link to="#">Giới thiệu về chúng tôi</router-link>
                  </li>

                  <li>
                    <router-link to="#">Tuyển dụng</router-link>
                  </li>

                  <li>
                    <router-link to="#">Ưu đãi - khuyến mại</router-link>
                  </li>
                </ul>
              </div>
            </div>

            <div>
              <h5>Chính sách & quy định</h5>
              <div class="info">
                <ul>
                  <li>
                    <router-link to="#">Chính sách bảo mật</router-link>
                  </li>

                  <li>
                    <router-link to="#">Chính sách vận chuyển</router-link>
                  </li>

                  <li>
                    <router-link to="#">Quy định thanh toán</router-link>
                  </li>
                </ul>
              </div>
            </div>

            <div>
              <h5>Hướng dẫn sử dụng</h5>
              <div class="info">
                <ul>
                  <li>
                    <router-link to="#">Hướng dẫn sử dụng</router-link>
                  </li>
                </ul>
              </div>
            </div>
          </div>
        </aside>
      </div>
      <div class="copyright">
        <div class="container mx-auto">
          <div class="col-left">
            <p>Copyright © 2022 CÔNG TY TNHH GỖ BẾN CÁT.</p>
          </div>
          <div class="col-right">
            <div>
              <router-link to="#">
                <img
                  :src="require('@/assets/images/icon-facebook.png')"
                  alt=""
                />
              </router-link>

              <router-link to="#">
                <img
                  :src="require('@/assets/images/icon-youtube.png')"
                  alt=""
                />
              </router-link>

              <router-link to="#">
                <img :src="require('@/assets/images/icon-lin.png')" alt="" />
              </router-link>

              <router-link to="#">
                <img :src="require('@/assets/images/icon-pinset.png')" alt="" />
              </router-link>
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
