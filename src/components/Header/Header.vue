<template>
  <header class="header header__wrapper">
    <div class="container">
      <div class="header__top">
        <a href="#" class="header__logo logo">GoTrip</a>
        <Nav class="header__nav-wrapper" />
      </div>
      <Content />
    </div>
    <BottomPart />
  </header>
</template>

<style lang="scss">
@import "@/assets/styles/header";
@import "@/assets/styles/buttons";
</style>

<script setup lang="ts">
import Nav from "@/components/Header/Nav/Nav.vue";
import Content from "@/components/Header/Content.vue";
import BottomPart from "@/components/Header/BottomPart.vue";
</script>

