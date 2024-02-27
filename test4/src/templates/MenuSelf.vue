<template>
    <div class="menu-demo">
      <a-menu mode="horizontal" :default-selected-keys="['1']">
        <a-menu-item key="0" :style="{ padding: 0, marginRight: '38px' }" disabled>
          <!-- <div
            :style="{
              width: '80px',
              height: '8px',
              borderRadius: '2px',
              background: 'var(--color-fill-3)',
              cursor: 'text',
            }"
          /> -->
        </a-menu-item>
        <a-menu-item key="1">首页</a-menu-item>
        <a-menu-item key="2">电影详情</a-menu-item>
        <a-menu-item key="3">电影排行</a-menu-item>
        <a-menu-item key="4">面包</a-menu-item>
      </a-menu>
    </div>
  </template>
  <style scoped>
  .menu-demo {
    box-sizing: border-box;
    width: 100%;
    /* padding: 40px; */
    background-color: var(--color-neutral-2);
  }
  </style>