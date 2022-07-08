<template>
  <div>
      <hooper :settings="hooperSettings" style="height: 100%">
        <slide >
        <img  src="../assets/bg.jpg" alt="">
        </slide>
        <slide>
        <img src="../assets/about-bg.jpg" alt="">
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