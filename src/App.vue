<script lang="ts" setup>
import PageHeader from './components/PageHeader.vue'
import PageSider from './components/PageSider.vue'
import PageContent from './components/PageContent.vue'
import PageFooter from './components/PageFooter.vue'
</script>

<template>
  <a-layout style="min-height: 100vh">
    <page-header />
    <a-layout>
      <page-sider />
      <a-layout style="padding: 0 24px 24px">
        <page-content />
      </a-layout>
    </a-layout>
    <page-footer />
  </a-layout>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
