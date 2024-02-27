<template>
  <div class="descriptions-container">
    <descriptions size='mini'></descriptions>
    <a-descriptions style="margin-top: 20px" :data="data" :size="size" :title="title" :column="1"/>
    <img :src="imgSrc" class="img-movie">
  </div>
</template>

<script>
export default {
  props: {
    title:String,
    data: Array,
    imgSrc: String
  },
  setup() {
    const size = 'medium'; // 可以根据需要设定默认值或者从父组件传递

    return {
      size
    };
  },
};
</script>

<style>
.descriptions-container {
  margin-left: 3%;
  height: 155px;
}
.img-movie{
  position: relative;
  right: -80%;
  width: 100px;
  top: -120px;
}
</style>