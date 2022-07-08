<template>
  <b-container>
    <b-row class="mt-5 mb-1">
      <b-col>
        <h3 class="text-center font-weigth-bold" style="font-size: 22px">
          Todays Top Deals
        </h3>
        <p class="text-center" style="font-size: 13px">Find yours exiting deals now</p>
      </b-col>
    </b-row>
    <b-row>
      <b-col class="border ml-1 mr-1">
        <h4 class="mb-0 mt-2 font-weigth-bold" style="font-size: 14px">Explore More Budget PC</h4>
        <hr />
        <b-row>
          <b-col v-for="(pc, i) in topDeals.budgets_pcs" :key="i" class="ml-1 mr-1">
            <b-row class="mt-1">
              <b-col style="width: 160px; height: 160px" class="border">
                <img
                  :src="
                    require(`~/assets/images/landingpage/topdeals/budgetpcs/${pc.product_image_url}.webp`)
                  "
                  alt="cpu-cooler"
                  class="img-fluid"
                />
              </b-col>
            </b-row>
            <p class="text-justify mt-4" style="font-size: 12px">
              {{ pc.name.slice(0,45) }}{{ `...` }}
            </p>
            <p class="text-justify mt-1" style="font-size: 12px">
              ${{ pc.price }}
            </p>
          </b-col>
        </b-row>
      </b-col>
      <b-col class="border ml-1 mr-1">
        <h4 class="mb-0 mt-2 font-weigth-bold" style="font-size: 14px">Explore More Monitors</h4>
        <hr />
        <b-row>
          <b-col v-for="(pc, i) in topDeals.budgets_pcs" :key="i" class="ml-1 mr-1">
            <b-row class="mt-1">
              <b-col style="width: 160px; height: 160px" class="border">
                <img
                  :src="
                    require(`~/assets/images/landingpage/topdeals/budgetpcs/${pc.product_image_url}.webp`)
                  "
                  alt="cpu-cooler"
                  class="img-fluid"
                />
              </b-col>
            </b-row>
            <p class="text-justify mt-4" style="font-size: 12px">
              {{ pc.name.slice(0,45) }}{{ `...` }}
            </p>
            <p class="text-justify mt-1" style="font-size: 12px">
              ${{ pc.price }}
            </p>
          </b-col>
        </b-row>
      </b-col>
      <b-col class="border ml-1 mr-1">
        <h4 class="mb-0 mt-2 font-weigth-bold" style="font-size: 14px">Explore More Graphics Cards</h4>
        <hr />
        <b-row>
          <b-col v-for="(pc, i) in topDeals.budgets_pcs" :key="i" class="ml-1 mr-1">
            <b-row class="mt-1">
              <b-col style="width: 160px; height: 160px" class="border">
                <img
                  :src="
                    require(`~/assets/images/landingpage/topdeals/budgetpcs/${pc.product_image_url}.webp`)
                  "
                  alt="cpu-cooler"
                  class="img-fluid"
                />
              </b-col>
            </b-row>
            <p class="text-justify mt-4" style="font-size: 12px">
              {{ pc.name.slice(0,45) }}{{ `...` }}
            </p>
            <p class="text-justify mt-1" style="font-size: 12px">
              ${{ pc.price }}
            </p>
          </b-col>
        </b-row>
      </b-col>
      
    </b-row>
    <b-row>
      <b-col> </b-col>
      <b-col></b-col>
      <b-col></b-col>
    </b-row>
  </b-container>
</template>
<script lang="ts">
import Vue from "vue";
export default Vue.extend({
  data() {
    return {
      topDeals: {
        budgets_pcs: [
          {
            name: "AMD ryzen 5 5600x asus tuf gaming b550m-e 16gb ram 500gb ssd rtx 3060 ti 8gb graphics card budget pc",
            url: "/",
            product_image_url: "asus_amd_ryzen_5_5600x",
            price: "45000",
          },
          {
            name: "Intel core i5-12400 12th gen gigabyte b660m gaming x 8gb 3200mhz ram 500gb nvme pcie ssd budget pc",
            url: "/",
            product_image_url: "intel_core_i5_12400",
            price: "89000",
          },
        ],
        monitors: [],
        smart_watches: [],
        smart_tvs: [],
        gaming_chairs: [],
        graphics_cards: [],
      },
    };
  },
});
</script>