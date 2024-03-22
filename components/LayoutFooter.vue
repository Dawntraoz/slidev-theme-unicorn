<template>
  <footer
    v-if="website || handle"
    class="mt-auto flex justify-between w-full text-fuchsia-700 dark:text-white"
  >
    <p v-if="website" class="mb-0">{{ website }}</p>
    <p v-if="handle" class="mb-0">@{{ handle }}</p>
  </footer>
</template>

<script setup lang="ts">
const props = defineProps({
  website: {
    type: String,
  },
  handle: {
    type: String,
  },
});
</script>
