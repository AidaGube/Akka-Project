<template>
  <div class="price-item">
    <TagH type="h2"> 1047 </TagH>
    <p class="price__title">Небольшое описание в 2 строчки</p>
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
export default {
  components: { TagH },
};
</script>

<style>
.price {
  padding: 80px;
  background-color: #fff;
}
.price__row {
  display: flex;
  padding: 40px;
}
.price-item {
  border-right: 2px solid #eaecef;
  width: 25%;
  text-align: center;
}
.price-item:last-child {
  border-right: none;
}
.price__title {
  padding: 12px 0 0;
  display: inline-block;
  width: 150px;
  font-family: Gilroy;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 16px;
  color: #272727;
}
</style>