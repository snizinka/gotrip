<template>
  <div class="header__content exploration">
    <div>
      <ActionButton class="header__exploration-btn">explore the world</ActionButton>
      <h1 class="header__exploration-title">
        Explore The Natural
        Beauty Of Halmahera
        With Us
      </h1>
      <h4 class="header__exploration-description">explore the beauty of god's earth in a beautiful forest and have fun</h4>
      <ActionButton class="header__explore-now-btn">Explore Now</ActionButton>
    </div>
    <div class="exploration__image-wrapper">
      <img src="@/assets/images/header/woman_with_a_hat.png" alt="Explorer" class="exploration__image">
      <BackgroundDecoration />
    </div>
  </div>
</template>
<script setup lang="ts">
import ActionButton from "@/components/Buttons/ActionButton.vue";
import BackgroundDecoration from "@/components/Header/BackgroundDecoration.vue";
</script>
