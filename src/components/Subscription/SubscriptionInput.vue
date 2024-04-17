<template>
  <form class="subscription-form subscription-form__wrapper">
    <input type="text" placeholder="Yourmail@mail.com" class="subscription-form__input">
    <ActionButton class="subscription-form__btn">Subscribe</ActionButton>
  </form>
</template>
<script setup lang="ts">
import ActionButton from "@/components/Buttons/ActionButton.vue";
</script>
