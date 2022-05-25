<script setup>
import Header from "../components/Header.vue";
</script>

<template>
  <main>
    <!-- header -->
    <Header
      title="Vue Travel Tours App"
      subtitle="Lorem ipsum dolor sit amet."
    />
    <!-- header end -->
    <!-- section -->
    <section class="main-section py-5">
      <div class="container">
        <div class="row mb-3">
          <div class="col-md-9 col-7">
            <h2>Tour List</h2>
          </div>
          <div class="col-md-3 col-5">
            <select v-model="categoryFilter" class="form-control">
              <option value="all">all</option>
            </select>
          </div>
        </div>
        <!-- tour-list -->
        <div class="tour-list row">
          <div class="col-lg-4 col-sm-6">
            <div class="tour">
              <div
                class="tour-thumbnail"
                style="
                  background-image: url('https://picsum.photos/id/684/1600/1200');
                "
              ></div>
              <div class="tour-body">
                <h5 class="text-danger">Example</h5>
                <p class="text-muted mb-0">
                  <i class="fas fa-map-marked-alt"></i> Country, City
                </p>
                <div class="category-list">
                  <div class="category-badge bg-primary text-white">
                    <i class="fas fa-tram"></i><span>Cable car</span>
                  </div>
                  <div class="category-badge bg-primary text-white">
                    <i class="fas fa-university"></i><span>Museum</span>
                  </div>
                </div>
                <p class="tour-description">
                  Lorem ipsum, dolor sit amet consectetur adipisicing elit.
                  Fugit doloremque amet quis debitis vel animi voluptates
                  repudiandae. Exercitationem quia et praesentium! Repudiandae
                  ipsa aliquid, maiores debitis amet hic perspiciatis unde
                  quidem molestias eius quam pariatur. Dignissimos sint
                  doloremque autem reprehenderit magnam rerum repellendus cum
                  quibusdam consectetur eaque voluptates suscipit eius ducimus,
                  vero tempore eveniet, illo quos, porro minima dolor odit
                  perferendis impedit. Delectus quae tempora sequi assumenda
                  expedita officia quasi repellat culpa impedit natus quas
                  molestiae sint rem, perferendis distinctio enim quis fuga eos
                  animi vel necessitatibus? Quidem veritatis, perferendis cum
                  tempora obcaecati blanditiis eius in quo ad aliquid optio.
                </p>
                <p class="text-right posted-at">Posted at 2021/01/05</p>
              </div>
            </div>
          </div>
        </div>
        <!-- tour-list -->
      </div>
    </section>
    <!-- section end -->
    <!-- footer -->
    <footer class="bg-light py-2">
      <p class="m-0 text-center">Travel Tours App</p>
    </footer>
    <!-- footer end -->
  </main>
</template>

<script>
export default {
  name: "HomeView",
  data() {
    return {
      categoryFilter: "all",
    };
  },
  mounted() {
    // 試著在元件掛載後使用 axios 串接來自 JSONbin 上的資料
    // https://jsonbin.io
    // 相關資源可參照 src/config/apiConfig
    // headers: { "X-ACCESS-KEY": X-ACCESS-KEY }
  },
};
</script>

