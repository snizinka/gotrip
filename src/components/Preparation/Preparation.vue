<template>
  <section class="preparation preparation__wrapper">
    <div class="container preparation__container">
      <h2 class="preparation__title title">Prepare Yourself And Start Exploring With Us.</h2>
      <h3 class="preparation__subtitle description">There's the best discount for you today.</h3>
      <ActionButton class="preparation__btn action-btn--medium">Get Started</ActionButton>
      <img src="@/assets/images/preparation/prepare_decor_1.svg" alt="" class="preparation__bulb preparation__bulb--right-top">
      <img src="@/assets/images/preparation/prepare_decor_2.svg" alt="" class="preparation__bulb preparation__bulb--left-bottom">
    </div>
  </section>
</template>

<style lang="scss">
@import "@/assets/styles/preparation";
</style>
<script setup lang="ts">
import ActionButton from "@/components/Buttons/ActionButton.vue";
</script>
