<template>
  <header
      class="header header__wrapper"
  >
    <div class="container">
      <Nav class="header__nav-wrapper" />
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

