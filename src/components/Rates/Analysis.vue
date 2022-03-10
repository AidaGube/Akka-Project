<template>
  <div class="analysis">
    <TagH className="analysis__title" type="h3"> Глубокий анализ</TagH>
    <div class="analysys__bottom">
      <div class="analysis__row" v-for="item in items" :key="item.id">
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
.analysis__title {
  border-radius: 5px;
  padding: 8px 0;
  background: linear-gradient(0deg, #ffd773, #ffd773), #f4f7fe;
}
.analysis__row {
  display: flex;
  border-bottom: 2px solid #eaecef;
  margin-bottom: 20px;
}
.analysis__row:first-child .table__item {
  padding-top: 35px;
}
.analysis__row:last-child {
  border-bottom: none;
}
.analysis__row:last-child .table__item {
  padding-bottom: 35px;
}
</style>