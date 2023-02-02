<template>
  BODY: {{ bodyP }}
  <br />
  <br />
  <br />
</template>

<script setup>
import { ref, defineProps } from 'vue'
const props = defineProps(['bodyP'])
</script>
