<template>
  <nav class="nav">
    <ul class="nav__list">
      <NavListItem class="active">Home</NavListItem>
      <NavListItem>Services</NavListItem>
      <NavListItem>Pricing</NavListItem>
      <NavListItem>Contact</NavListItem>
    </ul>
    <ul class="nav__buttons">
      <li>
        <button class="nav__list-link nav__list-sign-up-btn sign-up-btn">Sign up</button>
      </li>
      <li>
        <LoginButton />
      </li>
    </ul>
  </nav>
</template>
<script setup lang="ts">
import LoginButton from "@/components/Header/Buttons/LoginButton.vue";
import NavListItem from "@/components/Header/Nav/NavListItem.vue";
</script>
