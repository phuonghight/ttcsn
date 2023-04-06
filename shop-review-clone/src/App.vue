<script setup>
import Header from '@/components/Header.vue';
import NavBarHeader from './components/NavBarHeader.vue';
</script>

<template>
  <div>
    <Header />
    <nav-bar-header />
    <router-view></router-view>
  </div>
</template>
