<template>
  <section class="reviews">
    <div class="container">
      <div class="reviews__row">
        <Item />
        <Item />
        <Item />
        <Item />
      </div>
    </div>
  </section>
</template>

<script>
import Item from "./Item.vue";
export default {
  components: { Item },
};
</script>


<style>
.reviews {
  padding: 80px;
  background-color: #fff;
}
.reviews__row {
  display: flex;
}
.reviews-item {
  width: 25%;
  text-align: center;
}
@media (max-width:756px) { 
.reviews_row {
    width: 100%;
    flex-direction: column;
    padding-top: 60px;
}
}
</style>