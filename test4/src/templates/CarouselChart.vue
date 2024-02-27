<template>
  <a-carousel
    :style="{
      width: '60%',
      height: '240px',
    }"
    :auto-play="true"
    indicator-type="dot"
    show-arrow="hover"
  >
  <carousel move-speed="100"></carousel>
    <a-carousel-item v-for="image in images" :key="image.id" style="display: flex; justify-content: center;">
      <img
        :src="image"
        :style="{
          height: '100%',
        }"
      />
    </a-carousel-item>
  </a-carousel>
</template>
<!-- <template>
    <a-carousel
      :autoPlay="true"
      animation-name="card"
      show-arrow="never"
      indicator-position="outer"
      :style="{
        width: '60%',
        height: '120px',
        
      }"
    >
    <carousel move-speed="100"></carousel>
      <a-carousel-item v-for="image in images" :style="{ width: '60%' }" :key="image.id" style="display: flex; justify-content: center;">
        <img
          :src="image"
          :style="{
            height: '100%',
          }"
        />
      </a-carousel-item>
    </a-carousel>
  </template>
   -->
  <script>
  export default {
    setup() {
      const images = [
        require('@/imgs/a2d4da54f32361acf1a1da254bc5b6e8.png'),
        require('@/imgs/a8a6622e814d2fd061057b52bfbe8963.png'),
        require('@/imgs/ed72da2c2eefd55e2b7642cf1699c46a.jpg'),
        require('@/imgs/ed72da2c2eefd55e2b7642cf1699c46a.jpg'),
      ];
      return {
        images
      }
    },
  };
  </script>
  
  <style>
  </style>
  