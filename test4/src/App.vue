<template>
  <div>
    <MenuSelf></MenuSelf>
    <div class="carousel-container">    
      <carouselChart></carouselChart>

    </div>
    <div>
    <template v-for="(item, index) in items" :key="index">
      <ProductDetails :title="item.title" :data="item.data" :imgSrc="item.imgSrc" />
    </template>
  </div>
  </div>
</template>

<script>
import MenuSelf from './templates/MenuSelf.vue';
import carouselChart from './templates/CarouselChart';
import ProductDetails from './templates/ProductDetails'
export default{
  // eslint-disable-next-line vue/multi-word-component-names
  
  data() {
    return {
      items: [
        {
          title:'周处除三害',
          data: [
            { label: '上映日期:', value: '2023-12-08(中国大陆)' },
            { label: '导演', value: '黄精甫' },
            { label: '类型', value: ' 动作 / 犯罪' }
          ],
          imgSrc: require('@/imgs/p2903830747.webp')
        },
        {
          title:'照明商店',
          data: [
            { label: '上映日期', value: '2023-12-09(中国大陆)' },
            { label: '导演', value: '蔡耳朵' },
            { label: '类型', value: ' 剧情 / 悬疑 / 奇幻' }
          ],
          imgSrc: require('@/imgs/p2901397955.webp')
        },
        {
          title:'三大队',
          data: [
            { label: '上映日期:', value: '2023-12-08(中国大陆)' },
            { label: '导演', value: '黄精甫' },
            { label: '类型', value: ' 动作 / 犯罪' }
          ],
          imgSrc: require('@/imgs/p2901703469.webp')
        },
        {
          title:'零时劫案',
          data: [
            { label: '上映日期:', value: '2023-12-08(中国大陆)' },
            { label: '导演', value: '黄精甫' },
            { label: '类型', value: ' 动作 / 犯罪' }
          ],
          imgSrc: require('@/imgs/p2902984351.webp')
        },
        {
          title:'养峰人',
          data: [
            { label: '上映日期:', value: '2023-12-08(中国大陆)' },
            { label: '导演', value: '黄精甫' },
            { label: '类型', value: ' 动作 / 犯罪' }
          ],
          imgSrc: require('@/imgs/p2902861438.webp')

        }
        // 可以根据需要添加更多子组件的数据
      ]
    };
  },
  components:{
    MenuSelf,
    carouselChart,
    ProductDetails
  }
}

</script>

<style>
  .carousel-container {
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
