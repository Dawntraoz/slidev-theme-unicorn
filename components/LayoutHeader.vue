<template>
  <header v-if="logoHeader">
    <img :src="logoHeader" width="60" height="60" class="object-contain" />
  </header>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
    logoHeader: {
      type: String,
    },
  })
</script>
