<template>
  <div class="tariffs-item">
    <TagH className="tariffs__title" type="h5"> Продвижение по позициям </TagH>
    <img :src="tariffImg" />
    <div class="tariffs-item__description">
      Продвинем 10 сылок на первые места
    </div>
    <span class="tariffs-item__price">15000 руб</span>
    <Button className="btn-light" text="Оставить заявку" />
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import tariffImg from "@/assets/tariffs-icon.png";
import Button from "@/components/Buttons/Button";
export default {
  components: { TagH, Button },
  data() {
    return {
      tariffImg,
    };
  },
};
</script>

<style>
</style>

