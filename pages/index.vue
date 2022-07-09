<template>
  <div>
    <LandingNavbar />
    <LandingHeader />
    <FeaturedCategory />
    <FeaturedItems />
    <GamingPc />
    <TopDeals />
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import LandingNavbar from "~/components/navbar/LandingNavbar.vue";
import LandingHeader from "~/components/header/LandingHeader.vue";
import FeaturedCategory from "~/components/homepage/FeaturedCategory.vue";
import FeaturedItems from "~/components/homepage/FeaturedItems.vue";
import GamingPc from "~/components/homepage/GamingPc.vue";
import TopDeals from "~/components/homepage/TopDeals.vue";
import Footer from "~/components/footer/Footer.vue";

export default Vue.extend({
  components: {
    LandingNavbar,
    LandingHeader,
    FeaturedCategory,
    FeaturedItems,
    GamingPc,
    TopDeals,
    Footer,
  },
  name: "Index",
});
</script>
              