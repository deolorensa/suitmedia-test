<template>
  <div>
    <div class=" w-full p-2">
      <div class="container w-full- mx-auto px-32">
        <div class="flex flex-row items-center justify-between">
          <div>
            <a class="text-xl font-black " href="#">Company</a>
          </div>
          <div>
            <button ref="btnRef" v-on:mouseenter="toggleTooltip()" class="text-sm p-3 font-semibold text-gray-500 uppercase hover:bg-gray-200 " >about</button>
            <div ref="tooltipRef" v-bind:class="{'hidden': !tooltipShow, 'block': tooltipShow}" class="z-10 bg-white divide-y divide-gray-100 ">
              <ul class=" text-sm text-gray-700 dark:text-gray-200">
                <li>
                  <a href="#" class="block px-8 py-2 hover:bg-gray-700 hover:text-white font-semibold uppercase">history</a>
                </li>
                <li>
                  <a href="#" class="block px-8 py-2 hover:bg-gray-700 hover:text-white font-semibold uppercase">vision mission</a>
                </li>
              </ul>
          </div>
            <a class="text-sm p-3 font-semibold text-gray-500 uppercase hover:bg-gray-200 " href="#">our work</a>
            <a class="text-sm p-3 font-semibold text-gray-500 uppercase hover:bg-gray-200 " href="#">our team</a>
            <a class="text-sm p-3 font-semibold text-gray-500 uppercase hover:bg-gray-200 " href="#">contact</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { createPopper } from "@popperjs/core";
export default {
    data() {
        return {
            tooltipShow: false
        }
    },
    methods: {
      toggleTooltip: function(){
        if(this.tooltipShow){
          this.tooltipShow = false;
        } else {
          this.tooltipShow = true;
          createPopper(this.$refs.btnRef, this.$refs.tooltipRef, {
            placement: "bottom"
          });
        }
      },
    }
}
</script>

<style>

</style>