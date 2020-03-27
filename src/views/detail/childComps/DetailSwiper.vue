<template>
  <swiper class="detail-swiper">
    <swiper-item v-for="item in topImages">
      <img :src="item" alt />
    </swiper-item>
  </swiper>
</template>

<script>
import { Swiper, SwiperItem } from "components/common/swiper";
export default {
  name: "DetailSwiper",
  components: { Swiper, SwiperItem },
  props: {
    topImages: {
      type: Array,
      defualt() {
        return [];
      }
    }
  }
};
</script>
<style lang='scss' scoped>
.detail-swiper {
  text-align: center;
  height: 300px;
}
</style>