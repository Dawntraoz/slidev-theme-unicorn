<template>
  <default class="image-center">
    <div class="flex flex-col">
      <slot />
      <img :src="image" alt="Slide image" :width="imageWidth" :height="imageHeight" class="rounded-md shadow-lg  m-auto object-contain" />
    </div>
  </default>
</template>

<script setup lang="ts">
import { defineProps, defineComponent } from 'vue'
import Default from '../layouts/default.vue'

const components = defineComponent({ Default })
const props = defineProps({
  image: {
    type: String,
  },
  imageWidth: {
    type: String,
  },
  imageHeight: {
    type: String,
  },
})
</script>
