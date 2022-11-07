<script setup>
import { ref } from "vue";
import { VueperSlides, VueperSlide } from "vueperslides";
import "vueperslides/dist/vueperslides.css";
defineProps({ components: { VueperSlides, VueperSlide }, msg: String });

const count = ref(0);
</script>

<template>
  <div class="content">
    <div class="fitur">
      <div class="fitur-item">
        <img src="/ayam goreng.jpg" alt="" />

        <h4>ayam goreng</h4>
      </div>
      <div class="fitur-item">
        <img src="/ayam bakar.jpeg" alt="" />

        <h4>ayam bakar</h4>
      </div>
      <div class="fitur-item">
        <img src="/ayam geprek.jpg" alt="" />

        <h4>ayam geprek</h4>
      </div>
    </div>
    <div class="footer"></div>
  </div>
</template>

<style>
.navbar {
  background-color: #FCEED5;
  width: 100%;
  padding: 15px;
  display: flex;
  box-shadow: 0 4px 10px rgba(200, 200, 200, 0.4);
}
.logo {
  text-decoration: none;
  display: block;
  font-size: 25px;
  font-weight: 700;
  color: #fff;
  margin-top: auto;
  margin-bottom: auto;
}
.logo img {
  height: 50px;
}
.navigation {
  display: flex;
  margin-left: auto;
}
.nav-item {
  display: block;
  padding: 7px 10px;
  color: #fff;
  text-decoration: none;
  font-weight: 700;
  background-color: #FCEED5;
  border-radius: 10px;
  margin-right: 10px;
  height: fit-content;
}
.greeting {
  background-color: #FCEED5;
  padding: 30px;
  color: #fff;
}
.greeting-content {
  max-width: 500px;
  margin: auto;
}

.banner img {
  width: 100%;
}
.fitur {
  display: flex;
}
.fitur-item {
  margin-left: auto;
  margin-right: auto;
  text-align: center;
}
.fitur-item img {
  width: 200px;
}
.footer {
  height: 50px;
  width: 100%;
  background-color: #FCEED5;
}
</style>
