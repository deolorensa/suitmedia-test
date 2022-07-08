<template>
<div>
  <div>
    <navbar-main/>
  </div>
  <div>
    <carousel-main/>
  </div>
  <div class="my-32">
    <div class="pb-10 text-center text-3xl text-black font-bold uppercase ">
      <p>our values</p>
    </div>
    <tabel-main/>
  </div>
  <div class="my-32">
    <div class="pb-10 text-center text-3xl text-black font-bold uppercase ">
      <p>contact us</p>
    </div>
    <form-main/>
  </div>
  <div>
    <footer-main/>
  </div>
</div>
</template>

<script>
import NavbarMain from '../components/NavbarMain.vue'
import CarouselMain from '@/components/CarouselMain.vue'
import FooterMain from '@/components/FooterMain.vue'
import TabelMain from '../components/TabelMain.vue'
import FormMain from '../components/FormMain.vue'
export default {
  components: {
    NavbarMain,
    CarouselMain,
    FooterMain,
    TabelMain,
    FormMain
}
}
</script>

NavbarMain