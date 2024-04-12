<script setup lang="ts">
import "vue3-select-component/dist/style.css";

import { ref } from "vue";
import VueSelect from "vue3-select-component";

const selected = ref<string | null>(null);
</script>

<template>
  <VueSelect
    v-model="selected"
    :options="[
      { label: 'Option #1', value: 'option_1' },
      { label: 'Option #2', value: 'option_2' },
      { label: 'Option #3', value: 'option_3' },
    ]"
    placeholder="Select an option"
  />
</template>
