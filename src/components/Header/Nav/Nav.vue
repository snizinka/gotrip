<template>
  <div class="nav">
    <a href="#" class="logo">GoTrip</a>
    <div class="nav__items">
      <BurgerButton @open-state-toggle="openStateToggle" />
      <nav
          :class="{ 'nav-wrapper__container--active': isOpen }"
          class="nav-wrapper"
      >
        <ul class="nav-wrapper__list">
          <NavListItem class="active">Home</NavListItem>
          <NavListItem>Services</NavListItem>
          <NavListItem>Pricing</NavListItem>
          <NavListItem>Contact</NavListItem>
        </ul>
        <ul class="nav-wrapper__buttons">
          <li>
            <button class="nav-wrapper__list-link nav-wrapper__list-sign-up-btn sign-up-btn">Sign up</button>
          </li>
          <li>
            <LoginButton />
          </li>
        </ul>
      </nav>
    </div>
  </div>
</template>
<script setup lang="ts">
import LoginButton from "@/components/Header/Buttons/LoginButton.vue";
import NavListItem from "@/components/Header/Nav/NavListItem.vue";
import BurgerButton from "@/components/Buttons/BurgerButton.vue";
import {ref} from "vue";

const isOpen = ref(false)

function openStateToggle (isOpenState) {
  isOpen.value = isOpenState
}
</script>
