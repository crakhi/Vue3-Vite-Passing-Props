<script setup>
import { ref } from 'vue'
import TitleChild from '@/components/TitleChild.vue'

const msg = ref('Hello World!')
</script>

<template>
  <input v-model="msg">

  <TitleChild :titleP="msg" />
</template>