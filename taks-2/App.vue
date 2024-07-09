<script setup>
import { ref, watch } from 'vue';
import Modal from './Modal.vue';

const isModalAccepted = ref(undefined);

watch(isModalAccepted, (newValue) => {
  if(newValue === false) {
    alert('You have accept cookies to display the message');
  }
}, {immediate: false})
</script>

<template>
  <div v-if="isModalAccepted">Display this div only if cookie accepted</div>
  <Modal
    v-model="isModalAccepted"
  />
</template>
