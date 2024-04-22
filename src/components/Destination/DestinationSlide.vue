<template>
  <img :src="importedImageLink" alt="forest" class="destination-slider__image">
</template>

<script setup lang="ts">
  import {onMounted, ref} from "vue";
  const { imagePath } = defineProps(['imagePath'])

  let importedImageLink = ref('')

  onMounted (async () => {
    try {
      const image = await import(imagePath)
      importedImageLink.value = image.default
    } catch (exception) {
      console.log(exception)
    }
  })
</script>
