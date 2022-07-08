<template>
  <div>
      <hooper :infiniteScroll="true" :settings="hooperSettings" style="height: 100%">
        <slide >
          <div class="relative">
            <img  src="../assets/bg.jpg" alt="">
            <div class=" absolute bottom-40 left-40">
              <p class="bg-black opacity-70 text-white text-3xl font-bold max-w-2xl uppercase p-3">this is a place where technology & creativity fused into digital chemistry</p>
            </div>
          </div>
        </slide>
        <slide >
          <div class="relative">
            <img  src="../assets/about-bg.jpg" alt="">
            <div class=" absolute bottom-40 left-40">
              <p class="bg-black opacity-70 text-white text-3xl font-bold max-w-2xl uppercase p-3">we dont have the best but we have greatest team</p>
            </div>
          </div>
        </slide>
        <hooper-navigation slot="hooper-addons"></hooper-navigation>
        <hooper-pagination slot="hooper-addons"></hooper-pagination>
    </hooper>
  </div>
</template>

<script>
import { Hooper, Slide, Navigation as HooperNavigation, Pagination as HooperPagination, } from 'hooper';
import 'hooper/dist/hooper.css';

export default {
  name: 'App',
    data() {
    return {
      hooperSettings: {
        itemsToShow: 1,
        centerMode: true
      }
    };
  },
  components: {
    Hooper,
    Slide,
    HooperNavigation,
    HooperPagination,
  }
};
</script>

<style>

</style>