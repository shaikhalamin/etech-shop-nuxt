<template>
  <b-row class="border-top bg-dark">
    <b-col>
      <b-row class="mt-5 mb-1">
        <b-col>
          <h3 class="text-center text-white font-weigth-bold" style="font-size: 22px">
            Etech-shop
          </h3>
          <p class="text-center text-white" style="font-size: 13px">
            Find yours greate products at etech-shop
          </p>
        </b-col>
      </b-row>
      <b-container>
        <b-row>
          <b-col>
            <h4 class="text-justify text-white mt-2 mb-2">Support</h4>
            <ul>
              <li>
                <p class="text-white ft-12">8AM-9PM</p>
                <p class="text-white ft-12">09389348347</p>
              </li>
              <li>
                <p class="text-white ft-12">Store Locator</p>
                <p class="text-white ft-12">Find Our Store</p>
              </li>
            </ul>
          </b-col>
          <b-col>
            <h4 class="text-center text-white mt-2 mb-2">About Us</h4>
            <b-row>
              <b-col>
                <ul>
                  <li class="text-white ft-12">EMI</li>
                  <li class="text-white ft-12">Privacy Policy</li>
                  <li class="text-white ft-12">Etech Policy</li>
                  <li class="text-white ft-12">Brands</li>
                </ul>
              </b-col>
              <b-col>
                <ul>
                  <li class="text-white ft-12">About Us</li>
                  <li class="text-white ft-12">Terms and Conditions</li>
                  <li class="text-white ft-12">Blog</li>
                  <li class="text-white ft-12">Online Support</li>
                </ul>
              </b-col>
            </b-row>
          </b-col>
          <b-col>
            <h4 class="text-justify text-white">Stay Connected</h4>
            <ul>
              <li class="text-white ft-12">Etech Shops</li>
              <li class="text-white ft-12">Kuwati Masjid Road,Uttar Badda, Dhaka - 1212</li>
              <li class="text-white ft-12">Email: alamin.cse15@gmail.com</li>
            </ul>
          </b-col>
        </b-row>
        <b-row class="border-top">
          <b-col class="text-center text-white mt-1 mb-2">&copy; Etech-shops {{ new Date().getFullYear().toString() }}</b-col>
        </b-row>
      </b-container>
    </b-col>
  </b-row>
</template>

<script lang="ts">
import Vue from "vue";
export default Vue.extend({});
</script>