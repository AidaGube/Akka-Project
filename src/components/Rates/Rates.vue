<template>
  <section class="rates">
    <div class="container">
      <TagH type="h2"> Сравнение тарифов </TagH>
      <div class="rates__titles">
        <span>Продвинутый</span>
        <span>Комплексный</span>
        <span>Оптимизация</span>
        <span>Потрясающий</span>
      </div>
      <Analysis :items="items" />
      <Keywords :items="itemsKeywords" />
      <div class="rates__btns">
        <div>
          <TagH type="h4"> 30 680 ₽ </TagH>
          <Button text="Выбрать" />
        </div>
        <div>
          <TagH type="h4"> 21 590 ₽ </TagH>
          <Button text="Выбрать" />
        </div>
        <div>
          <TagH type="h4"> 21 590 ₽ </TagH>
          <Button text="Выбрать" />
        </div>
        <div>
          <TagH type="h4"> 13 500 ₽ </TagH>
          <Button text="Выбрать" />
        </div>
      </div>
    </div>
  </section>
</template>1

<script>
import TagH from "@/components/TagH/TagH.vue";
import Keywords from "./Keywords.vue";
import Analysis from "./Analysis.vue";
import Button from "@/components/Buttons/Button";
export default {
  components: { TagH, Analysis, Keywords, Button },
  data() {
    return {
      items: [
        {
          id: 1,
          marks: [true, false, false, true],
          title: "Общий аудит сайта",
          description: "SEO, юзабилити, тексты. Пример аудита",
        },
        {
          id: 2,
          marks: [false, true, false, true],
          title: "Общий аудит сайта",
          description:
            "Определим основных конкурентов, их преимущества и недостатки, выстроим стратегию продвижения, без предоставления отчета",
        },
        {
          id: 3,
          marks: [true, false, true, false],
          title: "Составление семантического ядра",
          description:
            "Страхуем себя и ваш сайт, чтобы ничего не пострадало. Копию храним до 3 месяцев",
        },
      ],
      itemsKeywords: [
        {
          id: 1,
          marks: [true, false, false, true],
          title: "Составление семантического ядра",
          description: "Cписок ключевых слов, по которым будем продвигать сайт",
        },
        {
          id: 2,
          marks: [false, true, false, true],
          title:
            "Кластеризация ключевых слов и составление карты релевантности",
          description:
            "Распределим, какие страницы по каким запросам будем продвигать",
        },
      ],
    };
  },
};
</script>

<style>
.rates__btns {
  display: flex;
  justify-content: flex-end;
}
.rates__btns button {
  padding: 8px 20px;
}
.rates__btns div h4 {
  margin-bottom: 16px;
  text-align: center;
}
.rates__btns div {
  margin-left: 10px;
}
.rates {
  margin: 80px 0 0;
  padding: 80px 0;
  background-color: #fff;
}
.rates__titles {
  margin: 45px 0 20px;
  text-align: right;
}
.rates__titles span {
  cursor: pointer;
  margin-left: 40px;
  font-family: "Fira Sans Extra Condensed";
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 150%;
  text-transform: uppercase;
  color: #333333;
}
</style>