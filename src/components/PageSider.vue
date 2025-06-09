<template>
  <a-layout-sider width="200" style="background: #fff">
    <a-menu
      v-model:selectedKeys="selectedKeys2"
      v-model:openKeys="openKeys"
      mode="inline"
      :style="{ height: '100%', borderRight: 0 }"
    >
      <a-sub-menu key="sub1">
        <template #title>
          <span>
            <user-outlined />
            subnav 1
          </span>
        </template>
        <a-menu-item key="5">option1</a-menu-item>
        <a-menu-item key="6">option2</a-menu-item>
        <a-menu-item key="7">option3</a-menu-item>
        <a-menu-item key="8">option4</a-menu-item>
      </a-sub-menu>
      <a-sub-menu key="sub2">
        <template #title>
          <span>
            <laptop-outlined />
            subnav 2
          </span>
        </template>
        <a-menu-item key="9">option5</a-menu-item>
        <a-menu-item key="10">option6</a-menu-item>
        <a-menu-item key="11">option7</a-menu-item>
        <a-menu-item key="12">option8</a-menu-item>
      </a-sub-menu>
      <a-sub-menu key="sub3">
        <template #title>
          <span>
            <notification-outlined />
            subnav 3
          </span>
        </template>
        <a-menu-item key="13">option9</a-menu-item>
        <a-menu-item key="14">option10</a-menu-item>
        <a-menu-item key="15">option11</a-menu-item>
        <a-menu-item key="16">option12</a-menu-item>
      </a-sub-menu>
    </a-menu>
  </a-layout-sider>
</template>
<script lang="ts" setup>
import { UserOutlined, LaptopOutlined, NotificationOutlined } from '@ant-design/icons-vue'
import { ref } from 'vue'
const selectedKeys2 = ref<string[]>(['1'])
const openKeys = ref<string[]>(['sub1'])
</script>
<style scoped></style>
