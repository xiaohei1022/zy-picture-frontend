<template>
  <div id="basicLayout">
    <a-layout style="min-height: 100vh">
      <a-layout-header class="header">
        <GlobalHeader />
      </a-layout-header>
      <a-layout-content class="content">
        <router-view />
      </a-layout-content>
    </a-layout>
    <a-layout-footer class="footer"> 程序员展岩 </a-layout-footer>
  </div>
</template>

<script setup lang="ts">
import GlobalHeader from '@/components/GlobalHeader.vue'
import HomePage from '@/pages/HomePage.vue'
</script>

<style>
#basicLayout {
}

#basicLayout .footer {
  background: #efefef;
  padding: 16px;
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  text-align: center;
}
#basicLayout .header {
  padding-inline: 20px;
  margin-bottom: 16px;
  color: unset;
  background: white;
}
 #basicLayout .content {
   background: linear-gradient(to right, #fefefe, #fff);
   margin-bottom: 28px;
   padding: 20px;
 }
</style>
