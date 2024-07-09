<script setup>
import { ref } from 'vue';
import ListComponent from './ListComponent.vue';
import ListItem from './ListItem.vue';

const list = ref([
  {text: 'text0', index: 0},
  {text: 'text1', index: 1},
  {text: 'text2', index: 2},
]);
const index = ref(0);
</script>

<template>
  <h1>Current Index: {{ index }}</h1>
  <ListComponent
    :index="index"
    :list="list"
    @change="index = $event"
    v-slot="{ item }"
  >
    <ListItem :listContent="item" />
  </ListComponent>
</template>
