<template>
  <div class="partfolio-item">
    <img :src="PartfolioImg" />
    <img :src="PartfolioImgTwo" />
    <TagH className="partfolio__subtitle" type="h5">
      Продвижение по позициям
    </TagH>
    <div class="partfolio-item__description">ecutools.ru</div>
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import PartfolioImg from "@/assets/partfolio-1.png";
export default {
  components: { TagH },
  data() {
    return {
      PartfolioImg,
    };
  },
};
</script>

<style>
</style>

