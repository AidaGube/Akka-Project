
  <template>
  <section class="partfolio">
    <div class="container">
      <TagH className="partfolio__title" type="h2">
        Н2 - ПОРТФОЛИО САЙТОВ
      </TagH>
      <div class="partfolio__row">
        <Item />
        <Item />
        <Item />
        <Item />
      </div>
    </div>
  </section>
</template>


<script>
import TagH from "@/components/TagH/TagH.vue";
import Item from "./Item.vue";
export default {
  components: { Item, TagH },
};
</script>

<style>
.partfolio__row {
  display: flex;
}
.partfolio {
  background-color: #fff;
  padding: 80px 0;
}
.partfolio__title {
  margin-bottom: 45px;
}
.partfolio__subtitle {
  padding: 30px 0 7px;
  text-align: left;
}
.partfolio-item {
  text-align: left;
  width: 25%;
  background: #f5f7f9;
  border-radius: 20px;
  padding: 20px 20px 20px;
  margin-left: 15px;
}

.partfolio-item__description {
  display: inline-block;
  font-family: Gilroy;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 16px;
}
</style>