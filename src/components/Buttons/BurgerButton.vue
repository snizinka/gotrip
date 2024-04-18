<template>
  <button
      :class="{ 'burger-btn__wrapper--open': isOpen }"
      class="burger-btn"
      @click="toggleIsOpen"
  >
    <span class="burger-btn__line" />
    <span class="burger-btn__line" />
    <span class="burger-btn__line" />
    <span class="burger-btn__line" />
    <span class="burger-btn__line" />
    <span class="burger-btn__line" />
  </button>
</template>

<script setup lang="ts">
import {ref} from "vue";
const emit = defineEmits(['openStateToggle'])
const isOpen = ref(false)

function toggleIsOpen () {
  isOpen.value = !isOpen.value
  emit('openStateToggle', isOpen.value)
}
</script>
