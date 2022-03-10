<template>
  <div class="header-site__row">
    <img :src="HeaderImg" />
    <TagH className="header-site__title" type="h1">Создание сайтов</TagH>
  </div>
  <div class="price__row">
 <SitePrice/>
  <SitePrice/>
   <SitePrice/>
    <SitePrice/>
  </div>
     
</template>

<script>
import SitePrice from "@/components/HeaderSiteCreating/SitePrice.vue";
import HeaderImg from "@/assets/headersite.svg";
import TagH from "@/components/TagH/TagH.vue";
export default {
  components: { TagH, SitePrice},
  data() {
    return {
      HeaderImg,
    };
  },
};
</script>

<style>
.header-site__row {
  position: relative;
  max-width: 100%;
}
.header-site__title {
  text-align: center;
  position: absolute;
  top:70px;
  left: 0;
  width: 100%;
}
</style>