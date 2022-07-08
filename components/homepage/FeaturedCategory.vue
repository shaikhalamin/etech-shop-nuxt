<template>
  <div>
    <b-row class="mt-3 mb-2">
      <b-col>
        <h3 class="text-center font-weigth-bold" style="23px;">Featured Category</h3>
        <p class="text-center" style="12px;">
          Check & Get Your Desired Product from Featured Category!
        </p>
      </b-col>
    </b-row>
    <b-row class="mt-1">
      <b-col>
        <b-container>
          <b-row>
            <b-col v-for="(category, i) in featured_categories_top" :key="i" class="border ml-1 mr-1" >
              <b-row class="mt-4">
                <b-col style="width: 70px; height: 45px">
                  <img
                    :src="require(`~/assets/images/landingpage/icons/${category.src}.png`)"
                    alt="cpu-cooler"
                    class="img-fluid"
                  />
                </b-col>
              </b-row>
              <p class="text-center mt-4" style="font-size:12px">{{ category.name }}</p>
            </b-col>
          </b-row>
        </b-container>
      </b-col>
    </b-row>
    <b-row class="mt-1">
      <b-col>
        <b-container>
          <b-row>
            <b-col v-for="(category, i) in featured_categories_down" :key="i" class="border ml-1 mr-1" >
              <b-row class="mt-4">
                <b-col style="width: 70px; height: 45px">
                  <img
                    :src="require(`~/assets/images/landingpage/icons/${category.src}.png`)"
                    alt="cpu-cooler"
                    class="img-fluid"
                  />
                </b-col>
              </b-row>
              <p class="text-center mt-4" style="font-size:12px">{{ category.name }}</p>
            </b-col>
          </b-row>
        </b-container>
      </b-col>
    </b-row>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      featured_categories_top: [
        {
          name: "Action Camera",
          src: "camera",
        },
        {
          name: "Gimbel",
          src: "gimbal",
        },
        {
          name: "Smart Watch",
          src: "smartwatch",
        },
        {
          name: "Graphics Tablet",
          src: "tablet",
        },
        {
          name: "Head Phones",
          src: "headphones",
        },
        {
          name: "Mother Board",
          src: "motherboard",
        },
        {
          name: "Processor",
          src: "processor",
        },
        {
          name: "Ram",
          src: "ram",
        },
      ],
      featured_categories_down: [
        {
          name: "Monitor",
          src: "monitor",
        },
        {
          name: "Graphics Card",
          src: "graphicscard",
        },
        {
          name: "Smart Tv",
          src: "smart_tv",
        },
        {
          name: "Laptop",
          src: "laptop",
        },
        {
          name: "Printer",
          src: "printer",
        },
        {
          name: "Cpu Cooler",
          src: "cpu_cooler",
        },
        {
          name: "Mouse",
          src: "mouse",
        },
        {
          name: "Key Board",
          src: "keyboard",
        },
      ],
    };
  },
});
</script>