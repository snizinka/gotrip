<template>
  <section class="subscription">
    <div class="subscription__container container">
      <h2 class="subscription__title title">
        Subscribe
        <br>
        To Our Newsletter
      </h2>
      <SubscriptionInput />
    </div>
  </section>
</template>

<style lang="scss">
@import "@/assets/styles/subscription";
</style>
<script setup lang="ts">
import SubscriptionInput from "@/components/Subscription/SubscriptionInput.vue";
</script>
