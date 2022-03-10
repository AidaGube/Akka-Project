<template>
  <div class="keywords">
    <TagH className="keywords__title" type="h3"
      >Работа с ключевыми словами</TagH
    >
    <div class="analysys__bottom">
      <div class="keywords__row" v-for="item in items" :key="item.id">
        <Content :title="item.title" :description="item.description" />
        <Marks :marks="item.marks" />
      </div>
    </div>
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import Content from "./Content.vue";
import Marks from "./Marks.vue";
export default {
  components: { TagH, Content, Marks },
  props: ["items"],
};
</script>

<style>
.keywords__title {
  border-radius: 5px;
  padding: 8px 0;
  background: linear-gradient(0deg, #77cbfa, #77cbfa), #f4f7fe;
}
.keywords__row {
  display: flex;
  border-bottom: 2px solid #eaecef;
  margin-bottom: 20px;
}
.keywords__row:first-child .table__item {
  padding-top: 35px;
}
.keywords__row:last-child {
  border-bottom: none;
}
.keywords__row:last-child .table__item {
  padding-bottom: 35px;
}
.keywords__subtitle {
  text-align: left;
  margin-bottom: 10px;
}
</style>