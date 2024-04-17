<script setup lang="ts">
import Header from "@/components/Header/Header.vue";
import Destination from "@/components/Destination/Destination.vue";
import Feedback from "@/components/Feedback/Feedback.vue";
import Preparation from "@/components/Preparation/Preparation.vue";
import Subscription from "@/components/Subscription/Subscription.vue";
import Footer from "@/components/Footer/Footer.vue";
</script>

<template>
  <div>
    <Header />
    <main class="go-trip-main">
      <Destination />
      <Feedback />
      <Preparation />
      <Subscription />
    </main>
    <Footer />
  </div>
</template>
