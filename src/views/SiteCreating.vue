<template>
  <main>
    <HeaderSite />
    <ApplyForm />
    <Reviews />
    <Tariffs />
    <Rates />
    <Partfolio />
  </main>
</template>

<script>
import Calculator from "@/components/Calculator/Calculator.vue";
import Rates from "@/components/Rates/Rates.vue";
import ApplyForm from "../components/ApplyForm/ApplyForm.vue";
import Reviews from "../components/Reviews/Review.vue";
import Partfolio from "../components/Partfolio/Partfolio.vue";
import Tariffs from "../components/Tariffs/Tariffs.vue";
import Footer from "../components/Footer/Footer.vue";
import HeaderSite from "../components/HeaderSiteCreating/HeaderSite.vue";
import TagH from "../components/TagH/TagH.vue";
export default {
  components: {
    Calculator,
    Rates,
    TagH,
    ApplyForm,
    Reviews,
    Tariffs,
    Partfolio,
    Footer,
    HeaderSite ,
  },
};
</script>

<style>
</style>